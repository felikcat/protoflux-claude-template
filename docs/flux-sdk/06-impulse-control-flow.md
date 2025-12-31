<!--
Source: https://flux-sdk.samsmucny.com/ProtoGraph/Impulse-Control-Flow.html
License: CC BY-NC-SA 4.0
Author: Sam (Papaltine) Smucny
-->

# Impulse Control Flow

Impulses provide explicit instructions on the _order of execution_ of your program: do A _then_ do B _then_ do C...

## Refresher on Froox Context

By default, context expressions exist in the 'froox' context. This context is pure and lazy dataflow programming: values depend on other values, evaluated when requested by downstream nodes.

```
Value1 = 1 + 2 + 3;
Value2 = 4 + 5 + 6;
Value3 = Value1 + 4;
Value4 = Value2 + Value3
```

The order you define values _does not matter_ unless you have a real dataflow dependency. The froox context is _time independent_.

When you need to enforce explicit ordering of operations in time, you need impulses.

## Ways to Use Impulses in Froox Context

### Explicit Arguments

Passing impulses as arguments (continuation passing style):

```
NotifyUser = ErrorMessage <- "Something went wrong";
If(Condition=MaybeTrue, OnFalse=NotifyUser);
```

Good for simple, disconnected impulses. Can lead to "callback hell" for complex chains.

### Switch Expression

More fluent continuation passing style:

```
switch For(Count=100)
| LoopStart |> ImpulseDisplay
| LoopEnd   |> ImpulseDisplay
| LoopIteration ForNode |>
    switch ValueWrite<_>(Value=ForNode.Iteration, Variable=SomeVariable)
    | OnWritten |> ImpulseDisplay
    | OnFail    |> ImpulseDisplay;
```

When you bind the node (like `ForNode`), you can access outputs within switch branches. This ensures valid output values - accessing outputs outside the impulse context gives default values.

Deep nesting leads to the "pyramid of doom".

## Impulse Context

The impulse context layers on top of froox and is _time aware_. Order of declarations matters. Write equivalent of switch expressions using a flatter style:

```
impulse {
    bind ResultUrlIndex = GET_String(SomeUrl).OnResponse;
    bind ResultUrlPath = GET_String(FormatUrlParameters(SomeUrl, ResultUrlIndex.Content)).OnResponse;
    bind ResultFinalUrlPath = GET_String(FormatUrlParameters(ResultUrlPath.Content, ResultUrlIndex.Content)).OnResponse;
    bind ResultValue = GET_String(ResultFinalUrlPath.Content).OnResponse;
    FinalValue <- ParseContent(ResultValue.Content);
}
```

The main limitation: you can only bind to a single continuation. For branching, use explicit arguments or switch expressions inside the impulse context.

> If you leave off `.ContinuationName` from a `bind`, the impulse is sequenced without regard to which continuation it came from. This can cause you to lose control flow information.

```
impulse {
    bind ResultUrlIndex = GET_String(SomeUrl).OnResponse;
    bind ResultUrlPath = GET_String(FormatUrlParameters(SomeUrl, ResultUrlIndex.Content)).OnResponse;
    switch GET_String(FormatUrlParameters(ResultUrlPath.Content, ResultUrlIndex.Content))
    | OnError ErrorNode |>
        impulse {
            NiceMessage = PrettyPrint(ErrorNode.StatusCode);
            ErrorMessage <- NiceMessage;
        }
    | OnDenied |> ErrorMessage <- "You don't have access"
    | OnResponse ResultFinalUrlPath |>
        impulse {
            bind ResultValue = GET_String(ResultFinalUrlPath.Content, OnError=FailCallback).OnResponse;
            FinalValue <- ParseContent(ResultValue.Content);
        };
}
```

> Impulse contexts work best for the "happy path" where everything goes right. Error cases usually break this flow and work better as separate blocks or modules.
>
> Use the "Functional Core, Imperative Shell" design pattern: keep impulses at the edges and make core logic primarily pure data flows.

## Impulse Syntax Sugar

### if

```
if MaybeTrue then impulse {
    // Do things...
} else impulse {
    // Do other things...
}

// The else is optional
if MaybeTrue then impulse {
    // Do things...
}
```

Desugars to the `If` flow node with continuation passing style.

### while / whileAsync

```
local Counter: int;
while Counter < 10 do impulse {
    Counter <- Counter == 0 ? 1 : Counter * 2;
};

// Async variant
local Counter: int;
whileAsync Counter < 10 do impulse {
    DelaySecondsInt(1);
    Counter <- Counter == 0 ? 1 : Counter * 2;
};
```

Desugars to `While` or `AsyncWhile` nodes.

### for / forAsync

```
for _i = 100 to 10 by 8 do impulse {
    RootSlot->~trigger<int>("CountingDown", _i);
}

// Async variant
forAsync _i = 100 to 10 by 8 do impulse {
    RootSlot->~triggerAsync<int>("CountingDown", _i);
}
```

Desugars to `RangeForLoopInt` or `RangeForLoopIntAsync`. Start and end are inclusive, step size defaults to 1.

## Context Colors

The ProtoGraph type system enforces restrictions on what values are allowed in different contexts.

- **froox context**: Time independent, most basic
- **impulse context**: Adds arrow of time

Because impulse is a superset of froox, you can use froox expressions inside impulse, but not vice versa.

### Async Impulses

Within impulse contexts, there's another "color" to be aware of:
- **Synchronous impulses**: Finish immediately
- **Asynchronous impulses**: Finish at unknown future time

You can call synchronous from asynchronous impulses, but NOT asynchronous from synchronous.

Some nodes have async versions. Others "turn into" async when any continuation is async. The `impulse` context usually handles switching automatically.

## Advanced Topics

The closest analogy to the impulse context is the IO monad in Haskell. The impulse wire carries the state of the world with it like a timeline with events executing in causal sequence.

The froox context is analogous to the Reader monad with access to an implicit context (the Froox engine).
