# ProtoFlux:SetGlobalPosition

> Source: https://wiki.resonite.com/ProtoFlux:SetGlobalPosition

Set Global Position

\*

Next

Instance

Position

Transform

The **Set Global Position** node sets the input slot's position to the input float3 position vector in [global coordinate space](https://wiki.resonite.com/Coordinate_spaces#Global_vs._Local "Coordinate spaces").

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Sets the Instance slot's global position when an impulse is received.

### Instance ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot whose global position is set. Default is null, the node does not function without this input.

### Position ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The global position the input Instance slot is set to. Default is \[0;0;0\].

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

An impulse is fired whenever the Instance slot's position is set after the node receives an impulse. No impulse is fired from this output if the Instance input is null.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:SetGlobalPosition&oldid=110675](https://wiki.resonite.com/index.php?title=ProtoFlux:SetGlobalPosition&oldid=110675)"

Contents