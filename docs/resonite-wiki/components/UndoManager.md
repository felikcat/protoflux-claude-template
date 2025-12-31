# Component:UndoManager

> Source: https://wiki.resonite.com/Component:UndoManager

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/db/UndoManagerComponent.png/510px-UndoManagerComponent.png)](https://wiki.resonite.com/File:UndoManagerComponent.png) **Undo Manager** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UndoManager** component keeps track of all [user's](https://wiki.resonite.com/User "User") actions in the world, allowing users to [Undo](https://wiki.resonite.com/Undo "Undo") or revert back to a previous step or action. Undoing can be controlled in [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") within the [Undo Category](https://wiki.resonite.com/Category:ProtoFlux:Undo "Category:ProtoFlux:Undo"), where users create undo batches and steps that this component can utilize. Undoing can be disabled by setting max steps to `0`.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `MaxUndoSteps` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The maximum memory for Undoable actions per user for the current world. |
| `UnsavedChanges` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user has done anything that makes an undo step, which tells the world it has unsaved changes. |

Fields
Collapse

## See Also

[Undo](https://wiki.resonite.com/Undo "Undo")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UndoManager&oldid=96795](https://wiki.resonite.com/index.php?title=Component:UndoManager&oldid=96795)"

Contents