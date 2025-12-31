# Component:FileSystemItem

> Source: https://wiki.resonite.com/Component:FileSystemItem

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/9c/FileSystemItemComponent.png/510px-FileSystemItemComponent.png)](https://wiki.resonite.com/File:FileSystemItemComponent.png) **File System Item** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **FileSystemItem** component is a type of [Type:BrowserItem](https://wiki.resonite.com/Type:BrowserItem "Type:BrowserItem") used for system files or inventory items being viewed on the [dash menu](https://wiki.resonite.com/Dash_Menu "Dash Menu").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Browser` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [BrowserDialog](https://wiki.resonite.com/Type:BrowserDialog "Type:BrowserDialog") >** | The source browser this item came from. |
| `SelectedColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color this item's background should be when selected. |
| `SelectedText` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color this item's text should be when selected. |
| `NormalColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color this item's background should be at rest state |
| `NormalText` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color this item's text would be at rest state. |
| `Name` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the |
| `BasePath` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The base directory of the item. |
| `Type` | **[FileSystemItem.EntryType](https://wiki.resonite.com/Component:FileSystemItem#EntryType)** | Whether if this is a file or folder. |

Fields
Collapse

## EntryType

| Name | Value | Description |
| --- | --- | --- |
| `File` | 0 | This entry refers to a file. |
| `Directory` | 1 | This entry refers to a folder. |

Values

## Usage

Used internally by the inventory and file system menus. Not used by the user.

## Examples

[Dash menu](https://wiki.resonite.com/Dash_menu "Dash menu") Inventory and file system screen file and folder items.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FileSystemItem&oldid=97505](https://wiki.resonite.com/index.php?title=Component:FileSystemItem&oldid=97505)"

Contents