# Component:ContextMenuSubmenu

> Source: https://wiki.resonite.com/Component:ContextMenuSubmenu

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/8e/ContextMenuSubmenuComponent.png/510px-ContextMenuSubmenuComponent.png)](https://wiki.resonite.com/File:ContextMenuSubmenuComponent.png) **Context Menu Submenu** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

_This article or section is a stub. You can help the Resonite wiki by expanding it._

The ContextMenuSubmenu component can be used in combination with any button component to make said button open a custom context menu when clicked.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ItemsRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | All [Context Menu Item Sources](https://wiki.resonite.com/Component:ContextMenuItemSource "Component:ContextMenuItemSource") on slots immediately under this one will be included in the submenu. |
| `SearchWholeHierarchy` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Display all items under `ItemsRoot</slot> including sub slots, not just ones immediately under.<br>` |
| `DisableFlick` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow opening of the sub menu by clicking on the context menu center and moving it to this component's [Context Menu Item Source](https://wiki.resonite.com/Component:ContextMenuItemSource "Component:ContextMenuItemSource") on the same slot. |
| `SpeedOverride` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | Override the speed at which the new context menu will open. |
| `CounterClockwise` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the items should be arranged clockwise or counter-clockwise in the submenu. |
| `KeepPosition` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | When set, the context menu will stay in the same place as the submenu opens. Otherwise, the context menu will recenter on the user's laser. |
| `Hidden` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If set, the submenu is only visible to the user that opened it. |

Fields
Collapse

## Usage

Attach this component to a [slot](https://wiki.resonite.com/Slot "Slot") and attach a [Context Menu Item Source](https://wiki.resonite.com/Component:ContextMenuItemSource "Component:ContextMenuItemSource") along side it. Providing a slot to

## Examples

This is commonly used on avatars, using a [RootContextMenuItem](https://wiki.resonite.com/RootContextMenuItem_(Component) "RootContextMenuItem (Component)") as the button, but can also be used on anything else.

## Related Issues

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ContextMenuSubmenu&oldid=91257](https://wiki.resonite.com/index.php?title=Component:ContextMenuSubmenu&oldid=91257)"

Contents