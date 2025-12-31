# Component:AvatarUserPositioner

> Source: https://wiki.resonite.com/Component:AvatarUserPositioner

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarUserPositioner&diff=98196) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f6/AvatarUserPositionerComponent.png/510px-AvatarUserPositionerComponent.png)](https://wiki.resonite.com/File:AvatarUserPositionerComponent.png) **Avatar User Positioner** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarUserPositioner** component is used to position a user to the avatar upon equipping the avatar.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `PositionNode` | **[UserRoot.UserNode](https://wiki.resonite.com/Component:UserRoot#UserNode "Component:UserRoot")** | What node to use to match the position of the user. |
| `RotationNode` | **[UserRoot.UserNode](https://wiki.resonite.com/Component:UserRoot#UserNode "Component:UserRoot")** | What node to use to match the rotation of the user. |
| `PositionReference` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to position the user to instead of the slot this component is on when they equip the user. |
| `RotationReference` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to rotate the user to instead of the slot this component is on when they equip the user. |
| `PreserveUp` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to upright the user when they equip the avatar, or set them to the rotation this avatar is in when equipping. |
| `OnManualEquipOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to trigger this positioner only when the user clicks on the avatar to equip it rather than also triggering when the avatar is equipped through flux. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarUserPositioner&oldid=98196](https://wiki.resonite.com/index.php?title=Component:AvatarUserPositioner&oldid=98196)"

Contents