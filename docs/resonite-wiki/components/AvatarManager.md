# Component:AvatarManager

> Source: https://wiki.resonite.com/Component:AvatarManager

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarManager&diff=97395) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/39/AvatarManagerComponent.png/510px-AvatarManagerComponent.png)](https://wiki.resonite.com/File:AvatarManagerComponent.png) **AvatarManager** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

For detailed information on how this functions for mix and match body parts. Please also see [Equipping Multiple Avatars](https://wiki.resonite.com/Equipping_Multiple_Avatars "Equipping Multiple Avatars").

The **AvatarManager** component is found on User root slots and is used to manage avatars equipped to a particular user. It also keeps track of and sets the equipped parameters of [Component:AvatarObjectSlots](https://wiki.resonite.com/Component:AvatarObjectSlot "Component:AvatarObjectSlot") under an avatar, It manages the setting of fields on the [Component:AvatarRoot](https://wiki.resonite.com/Component:AvatarRoot "Component:AvatarRoot") and [Component:AvatarGroup](https://wiki.resonite.com/Component:AvatarGroup "Component:AvatarGroup") components.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_objectGroups` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[AvatarManager.EquippedGroup](https://wiki.resonite.com/Component:AvatarManager#EquippedGroup)** | A list of objects currently equipped by the user as part of an avatar. |
| `_currentAnchor` | _direct_ **[LinkRef\`1](https://wiki.resonite.com/index.php?title=Type:LinkRef%601&action=edit&redlink=1 "Type:LinkRef`1 (page does not exist)") < [AvatarAnchor](https://wiki.resonite.com/Component:AvatarAnchor "Component:AvatarAnchor") >** | The anchor the user associated with this component is currently sitting in. |
| `AutoAddNameBadge` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to auto add the name badge component if it doesn't exist on an avatar when equipping it. Usually managed by the world through the [Component:CommonAvatarBuilder](https://wiki.resonite.com/Component:CommonAvatarBuilder "Component:CommonAvatarBuilder") |
| `AutoAddIconBadge` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to auto add the icon badges if it doesn't exist on an avatar when equipping it. Usually managed by the world through the [Component:CommonAvatarBuilder](https://wiki.resonite.com/Component:CommonAvatarBuilder "Component:CommonAvatarBuilder") |
| `AutoAddLiveIndicator` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to auto add the live indicator component if it doesn't exist on an avatar when equipping it. Usually managed by the world through the [Component:CommonAvatarBuilder](https://wiki.resonite.com/Component:CommonAvatarBuilder "Component:CommonAvatarBuilder") |
| `EmptySlotHandler` | **[IEmptyAvatarSlotHandler](https://wiki.resonite.com/Type:IEmptyAvatarSlotHandler "Type:IEmptyAvatarSlotHandler")** | The object to handle empty avatar slots. Usually defined by the world through the [Component:CommonAvatarBuilder](https://wiki.resonite.com/Component:CommonAvatarBuilder "Component:CommonAvatarBuilder"). |
| `DefaultScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The default scale multiplier of the avatar currently equipped |
| `NameTagText` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The text that should be assigned to the avatar nametag's text field list |
| `NameTagColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color that should be assigned to the avatar nametag's color list. |
| `NameTagOutline` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color that should be assigned to the avatar nametag's color1 list. |
| `NameTagBackground` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color.that should be assigned to the avatar nametag's color background list. |
| `_badgeTemplates` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the slot that was made for the user for storage of their badges. |
| `_autoNameBadge` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the slot that was made for the user for their name badge. |
| `_autoIconBadge` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the slot that was made for the user for their Icon. |
| `_autoLiveIndicator` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot that was made for the user for their live indicator |
| `_updateVersion` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Internal. |

Fields
Collapse

## EquippedGroup

Equipped group is internally handled as a type to hold data from a Dictionary< [Component:AvatarRoot](https://wiki.resonite.com/Component:AvatarRoot "Component:AvatarRoot"), _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[Component:AvatarObjectSlot](https://wiki.resonite.com/Component:AvatarObjectSlot "Component:AvatarObjectSlot")** >

| Name | Type | Description |
| --- | --- | --- |
| `Root` | [AvatarRoot](https://wiki.resonite.com/Component:AvatarRoot "Component:AvatarRoot") | The avatar root associated with the currently equipped avatar. |
| `ObjectSlots` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[Component:AvatarObjectSlot](https://wiki.resonite.com/Component:AvatarObjectSlot "Component:AvatarObjectSlot")** | The list of currently equipped object nodes associated with `Root`. |

Fields

## Usage

Should not be used directly by the player, since this is used by the game instead to manage avatars on a user.

## Examples

## See Also

- [Equipping Multiple Avatars](https://wiki.resonite.com/Equipping_Multiple_Avatars "Equipping Multiple Avatars")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarManager&oldid=97395](https://wiki.resonite.com/index.php?title=Component:AvatarManager&oldid=97395)"

Contents