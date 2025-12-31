# Component:BrowserCreateDirectorDialog

> Source: https://wiki.resonite.com/Component:BrowserCreateDirectorDialog

(Redirected from [Component:BrowserCreateDirectorDialog](https://wiki.resonite.com/index.php?title=Component:BrowserCreateDirectorDialog&redirect=no "Component:BrowserCreateDirectorDialog"))

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:BrowserCreateDirectoryDialog&diff=98337) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/54/BrowserCreateDirectoryDialogComponent.png/510px-BrowserCreateDirectoryDialogComponent.png)](https://wiki.resonite.com/File:BrowserCreateDirectoryDialogComponent.png) **Browser Create Directory Dialog** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **BrowserCreateDirectoryDialogue** component is used mainly in the inventory screen when creating a new directory in the [inventory](https://wiki.resonite.com/Inventory "Inventory").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_browser` | **[BrowserDialog](https://wiki.resonite.com/Type:BrowserDialog "Type:BrowserDialog")** | The source browser Component. |
| `_callback` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[BrowserCreateDirectoryDialog.CreateHandler](https://wiki.resonite.com/Component:BrowserCreateDirectoryDialog#CreateHandler)** | A sync delegate to call when the Create Folder dialogue is confirmed. |
| `_text` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text for the Create Directory dialouge box. |
| `_textField` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The text field that is the name of the new directory. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `Create:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles creating a directory in the current directory. |
| `Cancel:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles canceling creating a directory. |

Triggers
Collapse

## CreateHandler

A sync delegate that takes a name and an "out string message" and modifies the message coming in. Returns a boolean.

## Usage

Used internally. Don't use it. :)

## Examples

The create directory dialogue in the inventory screen.

## See Also

- [Inventory](https://wiki.resonite.com/Inventory "Inventory") for what this controls.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BrowserCreateDirectoryDialog&oldid=98337](https://wiki.resonite.com/index.php?title=Component:BrowserCreateDirectoryDialog&oldid=98337)"

Contents