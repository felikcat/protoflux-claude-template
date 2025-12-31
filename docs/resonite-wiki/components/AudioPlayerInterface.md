# Component:AudioPlayerInterface

> Source: https://wiki.resonite.com/Component:AudioPlayerInterface

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a5/AudioPlayerInterfaceComponent.png/510px-AudioPlayerInterfaceComponent.png)](https://wiki.resonite.com/File:AudioPlayerInterfaceComponent.png) **Audio Player Interface** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AudioPlayerInterface** component is used on AudioClip objects that are spawned in by the user to allow the engine to interface with the stored audio clip.

This is a favorite-able item. See [Favorites](https://wiki.resonite.com/Favorites "Favorites").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ItemName` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The name of the audio clip. |
| `SpawningUser` | **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user that spawned this audio clip. |
| `SpawningUserID` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | The field of the UserRef that stores the spawning user's id. |
| `IsInstance` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this audio clip interface is a spawned interface or one being edited currently by the user. Usually set to true by the game when loaded as a user's favorite audio clip player |
| `URL` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Uri](https://wiki.resonite.com/Type:Uri "Type:Uri") >** | The field of the URI on the [Type:AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip") this component interfaces with. |
| `Clip` | **[AssetRef\`1](https://wiki.resonite.com/index.php?title=Type:AssetRef%601&action=edit&redlink=1 "Type:AssetRef`1 (page does not exist)") < [AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip") >** | The [Type:AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip") interfaced by this component. |
| `Group` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [AudioTypeGroup](https://wiki.resonite.com/Type:AudioTypeGroup "Type:AudioTypeGroup") >** | The audio group setting for this audio clip. |
| `Volume` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The volume setting of this audio clip. |
| `Spatialize` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The Spatialize setting of the audio clip. |
| `Doppler` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The Doppler setting of the audio clip. |
| `DefaultAudioClip` | **[AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip")** | The audio clip |

Fields
Collapse

## Usage

This can be attached to a slot in order for the user to make own audio clip interface for when they import an audio clip. Although, it may be easier to edit the default existing audio clip player interface.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Favorites](https://wiki.resonite.com/Favorites "Favorites")
- [Component:WorldLoadingProgressInterface](https://wiki.resonite.com/Component:WorldLoadingProgressInterface "Component:WorldLoadingProgressInterface")
- Component:AudioPlayerInterface
- [Component:AudioStreamInterface](https://wiki.resonite.com/Component:AudioStreamInterface "Component:AudioStreamInterface")
- [Component:VideoPlayerInterface](https://wiki.resonite.com/Component:VideoPlayerInterface "Component:VideoPlayerInterface")
- [Component:ProgressBarInterface](https://wiki.resonite.com/Component:ProgressBarInterface "Component:ProgressBarInterface")
- [Component:NamePlateInterface](https://wiki.resonite.com/Component:NamePlateInterface "Component:NamePlateInterface")
- [Component:ColorDialogInterface](https://wiki.resonite.com/Component:ColorDialogInterface "Component:ColorDialogInterface")
- [Component:NoticeDisplayInterface](https://wiki.resonite.com/Component:NoticeDisplayInterface "Component:NoticeDisplayInterface")
- [Component:TextDisplayInterface](https://wiki.resonite.com/Component:TextDisplayInterface "Component:TextDisplayInterface")
- [Component:HyperlinkDisplayInterface](https://wiki.resonite.com/Component:HyperlinkDisplayInterface "Component:HyperlinkDisplayInterface")
- [Component:DocumentInterface](https://wiki.resonite.com/Component:DocumentInterface "Component:DocumentInterface")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AudioPlayerInterface&oldid=93991](https://wiki.resonite.com/index.php?title=Component:AudioPlayerInterface&oldid=93991)"

Contents