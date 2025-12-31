# ProtoFlux:CreateReferenceUndoStep

> Source: https://wiki.resonite.com/ProtoFlux:CreateReferenceUndoStep

Create Reference Undo Step

\*

Next

Target

ForceNew

Undo

The **Create Reference Undo Step** will create an [undo](https://wiki.resonite.com/Undo "Undo") step in the [Context Menu](https://wiki.resonite.com/Context_Menu "Context Menu") of the person who the [impulse](https://wiki.resonite.com/Impulses "Impulses") came from. The node will then send to the [UndoManager](https://wiki.resonite.com/Component:UndoManager "Component:UndoManager") component in the [world](https://wiki.resonite.com/World "World") the value that the reference field provided into Target should revert to. Or in more simpler terms, the current reference the provided Target ( [ISyncRef](https://wiki.resonite.com/index.php?title=Type:ISyncRef%601&action=edit&redlink=1 "Type:ISyncRef`1 (page does not exist)")) contains is what it will be reset to when undone via the context menu.

when this node is paired with an [Undo Batch](https://wiki.resonite.com/ProtoFlux:Begin_Undo_Batch "ProtoFlux:Begin Undo Batch"), it's description if has one, will be ignored, and will be part of the [Undo Batch](https://wiki.resonite.com/ProtoFlux:Begin_Undo_Batch "ProtoFlux:Begin Undo Batch")'s undo step instead.

## Inputs

### Input ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Create the undo step and set the revert to value to the current value in the provided Target ( [ISyncRef](https://wiki.resonite.com/index.php?title=Type:ISyncRef%601&action=edit&redlink=1 "Type:ISyncRef`1 (page does not exist)"))

### ForceNew ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

_This article or section is a stub. You can help the Resonite wiki by expanding it._

### Target ( [ISyncRef](https://wiki.resonite.com/index.php?title=Type:ISyncRef%601&action=edit&redlink=1 "Type:ISyncRef`1 (page does not exist)"))

The [ISyncRef](https://wiki.resonite.com/index.php?title=Type:ISyncRef%601&action=edit&redlink=1 "Type:ISyncRef`1 (page does not exist)") to undo for this undo step.

## Outputs

### Output ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Continues to More undo steps, continues to code that eventually ends, or an [End Undo Batch](https://wiki.resonite.com/ProtoFlux:End_Undo_Batch "ProtoFlux:End Undo Batch") that continues to eventually ended code.

## Examples

- [This node being used in a set of nodes that undoes a bunch of actions that was done by a previous button](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ProtoFlux_example_undo_node_settup "File:ProtoFlux example undo node settup")

This node being used in a set of nodes that undoes a bunch of actions that was done by a previous button


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:CreateReferenceUndoStep&oldid=109585](https://wiki.resonite.com/index.php?title=ProtoFlux:CreateReferenceUndoStep&oldid=109585)"

Contents