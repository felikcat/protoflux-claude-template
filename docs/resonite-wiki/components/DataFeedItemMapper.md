# Component:DataFeedItemMapper

> Source: https://wiki.resonite.com/Component:DataFeedItemMapper

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/94/DataFeedItemMapperComponent.png/510px-DataFeedItemMapperComponent.png)](https://wiki.resonite.com/File:DataFeedItemMapperComponent.png) **Data Feed Item Mapper** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The DataFeedItemMapper allows you to define which data feed items map to which UI templates. It does this via the list `Mappings`, which take classes that extend [DataFeedItem](https://wiki.resonite.com/Type:DataFeedItem "Type:DataFeedItem") and If they match a mapping in the list it Duplicates that item's template and adds it into the list.

For more info on data feeds, see [Data Feeds](https://wiki.resonite.com/Data_Feed "Data Feed")

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Mappings` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[DataFeedItemMapper.ItemMapping](https://wiki.resonite.com/Component:DataFeedItemMapper#ItemMapping)** | A list of item Mappings to map data feed item types to Feed Templates. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnSetupTemplate:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Set up a basic settup with this component with a bunch of example UIs. |

Triggers
Collapse

## ItemMapping

| Name | Type | Description |
| --- | --- | --- |
| `ItemType` | _direct_ **[SyncType](https://wiki.resonite.com/Type:SyncType "Type:SyncType")** | The type to map to a template. The type coming from a data feed will extend the abstract class [DataFeedItem](https://wiki.resonite.com/Type:DataFeedItem "Type:DataFeedItem"). |
| `GenericReplacementTypes` | _[list](https://wiki.resonite.com/index.php?title=Type:SyncTypeList%601&action=edit&redlink=1 "Type:SyncTypeList`1 (page does not exist)")_ of **[SyncType](https://wiki.resonite.com/Type:SyncType "Type:SyncType")** | If `ItemType` is a type that has generic single letter arguments, the type won't be accepted if it's arguments in order don't match the arguments in this list in order. |
| `Template` | **[FeedItemInterface](https://wiki.resonite.com/Component:FeedItemInterface "Component:FeedItemInterface")** | The template to duplicate when matched with this item mapping. |

Fields

## Usage

This component is to be put into a [Component:SingleFeedView](https://wiki.resonite.com/Component:SingleFeedView "Component:SingleFeedView") or similar so that the component it is specified inside of can use this component to map incoming feed items from the data feed to UI or object templates.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DataFeedItemMapper&oldid=97914](https://wiki.resonite.com/index.php?title=Component:DataFeedItemMapper&oldid=97914)"

Contents