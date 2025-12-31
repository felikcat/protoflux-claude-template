# Component:WorldOrbSaver

> Source: https://wiki.resonite.com/Component:WorldOrbSaver

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[File:WorldOrbSaverComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=WorldOrbSaverComponent.png "File:WorldOrbSaverComponent.png") **World Orb Saver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **WorldOrbSaver** Component handles when a user is saving a world to their inventory when saving a world in general.

See [World](https://wiki.resonite.com/World "World") for more info about worlds.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Orb` | **[WorldOrb](https://wiki.resonite.com/Component:WorldOrb "Component:WorldOrb")** | The orb to save to the user's inventory. |
| `saveHereItem` | **[ContextMenuItem](https://wiki.resonite.com/Component:ContextMenuItem "Component:ContextMenuItem")** | The context menu item used to trigger "Save Here". |
| `saveToInventoryItem` | **[ContextMenuItem](https://wiki.resonite.com/Component:ContextMenuItem "Component:ContextMenuItem")** | The context menu item used to trigger "Save to Inventory". |
| `cancelItem` | **[ContextMenuItem](https://wiki.resonite.com/Component:ContextMenuItem "Component:ContextMenuItem")** | The context menu item used to trigger "Cancel" |
| `menu` | **[ContextMenu](https://wiki.resonite.com/Component:ContextMenu "Component:ContextMenu")** | The context menu that was opened to handle this item's menu. |
| `interactive` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this item is interactive or not. |
| `saving` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this item is currently saving to the user's inventory. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnSaveHere:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the item is being "saved here". |
| `OnSaveToInventory:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the item is being saved to inventory. |
| `OnCancel:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the saving of this item is being canceled. |

Triggers
Collapse

## Usage

See [World](https://wiki.resonite.com/World "World") for more info about worlds.

## Examples

See [World](https://wiki.resonite.com/World "World") for more info about worlds.

## See Also

- [World](https://wiki.resonite.com/World "World")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:WorldOrbSaver&oldid=100816](https://wiki.resonite.com/index.php?title=Component:WorldOrbSaver&oldid=100816)"

Contents