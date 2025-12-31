# ProtoFlux:BeginUndoBatch

> Source: https://wiki.resonite.com/ProtoFlux:BeginUndoBatch

Begin Undo Batch

\*

Next

Description

Undo

A **Begin Undo Batch** is used to batch together every [undo](https://wiki.resonite.com/Undo "Undo") step called after it, like [Create Spawn Undo Step](https://wiki.resonite.com/ProtoFlux:Create_Spawn_Undo_Step "ProtoFlux:Create Spawn Undo Step"), [Create Field Undo Step](https://wiki.resonite.com/ProtoFlux:Create_Field_Undo_Step "ProtoFlux:Create Field Undo Step"), and [Create Undo Reference Step](https://wiki.resonite.com/ProtoFlux:Create_Reference_Undo_Step "ProtoFlux:Create Reference Undo Step") to name a few from the [ProtoFlux Undoable Category](https://wiki.resonite.com/Category:ProtoFlux:Undo "Category:ProtoFlux:Undo").

The node will create an undo step in the context menu of the person who the impulse came from.

This node needs to be ended with a [End Undo Batch](https://wiki.resonite.com/ProtoFlux:End_Undo_Batch "ProtoFlux:End Undo Batch"), to batch together every undo step call after this node and before the end undo batch node.

The undo step descriptions between these nodes will be ignored.

## Inputs

### Input ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Start the undo batch.

### Description ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The description for this undo batch. The description will be automatically prepended with "Undo" in bigger text in the context menu.

## Outputs

### Output ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

The undo steps to batch with this undo batch followed by an [End Undo Batch](https://wiki.resonite.com/ProtoFlux:End_Undo_Batch "ProtoFlux:End Undo Batch").

## Examples

- [This node being used in a set of nodes that undoes a bunch of actions that was done by a previous button](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ProtoFlux_example_undo_node_settup "File:ProtoFlux example undo node settup")

This node being used in a set of nodes that undoes a bunch of actions that was done by a previous button


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:BeginUndoBatch&oldid=109317](https://wiki.resonite.com/index.php?title=ProtoFlux:BeginUndoBatch&oldid=109317)"

Contents