# Component:WorldPermissions

> Source: https://wiki.resonite.com/Component:WorldPermissions

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/91/WorldPermissionsComponent.png/510px-WorldPermissionsComponent.png)](https://wiki.resonite.com/File:WorldPermissionsComponent.png) **World Permissions** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **WorldPermissions** component controls various actions the selected roles can do in the world.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AllowSavingItems` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the selected roles can save items. |
| `AllowTransferingObjectsOut` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the selected roles can [smuggle](https://wiki.resonite.com/Transcient_Grabbing "Transcient Grabbing") items out. |
| `AllowSpawningObjects` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the selected roles can spawn objects. |
| `AllowSwappingAvatars` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the selected roles can swap into a different avatar. |
| `SaveCopyPermission` | **[WorldPermissions.SavePermission](https://wiki.resonite.com/Component:WorldPermissions#SavePermission)** | When can the selected roles save the world? |

Fields
Collapse

## SavePermission

| Name | Value | Description |
| --- | --- | --- |
| `OnlyOwners` | 0 | Only the owner or a member of a group that the group owns the world can save it. |
| `OnlyWhenPublic` | 1 | Only allow saving if the world is public. |
| `Anyone` | 2 | Anyone can save the world. |

Values

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

Found in the Permissions slot in the root of a world.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:WorldPermissions&oldid=97836](https://wiki.resonite.com/index.php?title=Component:WorldPermissions&oldid=97836)"

Contents