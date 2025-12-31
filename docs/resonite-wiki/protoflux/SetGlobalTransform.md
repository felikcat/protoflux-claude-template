# ProtoFlux:SetGlobalTransform

> Source: https://wiki.resonite.com/ProtoFlux:SetGlobalTransform

Set Global Transform

\*

Next

Instance

Position

Rotation

Scale

Transform

The **Set Global Transform** node sets the input slot's position, rotation and scale to the provided values in [global coordinate space](https://wiki.resonite.com/Coordinate_spaces#Global_vs._Local "Coordinate spaces").

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Sets the Instance slot's global transform when an impulse is received.

### Instance ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot whose global transform is set. Default is null, the node does not function without this input.

### Position ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The global position the input Instance slot is set to. Default is \[0;0;0\].

### Rotation ( [floatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ"))

The global rotation the input Instance slot is set to. Default is \[0;0;0\].

### Scale ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The global scale the input Instance slot is set to. Default is \[1;1;1\].

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

An impulse is fired whenever the Instance slot's transform is set after the node receives an impulse. No impulse is fired from this output if the Instance input is null.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:SetGlobalTransform&oldid=110683](https://wiki.resonite.com/index.php?title=ProtoFlux:SetGlobalTransform&oldid=110683)"

Contents