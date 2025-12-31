<!--
Source: https://flux-sdk.samsmucny.com/ProtoGraph/Dynamics.html
License: CC BY-NC-SA 4.0
Author: Sam (Papaltine) Smucny
-->

# Dynamic Scoping

Most of ProtoGraph uses static scoping (lexical scoping). This makes structuring and building modular programs easier, but some programming patterns like implicit parameters and exception handling are naturally better expressed using dynamic scoping.

Dynamic variables and impulses are very common throughout Resonite code. ProtoGraph has a special set of unified syntax starting with `~` (tilde) to help simplify working with them.

When applicable, the first parameter to dynamic nodes is a slot (like the target or source). This allows a fluent call style that looks like calling a method on the slot.

> The order of some dynamic nodes is different from the ProtoFlux nodes they generate. Use ProtoGraph documentation and examples, not Resonite ProtoFlux documentation, for parameter order.

## Dynamic Variables

These nodes allow you to read and write to dynamic variables.

| Node | Description |
|------|-------------|
| `~input<T>` | Sources a dynamic variable value |
| `~read<T>` | Read a dynamic variable value |
| `~write<T>` | Write to a dynamic variable |

### ~input

Source a dynamic variable using a variable name. The variable name needs to be a 'global'. Literal strings are automatically converted to globals. The type argument is required.

```
SourceDynVar = ~input<bool>("VariableName");
display(SourceDynVar.Value);
display(SourceDynVar.HasValue);
```

### ~read

Read a dynamic variable off of a source slot. The type argument is required.

```
DynVar = SourceSlot->~read<int>("VariableTag");
display(DynVar.Value);
display(DynVar.HasValue);
```

### ~write

Write to a dynamic variable. The type argument can be inferred from the `Value` argument. This is an impulse node (but not a 'dynamic impulse' node).

```
switch S->~write("VariablePath", Value="Value to write...")
| OnSuccess  |> impulse {}
| OnFailed   |> impulse {}
| OnNotFound |> impulse {};
```

## Dynamic Impulses

These nodes allow you to trigger and receive dynamic impulses. Normal rules of dynamic impulses in Resonite apply: triggers and receivers must be compatible (same data type and same sync/async color) to send/catch each other's impulses.

| Node | Description |
|------|-------------|
| `~trigger` | Trigger a dynamic impulse |
| `~trigger<T>` | Trigger a dynamic impulse with data |
| `~receive` | Receive a dynamic impulse |
| `~receive<T>` | Receive a dynamic impulse with data |
| `~triggerAsync` | Async version of `~trigger` |
| `~triggerAsync<T>` | Async version of `~trigger<T>` |
| `~receiveAsync` | Async version of `~receive` |
| `~receiveAsync<T>` | Async version of `~receiveAsync<T>` |

### Triggering

```
// Send a dynamic impulse with the data payload 1.6
// The type argument can be inferred
TargetSlot->~trigger("SubRoutine1", 1.6);

// Send without data (different impulse even with same tag)
TargetSlot->~trigger("SubRoutine1");
```

### Receiving

Use a switch to catch dynamic impulses:

```
switch ~receive<float>("SubRoutine1")
| OnTriggered Receiver |>
    impulse {
        // Get the value using Receiver.Value
        Value: float = Receiver.Value;
        // Do something with Value...
    };
```

## Sync vs Async Compatibility

- `~trigger` and `~receive` are synchronous
- `~triggerAsync` and `~receiveAsync` are asynchronous
- A sync trigger cannot be caught by an async receiver (and vice versa)
- Ensure matching colors when designing dynamic impulse systems
