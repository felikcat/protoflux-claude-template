# ProtoFlux:Sequence

> Source: https://wiki.resonite.com/ProtoFlux:Sequence

Sequence

\*

Calls

+

-

Flow

The **Sequence** node performs each of the provided [impulses](https://wiki.resonite.com/Impulses "Impulses") in order, waiting for the chain of each impulse to finish before executing the next one.

This can be useful for organizational purposes or to avoid code duplication if something needs to be performed after a bunch of branching paths.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Start execution of the node.

## Outputs

### Calls (List of [Call](https://wiki.resonite.com/Impulses "Impulses"))

The list of impulses to fire in order. This node will start at the first impulse, and after the context of the impulse finishes, the next impulse is fired. Repeats until the last impulse finishes.

## Examples

## See Also

- [ProtoFlux:Async Sequence](https://wiki.resonite.com/ProtoFlux:Async_Sequence "ProtoFlux:Async Sequence") for the asynchronous anlogue

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:Sequence&oldid=106520](https://wiki.resonite.com/index.php?title=ProtoFlux:Sequence&oldid=106520)"

Contents