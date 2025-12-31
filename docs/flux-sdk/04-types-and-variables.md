<!--
Source: https://flux-sdk.samsmucny.com/ProtoGraph/Types-and-Variables.html
License: CC BY-NC-SA 4.0
Author: Sam (Papaltine) Smucny
-->

# Types and Variables

## Overview

ProtoGraph, like ProtoFlux, has a strong, static type system. Every value/node in a program has a well defined type that can be determined without running the code. ProtoGraph attempts to infer types throughout the program which reduces the need for explicit type annotations; however, type annotations for important value definitions are recommended for readability.

While ProtoGraph/ProtoFlux is strongly typed, the serialized form (.brson Resonite records) is weakly typed. When loaded into Resonite, connections are checked and invalid connections result in `null` wires.

## Annotations

Type annotations provide extra tests on behavior: the compiler will produce an error if the annotated type does not match the derived type.

Type annotations are always required for values in a module's header (inputs/outputs/globals).

```
module TypeAnnotations

in  InputInteger: int

out Times2: int
out Times3: int

where {
    // Type is inferred for Times2 to be int
    Times2 = ValueAdd(InputInteger, InputInteger);

    // Manually annotate with a type for clarity
    Times3: int =
        ValueAdd<int>(InputInteger, InputInteger)
        ->ValueAdd<int>(InputInteger);
}
```

## Literals

ProtoGraph has literal values with specific syntax to prevent type ambiguities. The compiler will not implicitly coerce literal types.

| Type | Description | Syntax | Examples |
|------|-------------|--------|----------|
| bool | true or false | keywords | `true`, `false` |
| char | A single character | single quoted | `'A'` |
| string | A string of characters | double quoted | `"My String"` |
| int | A 32 bit integer | number or `i` | `1`, `1i` |
| float | A 32 bit floating point | number with `.` or exponent or `f` | `3.14`, `1e10`, `5f` |
| double | A 64 bit floating point | `d` | `42d`, `-1.8e-8` |
| long | A 64 bit integer | `L` | `100000L` |
| uint | An unsigned 32 bit integer | `ui` | `42ui` |
| ulong | An unsigned 64 bit integer | `uL` | `99999uL` |
| short | A 16 bit integer | `s` | `500s` |
| ushort | An unsigned 16 bit integer | `us` | `500us` |
| byte | An unsigned 8 bit integer | `uy` | `91uy` |
| sbyte | A signed 8 bit integer | `y` | `1y` |
| decimal | A signed 128 bit fixed decimal | `m` | `1111m` |

## Binary, Hexadecimal, & Octal

Literal numbers can use binary, octal, and hexadecimal:

```
DecimalNumber = 1234;
BinaryNumberUnsigned = 0b110011u;
OctalNumber = 0o1662;
HexNumber = 0xab12ef;
```

By default they are interpreted as `int`. Add a suffix to change the type.

## Value & Object Types

Types are divided into value types and object types:
- **Value types**: default value is a 'zero' value (0, 0.0, false)
- **Object types**: default value is null

## Generic Types

Types parameterized with another type are called generic.

### Lists

Multiple values of the same type can be grouped into a list. The type is written with `[]` after the type name:

```
IntList: int[] = [1, 2, 3];
StringList: string[] = ["Word", "Word2"];
```

## Variables

Variables are mutable: they can be changed using the write operator (`<-`). There are 3 kinds:

### Sync

```
sync SyncronizedInteger: int;
```

Synchronized variables use the data model to automatically synchronize values with other users.

### Store

```
store StoredInteger: int;
```

Stored variables are persistent but NOT synchronized with other users.

### Local

```
local LocalInteger: int;
```

Local variables are ephemeral and scoped to an impulse context. Each impulse context has its own local, discarded when the chain ends.

## Casting

Use `as<T>` to coerce one type to another:

```
as<object>("my string");
->as<object>; // Using pipe operator

// Casting object types
ActuallySlot: object = RootSlot->as<object>;
TheSlot = ActuallySlot->as<Slot>;

// Casting value types
LargerNumbersAsObject = as<object>(100->as<long> * 100L);
```

## Globals

Types may have the `global` modifier. Normal values can be converted to globals using `asDrivenGlobal`:

```
UserValue = LocalUser;
TrueValue = true;
SecondsTimer(
    1.0,
    UpdatingUser=UserValue->asDrivenGlobal,
    SkipIfNull=asDrivenGlobal(TrueValue),
    OnUpdate=ImpulseDisplay);
```

## Null Values

The default value of object and reference types is `null`. Use the `null<T>` keyword:

```
NullString = null<string>;
NullSlot = null<Slot>;

NullString->ConcatenateString("RealString")->display; // displays null
display(NullSlot == RootSlot) // displays false
```

> All objects/references in ProtoFlux are nullable. The runtime automatically propagates default values, but logic bugs can manifest if expected values are actually null.
