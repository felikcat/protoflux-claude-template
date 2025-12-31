# ProtoFlux:EndUndoBatch

> Source: https://wiki.resonite.com/ProtoFlux:EndUndoBatch

End Undo Batch

\*

Next

Undo

When paired with a [Begin Undo Batch](https://wiki.resonite.com/ProtoFlux:Begin_Undo_Batch "ProtoFlux:Begin Undo Batch"), the **End Undo Batch** node will batch all previous [undo](https://wiki.resonite.com/Undo "Undo") steps after the previous [Begin Undo Batch](https://wiki.resonite.com/ProtoFlux:Begin_Undo_Batch "ProtoFlux:Begin Undo Batch") into one, ignoring all undo descriptions on all undo nodes between the two. This will make all the undo steps one undo press on the [Context Menu](https://wiki.resonite.com/Context_Menu "Context Menu") of the user that [impulsed](https://wiki.resonite.com/Impulses "Impulses") the node chain.

## Inputs

### Input ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

End the undo batch.

## Outputs

### Output ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Code to run after the undo batch.

## Examples

- [This node being used in a set of nodes that undoes a bunch of actions that was done by a previous button](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ProtoFlux_example_undo_node_settup "File:ProtoFlux example undo node settup")

This node being used in a set of nodes that undoes a bunch of actions that was done by a previous button


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:EndUndoBatch&oldid=109721](https://wiki.resonite.com/index.php?title=ProtoFlux:EndUndoBatch&oldid=109721)"

Contents