# Component:InventoryBrowser

> Source: https://wiki.resonite.com/Component:InventoryBrowser

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/5a/InventoryBrowserComponent.png/510px-InventoryBrowserComponent.png)](https://wiki.resonite.com/File:InventoryBrowserComponent.png) **Inventory Browser** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **InventoryBrowser** Component is the component that handles the [Inventory](https://wiki.resonite.com/Inventory "Inventory") screen.

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
| `CustomItemSpawn` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [Record](https://wiki.resonite.com/index.php?title=Type:Record&action=edit&redlink=1 "Type:Record (page does not exist)") >** | The function to use when spawning items instead of the default one. |
| `_user` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user this belongs to. |
| `_autoReinitialize` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to fix issues by auto reinitializing. |
| `_initFunction` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [RecordDirectory](https://wiki.resonite.com/index.php?title=Type:RecordDirectory&action=edit&redlink=1 "Type:RecordDirectory (page does not exist)") >** | The function to run when initalizing. |
| `_currentPath` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The current inventory path this is navigated to. |
| `_currentOwnerId` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The owner of this inventory screen. |
| `_addNewButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button for adding new directories. |
| `_deleteButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button for deleting items and directories. |
| `_inventoriesButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to go to the main inventories screen in order to go to the personal inventory or group shared inventories. |
| `_shareButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to share folders to the public. |
| `_unshareButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to unshare folders to the public. |
| `_copyLink` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to copy the link for an item or folder. |
| `_addCurrentAvatar` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to favorite the currently selected avatar |
| `_lastSpecialItemType` | **[InventoryBrowser.SpecialItemType](https://wiki.resonite.com/Component:InventoryBrowser#SpecialItemType)** | The last special item type that was selected in this inventory. |

Fields
Collapse

## SpecialItemType

Every one of these map to their corrosponding [favorite](https://wiki.resonite.com/Favorite "Favorite") item. To see what components map to these enums when saved to inventory, refer to the [favorites](https://wiki.resonite.com/Favorites "Favorites") page.

| Name | Value | Description |
| --- | --- | --- |
| `None` | 0 | There is no special item. |
| `Avatar` | 1 | The item is tagged as being an [Avatar](https://wiki.resonite.com/Avatar "Avatar"). |
| `World` | 2 | The item is tagged as being a [World Orb](https://wiki.resonite.com/World_Orb "World Orb"). |
| `VirtualKeyboard` | 3 | The item is tagged as being a vr keyboard. |
| `InteractiveCamera` | 4 | The item is tagged as being an interactive camera object like the [Camera](https://wiki.resonite.com/Camera "Camera"). |
| `Facet` | 5 | The item is tagged as being a [Facet](https://wiki.resonite.com/Facet "Facet") the user can put on their dash. |
| `AudioPlayer` | 6 | The item is tagged as being an [Audio Player](https://wiki.resonite.com/Audio_Player "Audio Player"). |
| `VideoPlayer` | 7 | The item is tagged as being a [Video Player](https://wiki.resonite.com/Video_Player "Video Player"). |
| `TextDisplay` | 8 | The item is tagged as being a text display for pasted text. |
| `UrlDisplay` | 9 | The item is tagged as being a URL display for pasted links. |
| `DocumentDisplay` | 10 | The item is tagged as being a document display for PDFs and other files. |
| `AudioStreamController` | 11 | The item is tagged as being an audio stream. |
| `ProgressBar` | 12 | The item is tagged as being a progress bar for importing items |
| `WorldLoadingIndicator` | 13 | The item is tagged as being a loading bar for loading into worlds. |
| `ColorDialog` | 14 | The item is tagged as being a color dialog. |

Values

## Usage

Not used directly by the user.

## Examples

Is used to create and manage the inventory menu and items.

## See Also

- [Inventory](https://wiki.resonite.com/Inventory "Inventory")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:InventoryBrowser&oldid=98938](https://wiki.resonite.com/index.php?title=Component:InventoryBrowser&oldid=98938)"

Contents