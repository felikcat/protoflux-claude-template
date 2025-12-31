# Component:AvatarTrackingOffset

> Source: https://wiki.resonite.com/Component:AvatarTrackingOffset

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarTrackingOffset&diff=92139) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b3/AvatarTrackingOffsetComponent.png/510px-AvatarTrackingOffsetComponent.png)](https://wiki.resonite.com/File:AvatarTrackingOffsetComponent.png) **AvatarTrackingOffset** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

AvatarTrackingOffset can be used to shift the position of your trackers (including headset and hands) by a certain amount for an avatar.
To work, the component needs to be in the avatar's hierarchy.

This component effectively works like a "Playspace Mover".

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Offset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The amount that your tracking position should be offset when in the avatar |
| `_user` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user to which the offset is applied. This is set automatically when equipping an avatar with this component |

Fields
Collapse

## Behavior

## Examples

[SerenityFen](https://wiki.resonite.com/index.php?title=User:SerenityFen&action=edit&redlink=1 "User:SerenityFen (page does not exist)") uses this on their avatar's polymorph settings so that they move up when their legs are lengthened via scaling them.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarTrackingOffset&oldid=92139](https://wiki.resonite.com/index.php?title=Component:AvatarTrackingOffset&oldid=92139)"

Contents