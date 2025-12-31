# ProtoFlux:SetLocalPositionRotation

> Source: https://wiki.resonite.com/ProtoFlux:SetLocalPositionRotation

Set Local Position Rotation

\*

Next

Instance

Position

Rotation

Transform

The **Set Local Position Rotation** node sets the input slot's position and rotation to the provided values in [local coordinate space](https://wiki.resonite.com/Coordinate_spaces#Global_vs._Local "Coordinate spaces").

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Sets the Instance slot's local position and rotation when an impulse is received.

### Instance ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot whose local position and rotation are set. Default is null, the node does not function without this input.

### Position ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The local position the input Instance slot is set to. Default is \[0;0;0\].

### Rotation ( [floatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ"))

The local rotation the input Instance slot is set to. Default is \[0;0;0\].

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

An impulse is fired whenever the Instance slot's position and rotation are set after the node receives an impulse. No impulse is fired from this output if the Instance input is null.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:SetLocalPositionRotation&oldid=110703](https://wiki.resonite.com/index.php?title=ProtoFlux:SetLocalPositionRotation&oldid=110703)"

Contents