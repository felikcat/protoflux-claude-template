# Local Documentation

This directory contains local copies of official documentation for Flux SDK and ProtoGraph development.

## Flux SDK Documentation

Complete ProtoGraph language reference stored in `flux-sdk/`:

| File | Topic |
|------|-------|
| [01-introduction.md](flux-sdk/01-introduction.md) | Overview of ProtoGraph and its goals |
| [02-getting-started.md](flux-sdk/02-getting-started.md) | Installation, setup, and first program |
| [03-basic-syntax.md](flux-sdk/03-basic-syntax.md) | File structure, comments, keywords, grouping |
| [04-types-and-variables.md](flux-sdk/04-types-and-variables.md) | Type system, literals, variables (sync/store/local) |
| [05-expressions-and-operators.md](flux-sdk/05-expressions-and-operators.md) | Expressions, records, operators, bindings |
| [06-impulse-control-flow.md](flux-sdk/06-impulse-control-flow.md) | Impulses, froox vs impulse context, async |
| [07-dynamics.md](flux-sdk/07-dynamics.md) | Dynamic variables and impulses (~read, ~write, ~trigger) |
| [08-modules-and-packages.md](flux-sdk/08-modules-and-packages.md) | Module I/O, packages, dependencies |
| [09-froox-prelude.md](flux-sdk/09-froox-prelude.md) | Available nodes and modules |

## Source Attribution

Documentation sourced from [Flux SDK](https://flux-sdk.samsmucny.com/) by Sam (Papaltine) Smucny.

Licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/).

## Quick Reference

### Module Structure
```
module ModuleName

in  InputName: type
in  SlotInput: Slot element
in  ButtonInput: IButton global

out OutputName: type
out this: type

use OtherModule

where {
    // Body expressions
}
```

### Variable Types
- `sync` - Synchronized with all users (network traffic)
- `store` - Persistent, local only
- `local` - Ephemeral, per impulse chain

### Key Operators
- `->` Pipe (forward composition)
- `<-` Write (assignment to variable)
- `|>` Branch (impulse routing in switch)
- `.` Field accessor

### Control Flow
```
// Switch expression
switch If(Condition=expr)
| OnTrue  |> impulse { ... }
| OnFalse |> impulse { ... };

// Impulse context with bind
impulse {
    bind Result = SomeAsyncNode().OnResponse;
    Variable <- Result.Value;
};

// Syntax sugar
if Condition then impulse { ... } else impulse { ... };
for i = 0 to 10 do impulse { ... };
while Condition do impulse { ... };
```

### Dynamic Operations
```
// Dynamic variables
~input<T>("VariableName")
Slot->~read<T>("Tag")
Slot->~write("Path", Value=value)

// Dynamic impulses
Slot->~trigger("Tag")
Slot->~trigger<T>("Tag", data)
switch ~receive<T>("Tag") | OnTriggered R |> impulse { ... };
```
