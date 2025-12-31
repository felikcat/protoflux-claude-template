<!--
Source: https://flux-sdk.samsmucny.com/ProtoGraph/Expressions-and-Operators.html
License: CC BY-NC-SA 4.0
Author: Sam (Papaltine) Smucny
-->

# Expressions and Operators

Expressions in ProtoGraph produce, use, and combine data and control flows. All expressions evaluate to a record: a named tuple with key/value pairs. Records also have a `this` field that designates the default value.

## Record Types

Every module invocation returns a record of its outputs:

```
// TimeDelayWithData returns:
// {
//     this: AsyncOperation
//     DelayedValue: T
// }

// Unpack_Float4 returns:
// {
//     X: float
//     Y: float
//     Z: float
//     W: float
// }

// Literals are records with only `this`:
// "MyString": { this: string }
```

## Literal

Values representing constant input nodes:

- Booleans: `true` and `false`
- Integers: `1` and `-2`
- Floating point: `3.14` and `2e30`
- Characters: `'A'` and `'\n'`
- Strings: `"Hello World!"` and `"123-465-7890"`

Number types default to int (32 bit) or float (32 bit if using `.` or exponent). Use suffixes for other types.

## Identifier

A capitalized string of alphanumeric characters referencing modules/nodes or user-defined values:

- Froox Node: `ImpulseDisplay`
- Value: `MyValueX`

## Module Invocation

Invoke a module by writing its identifier. Inputs are specified within `( )`, separated by commas.

Positional arguments must come before named arguments. Unconnected parameters are only allowed for Froox engine nodes. Impulse arguments must be named.

```
If; // If with nothing connected
If(); // same as `If`
If(Condition=true, OnTrue=ImpulseDisplay, OnFalse=ImpulseDisplay); // All named
If(false, OnFalse=ImpulseDisplay); // Some positional, some named
If(OnTrue=ImpulseDisplay, Condition=false); // Named, different order
```

Access outputs using the `.` field accessor. The `this` field is accessed without `.`:

```
MyContext = Context();
MyContext; // => "AB" (the `this` value)
MyContext.A; // => "A"
MyContext.B; // => "B"
```

### Module Aliases

Some common modules have a keyword for simpler syntax:

```
// ValueDisplay<_>(true) or ObjectDisplay<_>(...)
display(true);
```

## Value Binding

Values are bound to names using `=`. The name is added to the current context's scope:

```
PackedNumbers = Pack_Int2(100, 200);
ANumber, BNumber = Unpack_Int2(PackedNumbers);
AString = "String";
AValue = 1 + ANumber;
ManyStrings = MultiplyString(AString, AValue);
```

### Type Annotation

Annotations are optional but provide validation and documentation:

```
PackedNumbers: int2 = Pack_Int2(100, 200);
ANumber: int, BNumber: int = Unpack_Int2(PackedNumbers);
AString: string = "String";
```

## Context Expression

Combine multiple expressions using `{ }` with semicolons:

```
module Context

out this: string
out A: string
out B: string

where {
    A = "A";
    B = "B";
    ConcatenateString(A, B);
} // Returns { this="AB"; A="A"; B="B" }
```

The final expression becomes the `this` value of the context.

## Switch

Switch expressions manage chaining and branching impulse control flows:

```
switch If(Condition=true)
| OnTrue  |> ImpulseDisplay
| OnFalse |> ImpulseDisplay;

switch For(Count=100)
| LoopStart |> ImpulseDisplay
| LoopEnd   |> ImpulseDisplay
| LoopIteration ForNode |>
    switch (SomeVariable <- ForNode.Iteration)
    | OnWritten |> ImpulseDisplay
    | OnFail    |> ImpulseDisplay;
```

The pattern must be a parameter name of the module. The optional node after the pattern binds the expression's result for use in the continuation.

## List

Multiple values grouped together using `[ ]`:

```
List1: int[] = [1, 2, 3];
One: int = List1[0];
```

Lists are fixed length and known at compile time. Indexing must use non-negative integer literals.

For modules returning lists, specify size with `.Count=`:

```
ImpulseDemultiplexer(Operations.Count=5)
```

## Undefined

`undefined` is a placeholder expression that can be used anywhere. The compiler will warn about undefined values. Useful during development but should not remain in complete programs.

## Operators

Operators are shorthand for different modules.

### Pipe

`->` is a forward composition operator. Takes value on left and module on right, applying value as first positional argument:

```
Uri1 =
    LocalUser
    ->UserRootSlot
    ->GetSlotName
    ->TrimString
    ->ReplaceFirstSubstring(SearchFor=".", ReplaceWith="/")
    ->ConcatenateString("/Data")
    ->StringToAbsoluteURI;
```

### Write

`<-` updates a variable to a new value. This is an impulse node:

```
store MyVar: int;
SomeValue = 25;

switch OnStart
| Trigger |> MyVar <- SomeValue;
```

### Arithmetic

`+`, `-`, `*`, `/`, `mod`, etc. work with standard order of operations. `-` can also be a prefix operator for negation:

```
NumberCalculation = 10 / 2 + 5 * 9 + 1 - 2

M1: float3 = pack(1.0, 0.0, 1.0);
M2: float3 = pack(1.9, -2.9, 0.1);
MM: float3x3 = PackRows_Float3x3(M1, M2, M1);
M3: float3 = MM * M2 - M1 + 2.0 / M2;
```

### Comparison

`==`, `!=`, `>`, `<`, `<=`, and `>=` are binary infix comparison operators.

### Boolean

`and`, `or`, `xor`, `xnor`, `nor`, and `nand` are binary boolean operations. `not` is a unary prefix operator. They can also be used as bitwise operators.

### Other

- If/Ternary: `if <condition> then <value_on_true> else <value_on_false>`
- Null coalesce: `<possibly_null> ?? <fallback_value>`
