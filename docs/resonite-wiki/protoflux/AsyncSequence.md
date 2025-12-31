# ProtoFlux:AsyncSequence

> Source: https://wiki.resonite.com/ProtoFlux:AsyncSequence

Async Sequence

\*

Calls

+

-

Async

The **Async Sequence** performs each of the provided [async impulses](https://wiki.resonite.com/Async_impulses "Async impulses") in order, waiting for the chain of each impulse to finish before executing the next one.

This can be useful for organizational purposes or to avoid code duplication if something needs to be performed after a bunch of branching paths.

## Inputs

### \\* ( [AsyncCall](https://wiki.resonite.com/Impulses\#ASync "Impulses"))

Start execution of the node.

## Outputs

### Calls (List of [AsyncCalls](https://wiki.resonite.com/Impulses\#ASync "Impulses"))

The list of impulses to fire in order. The impulses are run in [async flow](https://wiki.resonite.com/Async_flow "Async flow"), and after the context of the impulse finishes, the next impulse is fired.

## Examples

## See Also

- [ProtoFlux:Sequence](https://wiki.resonite.com/ProtoFlux:Sequence "ProtoFlux:Sequence") for the synchronous analogue.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:AsyncSequence&oldid=109293](https://wiki.resonite.com/index.php?title=ProtoFlux:AsyncSequence&oldid=109293)"

Contents