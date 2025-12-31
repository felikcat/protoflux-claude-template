# ProtoFlux:PackProtoFluxFromNode

> Source: https://wiki.resonite.com/ProtoFlux:PackProtoFluxFromNode

Pack Proto Flux From Node

\*

Next

StartNode

Target

Nodes

The `Pack ProtoFlux From Node` node takes in a start point for your [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") code and a target slot to place your code in, and when called, will pack everything in place into that provided slot.

If you decide to add more nodes and connect them to a node that is under a different slot, the connected nodes will pack correctly and be under the new slot. However, unpacking from the new slot may not completely unpack properly.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

It is preferred to use the [Pack ProtoFlux Nodes](https://wiki.resonite.com/ProtoFlux:Pack_ProtoFlux_Nodes "ProtoFlux:Pack ProtoFlux Nodes") node instead for packing to reduce the risk of some of your nodes not being completely packed/unpacked.


## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Calls an impulse to pack our selected nodes.

### StartNode ( [ProtoFluxNode](https://wiki.resonite.com/Type:ProtoFluxNode "Type:ProtoFluxNode"))

The starting point node where we should pack the nodes from.

### Target ( [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot"))

The target slot we want to pack to.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Continues the code from here.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:PackProtoFluxFromNode&oldid=110423](https://wiki.resonite.com/index.php?title=ProtoFlux:PackProtoFluxFromNode&oldid=110423)"

Contents