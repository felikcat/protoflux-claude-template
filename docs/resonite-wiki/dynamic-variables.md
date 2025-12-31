# Dynamic Variables

> Source: https://wiki.resonite.com/Dynamic_variables

**Dynamic variables** (dyn vars/dynvars) is a system of data storage for scoped data under slot hierarchies with arbitrary names, similar to an associative array.

## Overview

Dynamic variables are managed with two parts:
1. **Dynamic variable spaces** - Define the scope
2. **Dynamic variables** - Store the actual data

### Variable Spaces

Add a `DynamicVariableSpace` component to a slot to make it and all children part of that named space.

- A slot can be part of multiple spaces
- Spaces under child slots are NOT nested
- Use unique names for variable spaces

### Dynamic Variable Components

| Component | Use For |
|-----------|---------|
| `DynamicValueVariable` | Value types (int, string, float3, etc.) |
| `DynamicReferenceVariable` | Reference types (Slot, User, etc.) |
| `DynamicTypeVariable` | Type type |

### Dynamic Fields

Transform existing IField into dynamic variable:

| Component | Use For |
|-----------|---------|
| `DynamicField` | Value types |
| `DynamicReference` | Reference types |
| `DynamicTypeField` | Type type |

### Naming Restrictions

Names must NOT contain symbols, punctuation, or whitespace EXCEPT:
- Period (`.`)
- Underscore (`_`)
- Space (` `)
- Hyphen (`-`)

## Binding

### Direct vs Indirect Binding

| Format | Type | Behavior |
|--------|------|----------|
| `VariableName` | Indirect | Binds to first space without `OnlyDirectBinding` |
| `SpaceName/VariableName` | Direct | Binds to first space matching `SpaceName` |

### Example
```
└─ Foo - Variable Space "test"
   └─ Bar - Variable Space "test2"
      └─ Baz - Dynamic Variable "test/var"
```
- `test/var` binds to space `test`
- `var` would bind to space `test2`
- `var` with `test2` having `OnlyDirectBinding` would bind to `test`

### Binding Delay Warning

Some operations require `Delay Updates` of 2+ updates:
- Creating new dynamic reference variables
- Deleting dynamic variables
- Changing variable/space names
- Duplicating slots with dynamic variable space
- Reparenting slots under new variable space

## Reading Dynamic Variables

### ProtoFlux Nodes

| Node | Use Case |
|------|----------|
| `Read Dynamic Variable` | Read from outside the node's hierarchy |
| `Dynamic Variable Input` | Read constant-name variables within same space |

### Driving from Dynamic Variables

Use `DynamicValueVariableDriver` or `DynamicReferenceVariableDriver` to drive fields from dynamic variable values.

## Writing Dynamic Variables

Use these ProtoFlux nodes:
- `Write Dynamic Variable` - Write to existing variables
- `Write Or Create Dynamic Variable` - Create if doesn't exist

### Writing/Driving Delay Warning

If writing via component field sourcing, there's a 1 frame delay before propagation. Always use proper ProtoFlux nodes instead.

## Default Spaces

| Space | Location | Notes |
|-------|----------|-------|
| `World` | Under Root of any world | `OnlyDirectBinding` enabled |
| `User` | Under each User's User Root Slot | `OnlyDirectBinding` enabled |
| `Dash` | Under UserspaceRadiantDash in userspace | - |

## Best Practices

1. Have only one instance of each dynamic variable at a time
2. Use direct binding (`SpaceName/VarName`) for clarity
3. Use periods (`.`) to pseudo-isolate objects in complex systems
   - Example: `User/Avatar.Systems.Flight.Drag`

## ProtoFlux Syntax (ProtoGraph)

```protograph
// Read dynamic variable
HueRead = UISlot->~read<float>("ColorPicker/H");
Value = HueRead.Value;
Found = HueRead.FoundValue;

// Write dynamic variable (impulse node)
switch TargetSlot->~write("VariablePath", Value=MyValue)
| OnSuccess  |> impulse { }
| OnFailed   |> impulse { }
| OnNotFound |> impulse { };

// Source dynamic variable input
SourceDynVar = ~input<bool>("VariableName");
```
