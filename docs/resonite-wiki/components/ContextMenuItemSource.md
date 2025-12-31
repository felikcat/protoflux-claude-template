# Component:ContextMenuItemSource

> Source: https://wiki.resonite.com/Component:ContextMenuItemSource

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/de/ContextMenuItemSourceComponent.png/510px-ContextMenuItemSourceComponent.png)](https://wiki.resonite.com/File:ContextMenuItemSourceComponent.png) **Context Menu Item Source** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

_This article or section is a stub. You can help the Resonite wiki by expanding it._

The ContextMenuItemSource component is used to add additional items to a [context menu](https://wiki.resonite.com/Context_menu "Context menu").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Label` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The text label next to the item. |
| `Color` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The background/border color of the item. |
| `Sprite` | **[IAssetProvider\`1](https://wiki.resonite.com/Type:IAssetProvider%601 "Type:IAssetProvider`1") < [Sprite](https://wiki.resonite.com/Type:Sprite "Type:Sprite") >** | The icon that is displayed on the item. |
| `ButtonEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not the button is active. If false, it will be greyed out and unclickable. |
| `AllowDrag` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not the user can drag onto the button from the center of the context menu to click it. |
| `CloseMenuOnPress` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not the context menu should be closed after the item is pressed. |
| `Pressed` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | See [ButtonEvents](https://wiki.resonite.com/ProtoFlux:Button_Events "ProtoFlux:Button Events") |
| `Pressing` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | See [ButtonEvents](https://wiki.resonite.com/ProtoFlux:Button_Events "ProtoFlux:Button Events") |
| `Released` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | See [ButtonEvents](https://wiki.resonite.com/ProtoFlux:Button_Events "ProtoFlux:Button Events") |

Fields
Collapse

## Usage

Attach to a slot, and provide a name and color. The name and color can also be dynamically driven using a [Value Option Description Driver](https://wiki.resonite.com/Component:ValueOptionDescriptionDriver "Component:ValueOptionDescriptionDriver") to display what the button does/did.

To show up, it needs to be either within a [Context Menu Submenu](https://wiki.resonite.com/ContextMenuSubmenu_(Component) "ContextMenuSubmenu (Component)") or assigned to a [Root Context Menu Item](https://wiki.resonite.com/RootContextMenuItem_(Component) "RootContextMenuItem (Component)") as its Item.

## Examples

This is extremely popular in almost every avatar in Resonite. It is used in context menus to allow the customization of avatar settings like clothes, systems, code, and colors on the run without having to use an inspector. This component is also used in

## Related Issues

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ContextMenuItemSource&oldid=91256](https://wiki.resonite.com/index.php?title=Component:ContextMenuItemSource&oldid=91256)"

Contents