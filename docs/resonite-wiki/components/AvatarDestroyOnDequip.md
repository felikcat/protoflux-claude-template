# Component:AvatarDestroyOnDequip

> Source: https://wiki.resonite.com/Component:AvatarDestroyOnDequip

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarDestroyOnDequip&diff=93120) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/61/AvatarDestroyOnDequipComponent.png/510px-AvatarDestroyOnDequipComponent.png)](https://wiki.resonite.com/File:AvatarDestroyOnDequipComponent.png) **AvatarDestroyOnDequip** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarDestroyOnDequip** component destroys `DestroyRoot` when the avatar it's in the hierarchy of is unequipped, or the slot the component is attached to if `DestroyRoot` is null.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `DestroyRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to destroy when the avatar this component is a part of is dequipped, or null to destroy the slot this component is attached to. |

Fields
Collapse

## Usage

Attach to a part of an Avatar's hierarchy and then provide a slot to `DestroyRoot` (or keep it null to destroy the slot this component is on). When the parent avatar is dequipped, the target slot will be destroyed.

## Examples

Can be used to remove slots that are generated when a user enters an avatar, but need to be destroyed when they leave said avatar. or it can destroy a slot outside the avatar, which could be used in puzzles or world systems.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarDestroyOnDequip&oldid=93120](https://wiki.resonite.com/index.php?title=Component:AvatarDestroyOnDequip&oldid=93120)"

Contents