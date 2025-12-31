# Component:SavedReferenceTable

> Source: https://wiki.resonite.com/Component:SavedReferenceTable

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/7b/SavedReferenceTableComponent.png/510px-SavedReferenceTableComponent.png)](https://wiki.resonite.com/File:SavedReferenceTableComponent.png) **Saved Reference Table** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Used solely by [Component:SpawnOrDestroy](https://wiki.resonite.com/Component:SpawnOrDestroy "Component:SpawnOrDestroy") to store the data of a destroyed object to restore later.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Table` | _direct_ **[SyncRefDictionary\`2](https://wiki.resonite.com/index.php?title=Type:SyncRefDictionary%602&action=edit&redlink=1 "Type:SyncRefDictionary`2 (page does not exist)") < [String](https://wiki.resonite.com/Type:String "Type:String"), [IWorldElement](https://wiki.resonite.com/Type:IWorldElement "Type:IWorldElement") >** | The table to save destroyed object data. |

Fields
Collapse

## See Also

- [Component:SpawnOrDestroy](https://wiki.resonite.com/Component:SpawnOrDestroy "Component:SpawnOrDestroy")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SavedReferenceTable&oldid=106544](https://wiki.resonite.com/index.php?title=Component:SavedReferenceTable&oldid=106544)"

Contents