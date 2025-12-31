# ProtoFlux:CallRelay

> Source: https://wiki.resonite.com/ProtoFlux:CallRelay

[A visual image of an Call Relay node by itself, connected to nothing.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ProtoFlux_visuals_Call_Relay.webp "File:ProtoFlux visuals Call Relay.webp")

_due to wiki limitations, this node does not currently have an HTML rendering of the node._

A Call Relay is a slightly different variation of the [Continuation Relay](https://wiki.resonite.com/ProtoFlux:Continuation_Relay "ProtoFlux:Continuation Relay") node, It can be found in the node browser under Core, and when connected to itself, or as the last node before recursion in a chain or loop of nodes it will not cause an exception.

![](https://wiki.resonite.com/images/b/b7/DangerIcon.svg)

Using this node to create loops without adding functionality to break the flow can and will crash your game, as resonite has no iteration limit for ProtoFlux.


This behaviour can be used to create loops within protoflux, but nodes such as [ProtoFlux:While](https://wiki.resonite.com/ProtoFlux:While "ProtoFlux:While") and [ProtoFlux:For](https://wiki.resonite.com/ProtoFlux:For "ProtoFlux:For") would be more suitable, as they come with built in ways of "ending" the loop that needs to be added for protoflux to be safe, and additional outputs for the start, continuation, and end of a loop.

## Inputs

### Input ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

The Call to send to the output

## Outputs

### Output ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

The Call continued from the Input ( [Call](https://wiki.resonite.com/Impulses "Impulses")) signal.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:CallRelay&oldid=109337](https://wiki.resonite.com/index.php?title=ProtoFlux:CallRelay&oldid=109337)"

Contents