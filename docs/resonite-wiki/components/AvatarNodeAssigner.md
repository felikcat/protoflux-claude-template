# Component:AvatarNodeAssigner

> Source: https://wiki.resonite.com/Component:AvatarNodeAssigner

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarNodeAssigner&diff=93719) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b3/AvatarNodeAssignerComponent.png/510px-AvatarNodeAssignerComponent.png)](https://wiki.resonite.com/File:AvatarNodeAssignerComponent.png) **AvatarNodeAssigner** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarNodeAssigner** component only functions on an avatar being equipped or de-equipped by a user. When equipped, the component finds the first [Component:AvatarObjectSlot](https://wiki.resonite.com/Component:AvatarObjectSlot "Component:AvatarObjectSlot") with a body node value that equals `Node`. if found, it assigns all slot storage fields in `Targets` to the slot the [Component:AvatarObjectSlot](https://wiki.resonite.com/Component:AvatarObjectSlot "Component:AvatarObjectSlot") is on. When de-equipped, all slot storage fields in `Targets` have their stored slot cleared.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Node` | **[BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode")** | The body node to search for when the avatar this is on is equipped. |
| `Targets` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") < [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot") >** | The slot storage fields to fill when an [Component:AvatarObjectSlot](https://wiki.resonite.com/Component:AvatarObjectSlot "Component:AvatarObjectSlot") of node type `Node` is found. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarNodeAssigner&oldid=93719](https://wiki.resonite.com/index.php?title=Component:AvatarNodeAssigner&oldid=93719)"

Contents