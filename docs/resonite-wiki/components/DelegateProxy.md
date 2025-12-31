# Component:DelegateProxy

> Source: https://wiki.resonite.com/Component:DelegateProxy

Collapse **Component image**

[File:DelegateProxy\`1Component.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=DelegateProxy%601Component.png "File:DelegateProxy`1Component.png") **Delegate Proxy\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DelegateProxy** is the Sync delegate version of a proxy used to store information about a world element in a user's hand before dropping it into a field. It's similar to grabbing a field name or a value.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Delegate` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **T** | The Sync delegate to proxy. |

Fields
Collapse

## Usage

Used in delegate grabbing, is not used by the user directly.

## Examples

The delegate item that is grabbed from inspectors when grabbing a Sync delegate description.

## See Also

- [Component:ReferenceProxy](https://wiki.resonite.com/Component:ReferenceProxy "Component:ReferenceProxy")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DelegateProxy&oldid=96434](https://wiki.resonite.com/index.php?title=Component:DelegateProxy&oldid=96434)"

Contents