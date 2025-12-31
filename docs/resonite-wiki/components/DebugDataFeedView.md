# Component:DebugDataFeedView

> Source: https://wiki.resonite.com/Component:DebugDataFeedView

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b4/DebugDataFeedViewComponent.png/510px-DebugDataFeedViewComponent.png)](https://wiki.resonite.com/File:DebugDataFeedViewComponent.png) **Debug Data Feed View** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DebugDataFeedView** component shows the data from a feed including calls to update already provided data from the feed.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This game element is a debug item. Elements like this may be removed at any time without warning, and creations should not rely on it.


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
| `TargetOutput` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field (usually the text on a text renderer) to update with the debug feed data. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `PathSegmentName:PathSegmentConverter` | **[PathSegmentConverter](https://wiki.resonite.com/index.php?title=Type:PathSegmentConverter&action=edit&redlink=1 "Type:PathSegmentConverter (page does not exist)")** | X | Converts a path name element and a depth into a corresponding locale string for translation. |

Triggers
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Other Data Feed Views](https://wiki.resonite.com/Type:IDataFeedView "Type:IDataFeedView")
- [Data Feeds](https://wiki.resonite.com/Data_Feeds "Data Feeds")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DebugDataFeedView&oldid=99204](https://wiki.resonite.com/index.php?title=Component:DebugDataFeedView&oldid=99204)"

Contents