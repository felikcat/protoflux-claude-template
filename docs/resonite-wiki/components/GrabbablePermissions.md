# Component:GrabbablePermissions

> Source: https://wiki.resonite.com/Component:GrabbablePermissions

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a0/GrabbablePermissionsComponent.png/510px-GrabbablePermissionsComponent.png)](https://wiki.resonite.com/File:GrabbablePermissionsComponent.png) **Grabbable Permissions** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GrabbablePermissions** component is used to control what roles can pick up what items.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Tags` | _direct_ **[TagFilter](https://wiki.resonite.com/Type:TagFilter "Type:TagFilter")** | A tag filter to filter what tags can or can't be grabbed by the selected roles. |
| `ValidateTypeListMode` | **[ListFilterMode](https://wiki.resonite.com/Type:ListFilterMode "Type:ListFilterMode")** | how to use the `ValidateTypes` list for the selected roles. |
| `ValidateTypes` | _[list](https://wiki.resonite.com/index.php?title=Type:SyncTypeList%601&action=edit&redlink=1 "Type:SyncTypeList`1 (page does not exist)")_ of **[SyncType](https://wiki.resonite.com/Type:SyncType "Type:SyncType")** | A list of C# types that will have `ValidateTypeListMode` applied to them. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

Used in the default world permissions slot in the root of a world to prevent spectators from interacting with items.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GrabbablePermissions&oldid=94784](https://wiki.resonite.com/index.php?title=Component:GrabbablePermissions&oldid=94784)"

Contents