# Component:RootContextMenuItem

> Source: https://wiki.resonite.com/Component:RootContextMenuItem

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/3a/RootContextMenuItemComponent.png/510px-RootContextMenuItemComponent.png)](https://wiki.resonite.com/File:RootContextMenuItemComponent.png) **Root Context Menu Item** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Root context menu item is a component that makes a new context menu item appear for the active user for when they open their context menu.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `OnlyForSide` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Chirality](https://wiki.resonite.com/Type:Chirality "Type:Chirality") >** | When set, the item will only be inserted when the context menu is opened on the specified hand. |
| `ExcludeOnTools` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not the item shows up when opening the context menu while having a tool equipped on the same hand. |
| `ExcludePrimaryHand` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Makes the item not show up when the context menu is open on the user's primary hand. |
| `ExcludeSecondaryHand` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Makes the item not show up when the context menu is open on the user's secondary hand. |
| `Item` | **[ContextMenuItemSource](https://wiki.resonite.com/Component:ContextMenuItemSource "Component:ContextMenuItemSource")** | The [ContextMenuItemSource](https://wiki.resonite.com/ContextMenuItemSource_(Component) "ContextMenuItemSource (Component)") that will be inserted into the context menu. |

Fields
Collapse

## Usage

## Examples

## Related Issues

## Related Components

[ContextMenuItemSource](https://wiki.resonite.com/Component:ContextMenuItemSource "Component:ContextMenuItemSource")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RootContextMenuItem&oldid=91535](https://wiki.resonite.com/index.php?title=Component:RootContextMenuItem&oldid=91535)"

Contents