# ProtoFlux:AsyncFor

> Source: https://wiki.resonite.com/ProtoFlux:AsyncFor

Async For

\*

LoopStart

Count

LoopIteration

Reverse

LoopEnd

Iteration

Async

The **Async For** node is used to perform looping operations by allowing one to fire impulses a set amount of times. It is the [async](https://wiki.resonite.com/Async "Async") variant of the [For](https://wiki.resonite.com/ProtoFlux:For "ProtoFlux:For") node.

## Inputs

### \\* ( [IAsyncOperation](https://wiki.resonite.com/Impulses\#ASync "Impulses"))

Begin the for loop.

### Count ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The amount of times to trigger `LoopIteration`. Will not trigger any iterations if less than 1.

### Reverse ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

If `True`, the `Iteration` output will start at `Count - 1` and go down towards `0`.

## Outputs

### LoopStart ( [AsyncCall](https://wiki.resonite.com/Impulses\#ASync "Impulses"))

Fires after `*` is pulsed and before any iterations are done. Will be pulsed even if `Count < 1`.

### LoopIteration ( [AsyncCall](https://wiki.resonite.com/Impulses\#ASync "Impulses"))

Fires for each iteration of the loop. This impulse is triggered `Count` amount of times and the next iteration will only be fired once the current iteration's [context](https://wiki.resonite.com/Context "Context") is finished.

### LoopEnd ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires after the final `LoopIteration` completes execution.

### Iteration ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

For each `LoopIteration`, this output is set to be the index of the iteration for said iteration's context. By default, this will start at `0` and increment until `Count - 1` unless `Reverse` is `True`.

## Examples

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:AsyncFor&oldid=109289](https://wiki.resonite.com/index.php?title=ProtoFlux:AsyncFor&oldid=109289)"

Contents