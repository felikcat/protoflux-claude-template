# Component:AvatarObjectPermissions

> Source: https://wiki.resonite.com/Component:AvatarObjectPermissions

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarObjectPermissions&diff=93892) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f9/AvatarObjectPermissionsComponent.png/510px-AvatarObjectPermissionsComponent.png)](https://wiki.resonite.com/File:AvatarObjectPermissionsComponent.png) **Avatar Object Permissions** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarObjectPermission** component is a [Permissions](https://wiki.resonite.com/index.php?title=Permissions&action=edit&redlink=1 "Permissions (page does not exist)") component which determines which avatars users are allowed to equip if the avatar is tagged properly.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Tags` | _direct_ **[TagFilter](https://wiki.resonite.com/Type:TagFilter "Type:TagFilter")** | The list of tags and whether they are white listed or black listed |

Fields
Collapse

## Usage

This permission allows or disallows specific avatars to be used. Tags are used to determine to in-/equipability of such tagged avatars.

## Examples

Avatar-A has the Tag "AvatarA".
Avatar-B has the Tag "AvatarB".

If the permission is set to `Whitelist` then only the tags which \*are\* in the list are allowed to be equipped.

If the list contains "A" as a tag and only AvatarA has the Tag (on avatar root) "A" and the FilterMode is set to `Whitelist`. Then only AvatarA is allowed to be equipped.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarObjectPermissions&oldid=93892](https://wiki.resonite.com/index.php?title=Component:AvatarObjectPermissions&oldid=93892)"

Contents