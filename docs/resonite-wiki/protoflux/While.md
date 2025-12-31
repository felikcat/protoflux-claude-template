# ProtoFlux:While

> Source: https://wiki.resonite.com/ProtoFlux:While

While

\*

LoopStart

Condition

LoopIteration

LoopEnd

Flow

The **While** node is used to perform looping operations by allowing one to fire [impulses](https://wiki.resonite.com/Impulses "Impulses") continuously while a condition remains true.

![](https://wiki.resonite.com/images/b/b7/DangerIcon.svg)

Be very careful when developing with this node. [There is no iteration limit for debugging](https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/774) and [ProtoFlux does not have handling for execution taking too long](https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/1677). If you accidentally create an infinite loop, you'll be unable to save progress or anything else important. Consider adding your own iteration limit, not being connected to an input impulse while developing, and save before testing!


## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Begin the while loop.

### Condition ( [Boolean](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Condition that the loop will check to determine if it should iterate again or not. If `True`, it will iterate again.

## Outputs

### LoopStart ( [Impulse](https://wiki.resonite.com/Impulses "Impulses"))

Fires after `*` is pulsed and before any iterations are performed. Will be pulsed even if `Condition` is `False` at the time of the loop beginning.

### LoopIteration ( [Impulse](https://wiki.resonite.com/Impulses "Impulses"))

Will be pulsed for as long `Condition` is `True`. Only after the [context](https://wiki.resonite.com/Context "Context") of the current loop iteration is finished will the next iteration fire.

### LoopEnd ( [Impulse](https://wiki.resonite.com/Impulses "Impulses"))

Fires after `Condition` turns `False`, continuing the impulse chain from before.

## Known Issues

- As of the time of writing, there is [a known issue](https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/256) where if the final node in the `LoopIteration` chain is a [Write](https://wiki.resonite.com/ProtoFlux:Write "ProtoFlux:Write") node, said node modifies a variable used for conditional evaluation, _and_ the value to write is based off said variable, the write will be using a previously cached value. This can cause an extra loop iteration to occur, which is very annoying to debug.

  - The easiest way to work around this bug is to add a "dummy" node after the write, such as an [Impulse Display](https://wiki.resonite.com/ProtoFlux:Impulse_Display "ProtoFlux:Impulse Display") or, if debugging a ton of impulses and lag is undesirable, an empty Write node.

## See Also

- If it is possible to determine the amount of times you need to loop beforehand, consider [ProtoFlux:For](https://wiki.resonite.com/ProtoFlux:For "ProtoFlux:For") instead.
- [ProtoFlux:Async While](https://wiki.resonite.com/ProtoFlux:Async_While "ProtoFlux:Async While") for the [async](https://wiki.resonite.com/Async "Async") variant of this node.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:While&oldid=93265](https://wiki.resonite.com/index.php?title=ProtoFlux:While&oldid=93265)"

Contents