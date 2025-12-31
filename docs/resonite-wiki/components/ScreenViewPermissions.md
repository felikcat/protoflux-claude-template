# Component:ScreenViewPermissions

> Source: https://wiki.resonite.com/Component:ScreenViewPermissions

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d4/ScreenViewPermissionsComponent.png/510px-ScreenViewPermissionsComponent.png)](https://wiki.resonite.com/File:ScreenViewPermissionsComponent.png) **Screen View Permissions** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ScreenViewPermissions** component is a [Permissions](https://wiki.resonite.com/index.php?title=Permissions&action=edit&redlink=1 "Permissions (page does not exist)") type component that can apply rules for what certain roles in a session can do with views like third person, free cam, or UI targetting.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ListMode` | **[ListFilterMode](https://wiki.resonite.com/Type:ListFilterMode "Type:ListFilterMode")** | How to filter and handle the list of `ViewFilters` for the selected roles. |
| `ViewFilters` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[ScreenViewPermissions.ViewTargettingFilter](https://wiki.resonite.com/Component:ScreenViewPermissions#ViewTargettingFilter)** | A list of targetting views to check a user with the selected role(s) with and act accordingly on if they are using one in the list. |

Fields
Collapse

## ViewTargettingFilter

| Name | Type | Description |
| --- | --- | --- |
| `ViewTargettingType` | _direct_ **[SyncType](https://wiki.resonite.com/Type:SyncType "Type:SyncType")** | The C# Type a View target has to be in order to be matched to this list item. |
| `RequireTag` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | This tag is required for a View targeting mode to be matched to this list item. |
| `EditModeOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The user has to be in edit mode for a View targeting mode to be matched to this list item. |

Fields

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

Can be used to prevent desktop users from going into third person or free cam, to prevent cheating in horror games or mazes.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ScreenViewPermissions&oldid=97720](https://wiki.resonite.com/index.php?title=Component:ScreenViewPermissions&oldid=97720)"

Contents