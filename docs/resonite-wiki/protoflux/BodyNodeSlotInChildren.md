# ProtoFlux:BodyNodeSlotInChildren

> Source: https://wiki.resonite.com/ProtoFlux:BodyNodeSlotInChildren

Body Node Slot In Children

Source

\*

Node

Body Nodes

Body Node Slot In Children is a ProtoFlux node that checks the parent slots of Source ( [Slot](https://wiki.resonite.com/Slot "Slot")) for a [Biped Rig](https://wiki.resonite.com/Component:BipedRig "Component:BipedRig") component, and then reads the BipedRig component for the provided Node ( [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode")). If the node's mapped slot is a child of Source ( [Slot](https://wiki.resonite.com/Slot "Slot")) it returns that mapped slot.

## Inputs

### Source ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot to check all of it's children infinitely far down for the provided Node ( [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode")).

### Node ( [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"))

The node to check Source ( [Slot](https://wiki.resonite.com/Slot "Slot"))'s children for.

## Outputs

### \\* ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot under the provided Source ( [Slot](https://wiki.resonite.com/Slot "Slot")) that has an assignment to the provided Node ( [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode")).

## Examples

- [Example of the Body Node Slot In Children node being used in an item attacher system.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Body_Node_Slot_In_Children.webp "File:Protoflux example Body Node Slot In Children.webp")

Example of the Body Node Slot In Children node being used in an item attacher system.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:BodyNodeSlotInChildren&oldid=109329](https://wiki.resonite.com/index.php?title=ProtoFlux:BodyNodeSlotInChildren&oldid=109329)"

Contents