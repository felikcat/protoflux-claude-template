# Component:RootCategoryView

> Source: https://wiki.resonite.com/Component:RootCategoryView

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a6/RootCategoryViewComponent.png/510px-RootCategoryViewComponent.png)](https://wiki.resonite.com/File:RootCategoryViewComponent.png) **Root Category View** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **RootCategoryView** component is commonly used in [Settings](https://wiki.resonite.com/Settings "Settings"), and [Worlds Menu](https://wiki.resonite.com/index.php?title=Worlds_Menu&action=edit&redlink=1 "Worlds Menu (page does not exist)") view to show the list of root view categories while still showing the current `Path` like audio device lists, trackers, worlds, or anything else feeds might have.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Feed` | **[IDataFeedComponent](https://wiki.resonite.com/Type:IDataFeedComponent "Type:IDataFeedComponent")** | The Feed to view items for in this data feed view. |
| `Path` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The path within the feed to view. |
| `GroupingKeys` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | A list of grouping keys to group alike data feed items together from the incoming data. |
| `SearchPhrase` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The phrase to search for within the current list of feed items under `Path`. |
| `UpdatingUser` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user handling the logic for this data feed view. |
| `ResetViewOnSave` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to clear the view upon saving this data feed view. |
| `CategoryManager` | _direct_ **[DataFeedItemMappingManager](https://wiki.resonite.com/Type:DataFeedItemMappingManager "Type:DataFeedItemMappingManager")** | The Mapper to handle showing categories in the root regardless of what `Path` is. |
| `ItemsManager` | _direct_ **[DataFeedItemMappingManager](https://wiki.resonite.com/Type:DataFeedItemMappingManager "Type:DataFeedItemMappingManager")** | The Mapper to handle showing items within a selected `Path`, no matter how deep of a `Path` this is viewing. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnSetupTemplate:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the setup template button is touched. |
| `PathSegmentName:PathSegmentConverter` | **[PathSegmentConverter](https://wiki.resonite.com/index.php?title=Type:PathSegmentConverter&action=edit&redlink=1 "Type:PathSegmentConverter (page does not exist)")** | X | Converts a path name element and a depth into a corresponding locale string for translation. |

Triggers
Collapse

## Usage

Attach to a slot and provide a [Feed](https://wiki.resonite.com/Type:IDataFeedView "Type:IDataFeedView"), a [Item Mapper](https://wiki.resonite.com/Component:DataFeedItemMapper "Component:DataFeedItemMapper"), and Slots to place items in order for it to work.

## Examples

Used in the settings and world views.

## See Also

- [Other Data Feed Views](https://wiki.resonite.com/Type:IDataFeedView "Type:IDataFeedView")
- [Data Feeds](https://wiki.resonite.com/Data_Feeds "Data Feeds")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RootCategoryView&oldid=99205](https://wiki.resonite.com/index.php?title=Component:RootCategoryView&oldid=99205)"

Contents