# ProtoFlux:CreateSpawnUndoStep

> Source: https://wiki.resonite.com/ProtoFlux:CreateSpawnUndoStep

Create Spawn Undo Step

\*

Next

Target

Description

Undo

The **Create Spawn Undo Step** will create an [undo](https://wiki.resonite.com/Undo "Undo") step in the [Context Menu](https://wiki.resonite.com/Context_Menu "Context Menu") of the person who the [impulse](https://wiki.resonite.com/Impulses "Impulses") came from. This node will make the description of the undo step in the context menu the provided Description ( [String](https://wiki.resonite.com/Type:String "Type:String")). This does the best when paired with a [Duplicate Slot](https://wiki.resonite.com/ProtoFlux:Duplicate_Slot "ProtoFlux:Duplicate Slot"), since the slot is being spawned this node will allow the [duplicate](https://wiki.resonite.com/Slot "Slot") to be undo-able by the user.

when this node is paired with an [Undo Batch](https://wiki.resonite.com/ProtoFlux:Begin_Undo_Batch "ProtoFlux:Begin Undo Batch"), it's description if has one, will be ignored, and will be part of the [Undo Batch](https://wiki.resonite.com/ProtoFlux:Begin_Undo_Batch "ProtoFlux:Begin Undo Batch")'s undo step instead.

## Inputs

### Input ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Create the undo step and set the object to be despawned upon undoing to the slot provided.

### Description ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The description for the undo step in the user's context menu. Gets overridden if this node is part of a [Undo Batch](https://wiki.resonite.com/ProtoFlux:Begin_Undo_Batch "ProtoFlux:Begin Undo Batch").

### Target ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The [Slot](https://wiki.resonite.com/Slot "Slot") to undo for this undo step.

## Outputs

### Output ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Continues to More undo steps, continues to code that eventually ends, or an [End Undo Batch](https://wiki.resonite.com/ProtoFlux:End_Undo_Batch "ProtoFlux:End Undo Batch") that continues to eventually ended code.

## Examples

- [This node being used in a set of nodes that undoes a bunch of actions that was done by a previous button](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ProtoFlux_example_undo_node_settup "File:ProtoFlux example undo node settup")

This node being used in a set of nodes that undoes a bunch of actions that was done by a previous button


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:CreateSpawnUndoStep&oldid=109587](https://wiki.resonite.com/index.php?title=ProtoFlux:CreateSpawnUndoStep&oldid=109587)"

Contents