# Component:SpawnOrDestroy

> Source: https://wiki.resonite.com/Component:SpawnOrDestroy

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c2/SpawnOrDestroyComponent.png/510px-SpawnOrDestroyComponent.png)](https://wiki.resonite.com/File:SpawnOrDestroyComponent.png) **Spawn Or Destroy** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SpawnOrDestroy** component is part of the [Undo](https://wiki.resonite.com/Undo "Undo") system, and handles spawning and destruction of objects in the [Undo](https://wiki.resonite.com/Undo "Undo") system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | **[Worker](https://wiki.resonite.com/index.php?title=Type:Worker&action=edit&redlink=1 "Type:Worker (page does not exist)")** | The target worker to use when executing. |
| `TargetParent` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The parent of this object to restore it to. |
| `_onRestored` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [Worker](https://wiki.resonite.com/index.php?title=Type:Worker&action=edit&redlink=1 "Type:Worker (page does not exist)") >** | The sync delegate with this compoonent's worker passed as an object to trigger when the object is restored. |
| `_mode` | **[SpawnOrDestroy.Mode](https://wiki.resonite.com/Component:SpawnOrDestroy#Mode)** | What mode to execute. |
| `_preserveAssets` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the destruction should preserve assets like meshes. |
| `_sendDestroyingEvents` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to send destruction events when destroying. |
| `_savedObject` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The URI of the saved object. |
| `_isComponent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this is in component form or internal to the engine. |
| `_referenceTable` | **[SavedReferenceTable](https://wiki.resonite.com/Component:SavedReferenceTable "Component:SavedReferenceTable")** | The place to store destroyed object data in order to restore the object later. |
| `_isSaving` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component is saving object data. |
| `_description` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The description of the object. |
| `_performed` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component is finished executing it's function. |

Fields
Collapse

## Usage

## Examples

Used to restore objects destroyed via undoable protoflux actions or context menu, or for undoing spawning of objects.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SpawnOrDestroy&oldid=106545](https://wiki.resonite.com/index.php?title=Component:SpawnOrDestroy&oldid=106545)"

Contents