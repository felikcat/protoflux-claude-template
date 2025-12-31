# Component:AvatarBadgeManager

> Source: https://wiki.resonite.com/Component:AvatarBadgeManager

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarBadgeManager&diff=91531) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/5c/AvatarBadgeManagerComponent.png/510px-AvatarBadgeManagerComponent.png)](https://wiki.resonite.com/File:AvatarBadgeManagerComponent.png) **AvatarBadgeManager** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarBadgeManager** component initializes the [user's](https://wiki.resonite.com/User "User") [badges](https://wiki.resonite.com/Badges "Badges") under the `Badges Root` slot.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `BadgeSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The size of the generated badges in local space. |
| `BadgeSeparation` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The separation in meters between the badges in local space |
| `MaxRowSize` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The maximum amount of badges on one row before moving to the next. |
| `_badgesRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to put the badges under. |
| `_badgesOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position of the `_badgesRoot` slot, which is used to move the badges away from the user's name tag and keep them positioned properly. |

Fields
Collapse

## Usage

This is used to help with organizing badges on a user's [Nameplate](https://wiki.resonite.com/Nameplate "Nameplate"), including custom badges. The [user badge manager](https://wiki.resonite.com/User_Badge_Manager "User Badge Manager") does this internally to help assign badges accordingly.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarBadgeManager&oldid=91531](https://wiki.resonite.com/index.php?title=Component:AvatarBadgeManager&oldid=91531)"

Contents