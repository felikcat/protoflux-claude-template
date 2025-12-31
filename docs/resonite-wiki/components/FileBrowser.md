# Component:FileBrowser

> Source: https://wiki.resonite.com/Component:FileBrowser

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[File:FileBrowserComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=FileBrowserComponent.png "File:FileBrowserComponent.png") **File Browser** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **FileBrowser** component is used to show file lists of files on the user's PC in the [userspace](https://wiki.resonite.com/Userspace "Userspace") [dash menu](https://wiki.resonite.com/Dash_menu "Dash menu").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `SelectedItem` | **[BrowserItem](https://wiki.resonite.com/Type:BrowserItem "Type:BrowserItem")** | The currently selected item being highlighted. |
| `_previousSelectedItem` | **[BrowserItem](https://wiki.resonite.com/Type:BrowserItem "Type:BrowserItem")** | The item previously highlighted. |
| `AllowSelect` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this file browser allows selecting item elements. |
| `ItemSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How big the items are on the view. |
| `_selectedText` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text to fill with the name of the selected item. |
| `_pathRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of the area being used to display the current path. |
| `_buttonsRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of the area being used to show the different button actions. |
| `_folderGrid` | **[GridLayout](https://wiki.resonite.com/Component:GridLayout "Component:GridLayout")** | The grid layout Component being used to align the folders in the directory. |
| `_itemGrid` | **[GridLayout](https://wiki.resonite.com/Component:GridLayout "Component:GridLayout")** | The grid layout Component being used to align the files in the directory. |
| `_tabSprite` | **[SpriteProvider](https://wiki.resonite.com/Component:SpriteProvider "Component:SpriteProvider")** | The sprite being used to show the tab sprite. |
| `_loadingIndicator` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot that stores the loading indicator for a newly opened directory. |
| `_swapper` | **[SlideSwapRegion](https://wiki.resonite.com/Component:SlideSwapRegion "Component:SlideSwapRegion")** | The component to handle the slide animation when opening a different directory. |
| `CurrentPath` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The current folder path. |
| `_lastPath` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The last folder path. |
| `_user` | _direct_ **[MachineUserRef](https://wiki.resonite.com/index.php?title=Type:MachineUserRef&action=edit&redlink=1 "Type:MachineUserRef (page does not exist)")** | The user using this file browser. |
| `_importButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to import a selected folder or file. |
| `_rawImportButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to import a selected file as a raw file object. |
| `_createNewButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to create a new file directory. |
| `_reloadButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button used to refresh the folder and file list. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `CreateDirectory:CreateHandler` | **[CreateHandler](https://wiki.resonite.com/Component:BrowserCreateDirectoryDialog#CreateHandler "Component:BrowserCreateDirectoryDialog")** | ✓ | Called when a directory is created. |
| `RunImport:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when an import needs to be made of a file. |
| `RunRawImport:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when a raw file import needs to be made of a file. |
| `CreateNew:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when a new item needs to be made. |
| `Reload:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when a reload needs to be done. |
| `OnGoUp:ButtonEventHandler<int>` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)") < [int](https://wiki.resonite.com/Type:Int "Type:Int") >** | ✓ | Called when the user wants to go up in directories. |

Triggers
Collapse

## CreateHandler

Handles creation of directories. Is a sync delegate type.

## Usage

Not used directly by the user.

## Examples

Used in the dash menu on the file browser tab.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FileBrowser&oldid=100110](https://wiki.resonite.com/index.php?title=Component:FileBrowser&oldid=100110)"

Contents