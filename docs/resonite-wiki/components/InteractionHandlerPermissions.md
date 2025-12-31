# Component:InteractionHandlerPermissions

> Source: https://wiki.resonite.com/Component:InteractionHandlerPermissions

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c5/InteractionHandlerPermissionsComponent.png/510px-InteractionHandlerPermissionsComponent.png)](https://wiki.resonite.com/File:InteractionHandlerPermissionsComponent.png) **Interaction Handler Permissions** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AllowOnlyWhitelistedTools` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether only tools which are set to `Allow` are are allowed to be equipped. |
| `ToolRules` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[InteractionHandlerPermissions.ToolRule](https://wiki.resonite.com/Component:InteractionHandlerPermissions#ToolRule)** | List of ToolRules. |

Fields
Collapse

## Usage

The type in each list item corrisponds to a tool in the game. For example, FrooxEngine.ProtoFluxTool is a [ProtoFlux Tool](https://wiki.resonite.com/ProtoFlux_Tool "ProtoFlux Tool")
Type in the type's name, and you can choose to allow or deny that kind of tool from being used by the selected roles.

## ToolRule

_This article or section is a stub. You can help the Resonite wiki by expanding it._

| Name | Type | Description |
| --- | --- | --- |
| `Type` | _direct_ **[SyncType](https://wiki.resonite.com/Type:SyncType "Type:SyncType")** | The full name of the tool's [Type:Type](https://wiki.resonite.com/Type:Type "Type:Type") |
| `IncludeDerived` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Allow tools that fall under this classification IE: an interface. |
| `Allow` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to allow usage of this tool by the selected roles. |

Fields

## Examples

used in the non-builder permissions under the roles in a new grid world.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:InteractionHandlerPermissions&oldid=97545](https://wiki.resonite.com/index.php?title=Component:InteractionHandlerPermissions&oldid=97545)"

Contents