# Component:FeedIndicatorInterface

> Source: https://wiki.resonite.com/Component:FeedIndicatorInterface

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/72/FeedIndicatorInterface%601Component.png/510px-FeedIndicatorInterface%601Component.png)](https://wiki.resonite.com/File:FeedIndicatorInterface%601Component.png) **Feed Indicator Interface\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **FeedIndicatorInterface** component is used as a template type item in data feed mappers in the [Data Feeds](https://wiki.resonite.com/Data_Feeds "Data Feeds") system. This works as a value viewing module for Feed items, as well as providing the wanted format for the item.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HasData` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The field to set when this interface is templated by a data feed for whether it has data or not. |
| `ItemName` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field to fill with the name of the interface item when it is templated via a data feed. For settings toggles, this would be the toggle name. |
| `ItemKey` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field to fill with the interfaces key if it is a dictionary type item. |
| `ItemDescription` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field to fill with the template description when template via a data feed. |
| `HasDescription` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | Whether the item when templated via a data feed has a description. |
| `DescriptionCleanup` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | If this interface doesn't have a description during templating via a data feed, then delete the slot specified. |
| `ItemIcon` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Uri](https://wiki.resonite.com/Type:Uri "Type:Uri") >** | The resource URL to fill with an image link/URI if the data feed item has an icon. |
| `HasIcon` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | Whether this template has an icon. This is set during duplication as a template via a data feed. |
| `IconCleanup` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to delete when this interface item doesn't have an icon when being duplicated as a template item by a data feed. |
| `View` | **[SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") < [IDataFeedView](https://wiki.resonite.com/Type:IDataFeedView "Type:IDataFeedView") >** | The data feed view that this template was instantiated by. Like a [SingleFeedView](https://wiki.resonite.com/Component:SingleFeedView "Component:SingleFeedView"). |
| `ParentContainer` | **[FeedItemInterface](https://wiki.resonite.com/Component:FeedItemInterface "Component:FeedItemInterface")** | This template's parent container. If that template also has a parent and a child, then it recursively goes up the containers till it finds the root interface with a parent and a child interface, then instantiates that interfaces child interface and it's Nested items instead of just this interface. |
| `ChildContainer` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | This template's child template which it instanciates if it's part of a parent child structure of interfaces. |
| `NestedItems` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[FeedItemInterface.NestedItem](https://wiki.resonite.com/Component:FeedItemInterface#NestedItem "Component:FeedItemInterface")** | A list of extra data feed items to instantiate the same as this one with the same arguments, except each one can be Nested under this item. |
| `EnabledState` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The enabled state of this feed interface item UI element. |
| `Value` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") <T>** | The value field to fill and update from the data feed with. |
| `Format` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field to fill with the format string the source data feed has specified should be used with this value when displaying it. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

## See Also

- [Data Feeds](https://wiki.resonite.com/Data_Feeds "Data Feeds")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FeedIndicatorInterface&oldid=97495](https://wiki.resonite.com/index.php?title=Component:FeedIndicatorInterface&oldid=97495)"

Contents