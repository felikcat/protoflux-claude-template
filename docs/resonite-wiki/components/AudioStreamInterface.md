# Component:AudioStreamInterface

> Source: https://wiki.resonite.com/Component:AudioStreamInterface

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d6/AudioStreamInterfaceComponent.png/510px-AudioStreamInterfaceComponent.png)](https://wiki.resonite.com/File:AudioStreamInterfaceComponent.png) **Audio Stream Interface** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AudioStreamInterface** component is used on AudioStream objects that are spawned in by the user via the dash to allow the engine to interface with the stored audio stream.

This is a favorite-able item. See [Favorites](https://wiki.resonite.com/Favorites "Favorites").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ItemName` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The name of the stream like Frooxius's Stream |
| `SpawningUser` | **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user that spawned the stream |
| `SpawningUserID` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The userid field of the `SpawningUser` |
| `IsInstance` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this interface is being edited or is part of a spawned audio stream. |
| `Source` | **[SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") < [IAudioStream](https://wiki.resonite.com/index.php?title=Type:IAudioStream&action=edit&redlink=1 "Type:IAudioStream (page does not exist)") >** | The audio stream this interfaces with |
| `Bitrate` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | The Bitrate setting of the spawned audiostream interface (like a UIX) |
| `Volume` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The Volume slider/setting of the spawned audio stream interface (like a UIX) |
| `Spatialize` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The Spatialize setting of the spawned audio stream interface (like a UIX) |

Fields
Collapse

## Usage

Can be used to make your own audio stream player interface as an inventory favorite

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Favorites](https://wiki.resonite.com/Favorites "Favorites")
- [Component:WorldLoadingProgressInterface](https://wiki.resonite.com/Component:WorldLoadingProgressInterface "Component:WorldLoadingProgressInterface")
- [Component:AudioPlayerInterface](https://wiki.resonite.com/Component:AudioPlayerInterface "Component:AudioPlayerInterface")
- Component:AudioStreamInterface
- [Component:VideoPlayerInterface](https://wiki.resonite.com/Component:VideoPlayerInterface "Component:VideoPlayerInterface")
- [Component:ProgressBarInterface](https://wiki.resonite.com/Component:ProgressBarInterface "Component:ProgressBarInterface")
- [Component:NamePlateInterface](https://wiki.resonite.com/Component:NamePlateInterface "Component:NamePlateInterface")
- [Component:ColorDialogInterface](https://wiki.resonite.com/Component:ColorDialogInterface "Component:ColorDialogInterface")
- [Component:NoticeDisplayInterface](https://wiki.resonite.com/Component:NoticeDisplayInterface "Component:NoticeDisplayInterface")
- [Component:TextDisplayInterface](https://wiki.resonite.com/Component:TextDisplayInterface "Component:TextDisplayInterface")
- [Component:HyperlinkDisplayInterface](https://wiki.resonite.com/Component:HyperlinkDisplayInterface "Component:HyperlinkDisplayInterface")
- [Component:DocumentInterface](https://wiki.resonite.com/Component:DocumentInterface "Component:DocumentInterface")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AudioStreamInterface&oldid=93992](https://wiki.resonite.com/index.php?title=Component:AudioStreamInterface&oldid=93992)"

Contents