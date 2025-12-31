# ProtoFlux:ElapsedTime

> Source: https://wiki.resonite.com/ProtoFlux:ElapsedTime

Elapsed Time

Reset

OnReset

\*

Time

The `Elapsed Time` node keeps track of how long it has been since the last time it was called. This node starts automatically, and when it is not called, it just uses the world time as the default result. Spawning multiple nodes will show that they keep track of their own individual value.

Nodes loaded from a save continue their output from the value they had when they were saved. (A [SyncTime](https://wiki.resonite.com/Type:SyncTime "Type:SyncTime") is used internally to track how much time has passed.)

## Inputs

### Reset ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Calls an impulse to reset the elapsed time.

## Outputs

### OnReset ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires after this node has reset their elapsed time value.

### \\* (Pseudo-generic)

Returns the amount of time it has been since this node has been called.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ElapsedTime&oldid=113098](https://wiki.resonite.com/index.php?title=ProtoFlux:ElapsedTime&oldid=113098)"

Contents