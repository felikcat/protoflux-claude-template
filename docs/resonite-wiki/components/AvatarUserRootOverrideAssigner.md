# Component:AvatarUserRootOverrideAssigner

> Source: https://wiki.resonite.com/Component:AvatarUserRootOverrideAssigner

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarUserRootOverrideAssigner&diff=97402) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/32/AvatarUserRootOverrideAssignerComponent.png/510px-AvatarUserRootOverrideAssignerComponent.png)](https://wiki.resonite.com/File:AvatarUserRootOverrideAssignerComponent.png) **AvatarUserRootOverrideAssigner** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Avatar User Root Override Assigner is a component that allows for changing the user's viewpoint, the user's first person standing location, or the user's ears location. This component works if parented under a user, for that user.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Override` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to relocate the user's eyes or ears to. |
| `Node` | **[AvatarUserRootOverrideAssigner.OverrideNode](https://wiki.resonite.com/Component:AvatarUserRootOverrideAssigner#OverrideNode)** | Whether to make the user's eyes, Standing position, or ears located at `Slot` without changing any slot transforms. |
| `_equippingSlot` | **[AvatarObjectSlot](https://wiki.resonite.com/Component:AvatarObjectSlot "Component:AvatarObjectSlot")** | an Avatar Object Slot to use for handling this node. |

Fields
Collapse

## OverrideNode

| Name | Value | Description |
| --- | --- | --- |
| `Eyes` | 0 | Make the user's view see from `Override` rather than the original position it usually is at. This however prevents looking around unless the slot is driven by the user's head rotation. |
| `Ears` | 1 | make the the user hear from `Override` position and rotation (not scale) rather than from their head. |
| `AvatarRoot` | 2 | Visually relocates the user's head and ears position to `Override` this makes it seem as if they were parented to the slot but without their Avatar. This is purely visual, and does not restrict looking around. |

Values

## Behavior

Needs to be parented under a user to work, and applies to the parent user. The component requires a slot, and an [AvatarObjectSlot](https://wiki.resonite.com/Component:AvatarObjectSlot "Component:AvatarObjectSlot"). The Avatar Object slot does not need an existing one, so best practice is to add a new Avatar Object Slot to the same Slot as this component, then put it into the `_equippingSlot` field. Also, adding the slot this component is on to `Override` allows for a self contained settup in one slot that fully works when parented to a user.

## Examples

- [GearBell's](https://wiki.resonite.com/index.php?title=User:GearBell&action=edit&redlink=1 "User:GearBell (page does not exist)") purple pill. (Overrides viewpoint to pill when held)
- [989onan's](https://wiki.resonite.com/User:989onan "User:989onan") Camera Override masked Protogen (allows for switching to the viewpoints of previously equipped visors)

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarUserRootOverrideAssigner&oldid=97402](https://wiki.resonite.com/index.php?title=Component:AvatarUserRootOverrideAssigner&oldid=97402)"

Contents