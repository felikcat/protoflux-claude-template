# Component:AvatarObjectComponentProxy

> Source: https://wiki.resonite.com/Component:AvatarObjectComponentProxy

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarObjectComponentProxy&diff=93891) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f6/AvatarObjectComponentProxyComponent.png/510px-AvatarObjectComponentProxyComponent.png)](https://wiki.resonite.com/File:AvatarObjectComponentProxyComponent.png) **Avatar Object Component Proxy** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarObjectComponentProxy** component receives equipping, dequipping, and preequipping events and sends them to every [IAvatarObjectComponent](https://wiki.resonite.com/index.php?title=Type:IAvatarObjectComponent&action=edit&redlink=1 "Type:IAvatarObjectComponent (page does not exist)") component under the `Target`

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot with components to send Equipping, Deequipping, and prequipping events to. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarObjectComponentProxy&oldid=93891](https://wiki.resonite.com/index.php?title=Component:AvatarObjectComponentProxy&oldid=93891)"

Contents