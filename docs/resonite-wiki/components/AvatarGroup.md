# Component:AvatarGroup

> Source: https://wiki.resonite.com/Component:AvatarGroup

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarGroup&diff=93910) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/ba/AvatarGroupComponent.png/510px-AvatarGroupComponent.png)](https://wiki.resonite.com/File:AvatarGroupComponent.png) **AvatarGroup** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

For detailed information on how this functions for mix and match body parts. Please also see [Equipping Multiple Avatars](https://wiki.resonite.com/Equipping_Multiple_Avatars "Equipping Multiple Avatars").

AvatarGroup is a component commonly found on the root of an avatar. It mostly controls where the avatar should be parented back to when dequipped, and is set by a user's [Avatar Manager](https://wiki.resonite.com/Component:AvatarManager "Component:AvatarManager").

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `OriginalParent` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot that this avatar was parented under before being equipped. |

Fields
Collapse

## Behavior

This component is currently not entirely functioning. see [Issue 3076](https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/3076)

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarGroup&oldid=93910](https://wiki.resonite.com/index.php?title=Component:AvatarGroup&oldid=93910)"

Contents