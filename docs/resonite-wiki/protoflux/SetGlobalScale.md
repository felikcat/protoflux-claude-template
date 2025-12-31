# ProtoFlux:SetGlobalScale

> Source: https://wiki.resonite.com/ProtoFlux:SetGlobalScale

Set Global Scale

\*

Next

Instance

Scale

Transform

The **Set Global Scale** node sets the input slot's scale to the input value in [global coordinate space](https://wiki.resonite.com/Coordinate_spaces#Global_vs._Local "Coordinate spaces").

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Sets the Instance slot's global scale when an impulse is received.

### Instance ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot whose global scale is set. Default is null, the node does not function without this input.

### Scale ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The global scale the input Instance slot is set to. Default is \[1;1;1\].

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

An impulse is fired whenever the Instance slot's scale is set after the node receives an impulse. No impulse is fired from this output if the Instance input is null.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:SetGlobalScale&oldid=110681](https://wiki.resonite.com/index.php?title=ProtoFlux:SetGlobalScale&oldid=110681)"

Contents