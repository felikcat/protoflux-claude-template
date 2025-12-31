# ProtoFlux:SetLocalPosition

> Source: https://wiki.resonite.com/ProtoFlux:SetLocalPosition

Set Local Position

\*

Next

Instance

Position

~Transform

The **Set Local Position** node sets the input slot's position to the provided position vector in [local coordinate space](https://wiki.resonite.com/Coordinate_spaces#Global_vs._Local "Coordinate spaces").

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Sets the Instance slot's local position when an impulse is received.

### Instance ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot whose local position is set. Default is null, the node does not function without this input.

### Position ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The local position the input Instance slot is set to. Default is \[0;0;0\].

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

An impulse is fired whenever the Instance slot's position is set after the node receives an impulse. No impulse is fired from this output if the Instance input is null.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:SetLocalPosition&oldid=110701](https://wiki.resonite.com/index.php?title=ProtoFlux:SetLocalPosition&oldid=110701)"

Contents