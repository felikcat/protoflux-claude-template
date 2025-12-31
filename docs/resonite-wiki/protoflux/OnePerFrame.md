# ProtoFlux:OnePerFrame

> Source: https://wiki.resonite.com/ProtoFlux:OnePerFrame

(Redirected from [ProtoFlux:OnePerFrame](https://wiki.resonite.com/index.php?title=ProtoFlux:OnePerFrame&redirect=no "ProtoFlux:OnePerFrame"))

Once Per Frame

\*

Next

Flow

This node will restrict the amount of impulses that go through Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses")) to one impulse per game tick. This is useful if you have multiple code branches that may or may not execute at the same time, but you want to run code after all of those branches only once.

Currently, Game Ticks and Framerate are locked and bound to one another. That is until Sauce replaces Unity and the engine threads are made separate.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Tell this node to send an impulse out of Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses")). Will only send one impulse in a game tick, ignoring every subsequent request during the game tick.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Will send an impulse only once in a game tick after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) has been called during a game tick.

## Examples

- [example of a once per frame being used at the end of multiple paths to prevent the final node chain from being called excessively.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_once_per_frame.webp "File:Protoflux example once per frame.webp")

example of a once per frame being used at the end of multiple paths to prevent the final node chain from being called excessively.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:OncePerFrame&oldid=110379](https://wiki.resonite.com/index.php?title=ProtoFlux:OncePerFrame&oldid=110379)"

Contents