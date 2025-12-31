# ProtoFlux:ImpulseMultiplexer

> Source: https://wiki.resonite.com/ProtoFlux:ImpulseMultiplexer

Impulse Multiplexer

\*

Impulses

Index

+

-

Flow

An impulse multiplexer is a ProtoFlux node that takes a \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) and an Index ( [int](https://wiki.resonite.com/Type:Int "Type:Int")) and outputs the impulse to a Impulses ( [Continuation](https://wiki.resonite.com/Impulses "Impulses")) output with the provided index.
This node could commonly be called a switch, switchboard, router, or an impulse array.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Tell this node to send an impulse out an Impulses ( [Continuation](https://wiki.resonite.com/Impulses "Impulses")) output with the provided Index ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

### Index ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

Index of the Impulses ( [Continuation](https://wiki.resonite.com/Impulses "Impulses")) output to send an impulse out of.

## Outputs

### Impulses ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Sends an impulse out of one of these with the index provided by Index ( [int](https://wiki.resonite.com/Type:Int "Type:Int")) when \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) is called

## Examples

- [An Impulse Multiplexer being used with an Impulse Demultiplexer to run a common code for many different paths before splitting off into multiple again.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ProtoFlux_example_Impulse_Multiplexer.webp "File:ProtoFlux example Impulse Multiplexer.webp")

An Impulse Multiplexer being used with an [Impulse Demultiplexer](https://wiki.resonite.com/ProtoFlux:Impulse_Demultiplexer "ProtoFlux:Impulse Demultiplexer") to run a common code for many different paths before splitting off into multiple again.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ImpulseMultiplexer&oldid=110007](https://wiki.resonite.com/index.php?title=ProtoFlux:ImpulseMultiplexer&oldid=110007)"

Contents