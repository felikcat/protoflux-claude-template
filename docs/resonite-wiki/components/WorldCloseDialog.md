# Component:WorldCloseDialog

> Source: https://wiki.resonite.com/Component:WorldCloseDialog

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/8e/WorldCloseDialogComponent.png/510px-WorldCloseDialogComponent.png)](https://wiki.resonite.com/File:WorldCloseDialogComponent.png) **World Close Dialog** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **WorldCloseDialog** component is used to confirm closing a world that the user is currently trying to close.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_worldName` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text field showing the name of the world being closed. |
| `_saveButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button used to save the world being closed. |
| `_saveAsButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button used to save the world as something for the world being closed. |
| `_discardButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button used to discard changes for the world being closed. |
| `_saveAction` | **[WorldCloseAction](https://wiki.resonite.com/Component:WorldCloseAction "Component:WorldCloseAction")** | The component to trigger with the request to save the world being closed. |
| `_saveAsAction` | **[WorldCloseAction](https://wiki.resonite.com/Component:WorldCloseAction "Component:WorldCloseAction")** | The component to trigger with the request to save the world as something for the world being closed. |
| `_discardAction` | **[WorldCloseAction](https://wiki.resonite.com/Component:WorldCloseAction "Component:WorldCloseAction")** | The component to trigger with the request to discard changes for the world being closed. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `Close:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | ✓ | Tells the world to close. |
| `OnCancel:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Tells the dialog to cancel closing the world. |

Triggers
Collapse

## Usage

Not used directly by the user.

## Examples

Generated when the user tries to close a world that has unsaved changes.

## See Also

- [World](https://wiki.resonite.com/World "World")
- [Worlds Menu](https://wiki.resonite.com/index.php?title=Worlds_Menu&action=edit&redlink=1 "Worlds Menu (page does not exist)")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:WorldCloseDialog&oldid=100812](https://wiki.resonite.com/index.php?title=Component:WorldCloseDialog&oldid=100812)"

Contents