# Component:UnresolvedReferences

> Source: https://wiki.resonite.com/Component:UnresolvedReferences

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/34/UnresolvedReferencesComponent.png/510px-UnresolvedReferencesComponent.png)](https://wiki.resonite.com/File:UnresolvedReferencesComponent.png) **Unresolved References** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UnresolvedReferences** component is internal to FrooxEngine and is found usually on a world root. It is used to store references that are unresolved by the load controller of the game for that world.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `References` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[UnresolvedReferences.UnresolvedReference](https://wiki.resonite.com/Component:UnresolvedReferences#UnresolvedReference)** | A list of references to keep a storage for. |

Fields
Collapse

## UnresolvedReference

| Name | Type | Description |
| --- | --- | --- |
| `Reference` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | A stored [RefID](https://wiki.resonite.com/Type:RefID "Type:RefID") of an unresolved reference. |

Fields

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UnresolvedReferences&oldid=106604](https://wiki.resonite.com/index.php?title=Component:UnresolvedReferences&oldid=106604)"

Contents