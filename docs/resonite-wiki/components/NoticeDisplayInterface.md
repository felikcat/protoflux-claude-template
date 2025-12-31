# Component:NoticeDisplayInterface

> Source: https://wiki.resonite.com/Component:NoticeDisplayInterface

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/89/NoticeDisplayInterfaceComponent.png/510px-NoticeDisplayInterfaceComponent.png)](https://wiki.resonite.com/File:NoticeDisplayInterfaceComponent.png) **Notice Display Interface** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **NoticeDisplayInterface** component allows the user to make custom notification dialogues or notification banners by saving this component as part of an item's root and then setting it as the user's notification interface.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This component isn't fully implemented yet.


This is a favoriteable item. For more info, see [Favorites](https://wiki.resonite.com/Favorites "Favorites").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ItemName` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The name of this favoritable item. |
| `SpawningUser` | **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user that spawned this favoritable item. |
| `SpawningUserID` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field containing the ID of the user that spawned this favoritable item. |
| `IsInstance` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this item is an instance. |
| `Heading` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field to populate with what the notification header should be. |
| `Icon` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Uri](https://wiki.resonite.com/Type:Uri "Type:Uri") >** | The field to populate with what the icon url should be for the notification. |
| `Text` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field to populate with the notification text. |
| `Color` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Color](https://wiki.resonite.com/Type:Color "Type:Color") >** | The field to populate with the color that the notification should be. |

Fields
Collapse

## Usage

Attach to a slot and set up with a UI to display and use it's various fields. Upon saving, favoriting, and restarting the game, notifications will take on the new UI's appearance and behavior.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Favorites](https://wiki.resonite.com/Favorites "Favorites")
- [Component:WorldLoadingProgressInterface](https://wiki.resonite.com/Component:WorldLoadingProgressInterface "Component:WorldLoadingProgressInterface")
- [Component:AudioPlayerInterface](https://wiki.resonite.com/Component:AudioPlayerInterface "Component:AudioPlayerInterface")
- [Component:AudioStreamInterface](https://wiki.resonite.com/Component:AudioStreamInterface "Component:AudioStreamInterface")
- [Component:VideoPlayerInterface](https://wiki.resonite.com/Component:VideoPlayerInterface "Component:VideoPlayerInterface")
- [Component:ProgressBarInterface](https://wiki.resonite.com/Component:ProgressBarInterface "Component:ProgressBarInterface")
- [Component:NamePlateInterface](https://wiki.resonite.com/Component:NamePlateInterface "Component:NamePlateInterface")
- [Component:ColorDialogInterface](https://wiki.resonite.com/Component:ColorDialogInterface "Component:ColorDialogInterface")
- Component:NoticeDisplayInterface
- [Component:TextDisplayInterface](https://wiki.resonite.com/Component:TextDisplayInterface "Component:TextDisplayInterface")
- [Component:HyperlinkDisplayInterface](https://wiki.resonite.com/Component:HyperlinkDisplayInterface "Component:HyperlinkDisplayInterface")
- [Component:DocumentInterface](https://wiki.resonite.com/Component:DocumentInterface "Component:DocumentInterface")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:NoticeDisplayInterface&oldid=95250](https://wiki.resonite.com/index.php?title=Component:NoticeDisplayInterface&oldid=95250)"

Contents