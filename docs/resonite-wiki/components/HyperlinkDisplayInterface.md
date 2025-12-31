# Component:HyperlinkDisplayInterface

> Source: https://wiki.resonite.com/Component:HyperlinkDisplayInterface

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2b/HyperlinkDisplayInterfaceComponent.png/510px-HyperlinkDisplayInterfaceComponent.png)](https://wiki.resonite.com/File:HyperlinkDisplayInterfaceComponent.png) **Hyperlink Display Interface** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **HyperlinkDisplayInterface** component is spawned by the favorites system when a user pastes a link that is recognized as a website link rather than a specific media type.

See [Favorites](https://wiki.resonite.com/Favorites "Favorites") on favoritable items like this one.

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
| `Url` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Uri](https://wiki.resonite.com/Type:Uri "Type:Uri") >** | The field to fill with the URL this hyperlink display should leas to. |
| `UrlString` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field to fill with the URL as a string so the hyperlink display can show what it leads to. |

Fields
Collapse

## Usage

This component can be made part of a UI that can be modified and favorited to become the user's default hyperlink spawning UI.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

- needs an image of the default spawned link that spawns when users paste website links.

## See Also

- [Favorites](https://wiki.resonite.com/Favorites "Favorites")
- [Component:WorldLoadingProgressInterface](https://wiki.resonite.com/Component:WorldLoadingProgressInterface "Component:WorldLoadingProgressInterface")
- [Component:AudioPlayerInterface](https://wiki.resonite.com/Component:AudioPlayerInterface "Component:AudioPlayerInterface")
- [Component:AudioStreamInterface](https://wiki.resonite.com/Component:AudioStreamInterface "Component:AudioStreamInterface")
- [Component:VideoPlayerInterface](https://wiki.resonite.com/Component:VideoPlayerInterface "Component:VideoPlayerInterface")
- [Component:ProgressBarInterface](https://wiki.resonite.com/Component:ProgressBarInterface "Component:ProgressBarInterface")
- [Component:NamePlateInterface](https://wiki.resonite.com/Component:NamePlateInterface "Component:NamePlateInterface")
- [Component:ColorDialogInterface](https://wiki.resonite.com/Component:ColorDialogInterface "Component:ColorDialogInterface")
- [Component:NoticeDisplayInterface](https://wiki.resonite.com/Component:NoticeDisplayInterface "Component:NoticeDisplayInterface")
- [Component:TextDisplayInterface](https://wiki.resonite.com/Component:TextDisplayInterface "Component:TextDisplayInterface")
- Component:HyperlinkDisplayInterface
- [Component:DocumentInterface](https://wiki.resonite.com/Component:DocumentInterface "Component:DocumentInterface")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:HyperlinkDisplayInterface&oldid=94792](https://wiki.resonite.com/index.php?title=Component:HyperlinkDisplayInterface&oldid=94792)"

Contents