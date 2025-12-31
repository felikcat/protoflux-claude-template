# Component:FolderImportDialog

> Source: https://wiki.resonite.com/Component:FolderImportDialog

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c9/FolderImportDialogComponent.png/510px-FolderImportDialogComponent.png)](https://wiki.resonite.com/File:FolderImportDialogComponent.png) **Folder Import Dialog** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **FolderImportDialog** component is used to make and handle the importing of a folder with the specified path. Generates a UIX upon attach.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Path` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The folder path to Import the contents of. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``RunImport:ButtonEventHandler`1<Int>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | ✓ | Imports the folder with the specified index option. |

Triggers
Collapse

## Usage

Used to Import folders. Use the version created via the normal [Import](https://wiki.resonite.com/Import "Import") process instead.

## Examples

Folder Import dialogue when importing folders into the game.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FolderImportDialog&oldid=97934](https://wiki.resonite.com/index.php?title=Component:FolderImportDialog&oldid=97934)"

Contents