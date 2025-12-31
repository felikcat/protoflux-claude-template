# ProtoFlux:PackProtoFluxInPlace

> Source: https://wiki.resonite.com/ProtoFlux:PackProtoFluxInPlace

Pack Proto Flux In Place

\*

Next

StartNode

Nodes

The `Pack ProtoFlux In Place` node takes in a start point for your [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") code, and when called, will pack everything in place, no matter where. If you have all your code sitting in [Root](https://wiki.resonite.com/Root "Root") or inside a [Slot](https://wiki.resonite.com/Slot "Slot"), it will pack it at that exact location.

If you decide to add more nodes and connect them to a node that is under a different slot, the connected nodes will pack correctly and be under the `StartNode`'s slot. However, unpacking from that slot that is holding the `StartNode` may not completely unpack properly.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

It is preferred to use the [Pack ProtoFlux Nodes](https://wiki.resonite.com/ProtoFlux:Pack_ProtoFlux_Nodes "ProtoFlux:Pack ProtoFlux Nodes") node instead for packing to reduce the risk of some of your nodes not being completely packed/unpacked.


## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Calls an impulse to pack the ProtoFlux in its exact spot.

### StartNode ( [ProtoFluxNode](https://wiki.resonite.com/Type:ProtoFluxNode "Type:ProtoFluxNode"))

The starting point node where we should pack the nodes from.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Continues the code from here.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:PackProtoFluxInPlace&oldid=110425](https://wiki.resonite.com/index.php?title=ProtoFlux:PackProtoFluxInPlace&oldid=110425)"

Contents