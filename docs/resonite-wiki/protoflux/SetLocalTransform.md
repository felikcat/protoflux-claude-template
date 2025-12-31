# ProtoFlux:SetLocalTransform

> Source: https://wiki.resonite.com/ProtoFlux:SetLocalTransform

Set Local Transform

\*

Next

Instance

Position

Rotation

Scale

Transform

The **Set Local Transform** node sets the input slot's position, rotation and scale to the provided values in [local coordinate space](https://wiki.resonite.com/Coordinate_spaces#Global_vs._Local "Coordinate spaces").

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Sets the Instance slot's local transform when an impulse is received.

### Instance ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot whose local transform is set. Default is null, the node does not function without this input.

### Position ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The local position the input Instance slot is set to. Default is \[0;0;0\].

### Rotation ( [floatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ"))

The local rotation the input Instance slot is set to. Default is \[0;0;0\].

### Scale ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The local scale the input Instance slot is set to. Default is \[1;1;1\].

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

An impulse is fired whenever the Instance slot's transform is set after the node receives an impulse. No impulse is fired from this output if the Instance input is null.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:SetLocalTransform&oldid=110709](https://wiki.resonite.com/index.php?title=ProtoFlux:SetLocalTransform&oldid=110709)"

Contents