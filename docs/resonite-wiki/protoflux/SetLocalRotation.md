# ProtoFlux:SetLocalRotation

> Source: https://wiki.resonite.com/ProtoFlux:SetLocalRotation

Set Local Rotation

\*

Next

Instance

Rotation

Transform

The **Set Local Rotation** node sets the input slot's rotation to the provided floatQ value in [local coordinate space](https://wiki.resonite.com/Coordinate_spaces#Global_vs._Local "Coordinate spaces").

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Sets the Instance slot's local roation when an impulse is received.

### Instance ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot whose local rotation is set. Default is null, the node does not function without this input.

### Rotation ( [floatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ"))

The local rotation the input Instance slot is set to. Default is \[0;0;0\].

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

An impulse is fired whenever the Instance slot's rotation is set after the node receives an impulse. No impulse is fired from this output if the Instance input is null.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:SetLocalRotation&oldid=110705](https://wiki.resonite.com/index.php?title=ProtoFlux:SetLocalRotation&oldid=110705)"

Contents