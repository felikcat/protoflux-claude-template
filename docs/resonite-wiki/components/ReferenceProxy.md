# Component:ReferenceProxy

> Source: https://wiki.resonite.com/Component:ReferenceProxy

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2b/ReferenceProxyComponent.png/510px-ReferenceProxyComponent.png)](https://wiki.resonite.com/File:ReferenceProxyComponent.png) **Reference Proxy** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ReferenceProxy** component is used to make a grabbed item this is on act as the reference this refers to. This is also generated when a reference in an [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector") is grabbed in the form of a block of text showing the reference and its id.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Reference` | _direct_ **[SyncRef](https://wiki.resonite.com/Type:SyncRef "Type:SyncRef")** | The reference this component should point to for grabbable objects, making them like inspector grab cards. |
| `SpawnInstanceOnTrigger` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to spawn an inspector when clicking primary with the grabbable this is on is being held. |

Fields
Collapse

## Usage

Attach to a slot with an [IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable") to make the grabbable act as the reference value itself.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:ValueProxy](https://wiki.resonite.com/Component:ValueProxy "Component:ValueProxy")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ReferenceProxy&oldid=101999](https://wiki.resonite.com/index.php?title=Component:ReferenceProxy&oldid=101999)"

Contents