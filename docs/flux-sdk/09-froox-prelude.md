<!--
Source: https://flux-sdk.samsmucny.com/ProtoGraph/Froox-Prelude.html
License: CC BY-NC-SA 4.0
Author: Sam (Papaltine) Smucny
-->

# Froox Prelude

By default, the modules in the `Froox` package are exposed in the default scope. You can use them without adding them to a `use` in the header.

## Export Froox Docs

To see what modules are in the Froox package, run:

```
flux-sdk froox-docs
```

This will output a YAML file listing all known modules accessible within ProtoGraph and information on the inputs/outputs of each module.

You can specify an output file:

```
flux-sdk froox-docs --out protoflux-nodes.yaml
```

## Common Froox Modules

### Math Operations

- `ValueAdd<T>`, `ValueSub<T>`, `ValueMul<T>`, `ValueDiv<T>`
- `ValueInc<T>`, `ValueDec<T>`
- `Avg`, `Ceil`, `CeilToInt`, `Floor`, `FloorToInt`
- `Cos`, `Sin`, `Tan`, `Acos`, `Asin`, `Atan`, `Atan2`
- `Pow`, `Sqrt`, `Abs`, `Min`, `Max`, `Clamp`
- `Lerp`, `InverseLerp`, `SmoothStep`
- `Log10_Float`, `Log_Float`

### Color Operations

- `ColorAddAlpha`, `ColorSetHue`, `ColorSetSaturation`
- `ColorFromHexCode`, `ColorToHSV`, `ColorFromHSV`
- `ColorLerp`, `ColorToHexString`

### String Operations

- `ConcatenateString`, `Capitalize`, `ToLower`, `ToUpper`
- `Contains`, `StartsWith`, `EndsWith`
- `CompareStrings`, `CountOccurrences`
- `Substring`, `Replace`, `Split`, `Join`, `Format`
- `TrimString`, `IndexOfString`, `ReplaceFirstSubstring`
- `MultiplyString`

### Packing/Unpacking

- `Pack_Int2`, `Pack_Int3`, `Pack_Int4`
- `Pack_Float2`, `Pack_Float3`, `Pack_Float4`
- `Unpack_Int2`, `Unpack_Int3`, `Unpack_Int4`
- `Unpack_Float2`, `Unpack_Float3`, `Unpack_Float4`
- `PackRows_Float3x3`

### Flow Control

- `If` (with OnTrue/OnFalse)
- `For`, `While`
- `AsyncFor`, `AsyncWhile`, `AsyncSequence`
- `RangeForLoopInt`, `RangeForLoopIntAsync`
- `Delay`, `DelaySecondsInt`
- `LocalImpulseTimeoutSeconds`

### Variables

- `ValueWrite<T>` / `ObjectWrite<T>`
- `WriteValueToGlobal`, `WriteObjectToGlobal`

### User/Session

- `LocalUser`, `HostUser`
- `UserRootSlot`, `GetSlotName`
- `ActiveUserRootUser`, `AllocatingUser`, `AnchoredUser`
- `SessionUser`, `SessionSlot`
- `UserFromID`, `UserToID`

### Events

- `OnActivated`, `OnDeactivated`, `OnDestroy`
- `OnLoaded`, `OnStart`
- `SecondsTimer` (with OnUpdate)
- `ButtonEvents` (with Pressed)
- `CallInput`

### Networking

- `GET_String`, `POST_String` (with OnResponse, OnError)
- WebSocket operations

### Display

- `ValueDisplay<T>`, `ObjectDisplay<T>`
- `display` (alias for appropriate display node)
- `DebugText`
- `ImpulseDisplay`

### Dynamic Variables/Impulses

- `~input<T>`, `~read<T>`, `~write<T>`
- `~trigger`, `~trigger<T>`
- `~receive`, `~receive<T>`
- `~triggerAsync`, `~triggerAsync<T>`
- `~receiveAsync`, `~receiveAsync<T>`
- `DynamicImpulseTrigger`, `DynamicImpulseReceiver`

### Type Operations

- `as<T>` (casting)
- `asDrivenGlobal`
- `null<T>`
- `NotNull`

### Comparison

- `ValueEquals<T>`, `NotEquals`
- `GreaterThan`, `LessThan`
- `GreaterOrEqual`, `LessOrEqual`

### Logic

- `And`, `Or`, `Not`
- `Xor`, `Xnor`, `Nor`, `Nand`
