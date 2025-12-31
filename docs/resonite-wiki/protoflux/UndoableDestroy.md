# ProtoFlux:UndoableDestroy

> Source: https://wiki.resonite.com/ProtoFlux:UndoableDestroy

Undoable Destroy

\*

Next

Target

Preserve Assets

Undo

The **Undoable Destroy** node will create an [undo](https://wiki.resonite.com/Undo "Undo") step in the [Context Menu](https://wiki.resonite.com/Context_Menu "Context Menu") of the [user](https://wiki.resonite.com/User "User") who the [impulse](https://wiki.resonite.com/Impulses "Impulses") came from. The destruction of the slot provided in Target ( [Slot](https://wiki.resonite.com/Slot "Slot")) will be undo-able by the user.

when this node is paired with an [Undo Batch](https://wiki.resonite.com/ProtoFlux:Begin_Undo_Batch "ProtoFlux:Begin Undo Batch"), it's description if has one, will be ignored, and will be part of the [Undo Batch](https://wiki.resonite.com/ProtoFlux:Begin_Undo_Batch "ProtoFlux:Begin Undo Batch")'s undo step instead.

## Inputs

### Input ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Create the undo step and set the Slot to be stored in the Undo Manager with references cut for later re-instantiating upon undoing the [Slot](https://wiki.resonite.com/Slot "Slot")'s destruction. (Basically make the destruction of the slot provided undoable)

### Target ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The [Slot](https://wiki.resonite.com/Slot "Slot") to undo destruction for this undo step.

### PreserveAssets ( [Boolean](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Whether to keep the assets store able in an [Asset Provider](https://wiki.resonite.com/Type:IAssetProvider%601 "Type:IAssetProvider`1") associated with this slot or discard them. Discarding them may lead to missing textures or assets.

## Outputs

### Output ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Continues to More undo steps, continues to code that eventually ends, or an [End Undo Batch](https://wiki.resonite.com/ProtoFlux:End_Undo_Batch "ProtoFlux:End Undo Batch") that continues to eventually ended code.

## Examples

- [This node being used in a set of nodes that undoes a bunch of actions that was done by a previous button](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ProtoFlux_example_undo_node_settup "File:ProtoFlux example undo node settup")

This node being used in a set of nodes that undoes a bunch of actions that was done by a previous button


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:UndoableDestroy&oldid=110917](https://wiki.resonite.com/index.php?title=ProtoFlux:UndoableDestroy&oldid=110917)"

Contents