# ProtoFlux:BodyNodeSlot

> Source: https://wiki.resonite.com/ProtoFlux:BodyNodeSlot

Body Node Slot

Source

\*

Node

Body Nodes

Body Node Slot is a ProtoFlux node that takes a user and reads their currently worn avatar's [Biped Rig Component](https://wiki.resonite.com/Component:BipedRig "Component:BipedRig") For the slot that matches the provided Node ( [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode")).

In simpler terms, it will return their upper left arm slot if given a BodyNode with the value "LeftUpperArm" and they are a humanoid.

## Inputs

### Source ( [User](https://wiki.resonite.com/Type:User "Type:User"))

The user to find a body part slot for.

### Node ( [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"))

The body node to find a slot for on Source ( [User](https://wiki.resonite.com/Type:User "Type:User")).

## Outputs

### \\* ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot on the Source ( [User](https://wiki.resonite.com/Type:User "Type:User")) that is mapped to Node ( [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode")) in the [Biped Rig Component](https://wiki.resonite.com/Component:BipedRig "Component:BipedRig").

## Examples

- [Example of the Body Node Slot node being used in an item attacher system.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Body_Node_Slot.webp "File:Protoflux example Body Node Slot.webp")

Example of the Body Node Slot node being used in an item attacher system.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:BodyNodeSlot&oldid=109327](https://wiki.resonite.com/index.php?title=ProtoFlux:BodyNodeSlot&oldid=109327)"

Contents