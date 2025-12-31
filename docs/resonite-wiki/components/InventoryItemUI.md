# Component:InventoryItemUI

> Source: https://wiki.resonite.com/Component:InventoryItemUI

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/8a/InventoryItemUIComponent.png/510px-InventoryItemUIComponent.png)](https://wiki.resonite.com/File:InventoryItemUIComponent.png) **Inventory Item UI** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **InventoryItemUI** component is used to represent an item or folder in the [Inventory](https://wiki.resonite.com/Inventory "Inventory").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Browser` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [BrowserDialog](https://wiki.resonite.com/Type:BrowserDialog "Type:BrowserDialog") >** | The browser this belongs too. |
| `SelectedColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of this item when selected. |
| `SelectedText` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The text of this item when selected. |
| `NormalColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of this item when not selected. |
| `NormalText` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The text of this item when not selected. |

Fields
Collapse

## Usage

Not used by the user.

## Examples

Makes up the [Inventory](https://wiki.resonite.com/Inventory "Inventory") UI.

## See Also

- [Inventory](https://wiki.resonite.com/Inventory "Inventory")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:InventoryItemUI&oldid=98942](https://wiki.resonite.com/index.php?title=Component:InventoryItemUI&oldid=98942)"

Contents