# Component:FeedItemInterface

> Source: https://wiki.resonite.com/Component:FeedItemInterface

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e4/FeedItemInterfaceComponent.png/510px-FeedItemInterfaceComponent.png)](https://wiki.resonite.com/File:FeedItemInterfaceComponent.png) **Feed Item Interface** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **FeedItemInterface** component is used as a template type item in data feed mappers in the [Data Feeds](https://wiki.resonite.com/Data_Feeds "Data Feeds") system.

All Feed interface types extend from this class, and are listed in the [Interfaces category](https://wiki.resonite.com/Category:Components:Radiant_UI:Data_Feeds:Interfaces "Category:Components:Radiant UI:Data Feeds:Interfaces").

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
| `ParentContainer` | **FeedItemInterface** | This template's parent container. If that template also has a parent and a child, then it recursively goes up the containers till it finds the root interface with a parent and a child interface, then instantiates that interfaces child interface and it's Nested items instead of just this interface. |
| `ChildContainer` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | This template's child template which it instanciates if it's part of a parent child structure of interfaces. |
| `NestedItems` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[FeedItemInterface.NestedItem](https://wiki.resonite.com/Component:FeedItemInterface#NestedItem)** | A list of extra data feed items to instantiate the same as this one with the same arguments, except each one can be Nested under this item. |
| `EnabledState` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The enabled state of this feed interface item UI element. |

Fields
Collapse

## NestedItem

| Name | Type | Description |
| --- | --- | --- |
| `Interface` | **FeedItemInterface** | The template to instance when templated by a data feed as part of this Nested item. |
| `Container` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Where to place this Nested item when it is generated. |
| `IgnoreParentContainer` | **[bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to ignore instantiating the parent container of `Interface` when this is instanciated. |

Fields

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

## See Also

- [Data Feeds](https://wiki.resonite.com/Data_Feeds "Data Feeds")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FeedItemInterface&oldid=97496](https://wiki.resonite.com/index.php?title=Component:FeedItemInterface&oldid=97496)"

Contents