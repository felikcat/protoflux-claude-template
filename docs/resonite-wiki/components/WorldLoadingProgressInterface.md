# Component:WorldLoadingProgressInterface

> Source: https://wiki.resonite.com/Component:WorldLoadingProgressInterface

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:WorldLoadingProgressInterface&diff=95856) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/7e/WorldLoadingProgressInterface.png/510px-WorldLoadingProgressInterface.png)](https://wiki.resonite.com/File:WorldLoadingProgressInterface.png) **World Loading Progress Interface** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **WorldLoadingProgressInterface** component is the key component in the creation of a user-definable world loading progress bar. See [Favorites](https://wiki.resonite.com/Favorites "Favorites") for favoritable items like this one.

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
| `Progress` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | Float field where 0.0 - 1.0 progress will be written. |
| `WorldName` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | String field where the loading world's name will be written. |
| `Stage` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [ProgressStage](https://wiki.resonite.com/Type:ProgressStage "Type:ProgressStage") >** | The field to write with the current progress stage of the currently loading world. This is written by the world loading main process. |
| `PhaseName` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | String field where the current loading phase name will be written. |
| `SubPhaseName` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | String field where the current loading sub-phase name will be written. |
| `HasCompleted` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | Boolean field that will be set to true on loading completion. |
| `HasFailed` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | Boolean field that will be set to true on loading failure. |
| `CompletionMessage` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | String field where message indicating completion will be written. |
| `FailureReason` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | String field where message indicating reason for loading failure will be written. |
| `LoadingAssets` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | Boolean field that is set true while loading assets. |
| `LoadedAssets` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | Integer field counting loaded assets. |
| `TotalAssets` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | Integer field counting total assets to be loaded. |
| `LoadedTextures2D` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | Integer field counting loaded ITexture2D assets. |
| `TotalTextures2D` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | Integer field counting total ITexture2D assets to be loaded. |
| `LoadedTextures3D` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | Integer field counting loaded ITexture3D assets. |
| `TotalTextures3D` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | Integer field counting total ITexture3D assets to be loaded. |
| `LoadedCubemaps` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | Integer field counting loaded Cubemap assets. |
| `TotalCubemaps` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | Integer field counting total Cubemap assets to be loaded. |
| `LoadedVideos` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | Integer field counting loaded Video assets. |
| `TotalVideos` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | Integer field counting total Video assets to be loaded. |
| `LoadedMeshes` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | Integer field counting loaded Mesh assets. |
| `TotalMeshes` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | Integer field counting total Mesh assets to be loaded. |
| `LoadedAudioClips` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | Integer field counting loaded Audio assets. |
| `TotalAudioClips` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | Integer field counting total Audio assets to be loaded. |
| `LoadedShaders` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | Integer field counting loaded Shader assets. |
| `TotalShaders` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | Integer field counting total Shader assets to be loaded. |
| `LoadedFonts` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | Integer field counting loaded Font assets. |
| `TotalFonts` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | Integer field counting total Font assets to be loaded. |
| `BytesDownloaded` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Long](https://wiki.resonite.com/Type:Long "Type:Long") >** | Long field counting total bytes downloaded so far. |
| `TotalBytes` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Long](https://wiki.resonite.com/Type:Long "Type:Long") >** | Long field count of total bytes expected to be downloaded. |
| `BytesPerSecond` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Long](https://wiki.resonite.com/Type:Long "Type:Long") >** | Long field indicating current Bytes-per-Second download rate. |
| `ProgressBar` | **[ProgressBarInterface](https://wiki.resonite.com/Component:ProgressBarInterface "Component:ProgressBarInterface")** | Reference to a [Component:ProgressBarInterface](https://wiki.resonite.com/Component:ProgressBarInterface "Component:ProgressBarInterface") component to use as the progress Bae visual. |

Fields
Collapse

## Usage

Use either the existing Resonite world loading bar under [Resonite Essentials](https://wiki.resonite.com/Resonite_Essentials "Resonite Essentials") or make a UI by attaching the component and making one from scratch. Then save the item with this component to the inventory and [favorite](https://wiki.resonite.com/Favorites "Favorites") it so it becomes the default world load indicator upon restarting.

## Examples

The default Resonite world loading bar that is part of the user's default [Favorites](https://wiki.resonite.com/Favorites "Favorites")

## See Also

- [Favorites](https://wiki.resonite.com/Favorites "Favorites")
- Component:WorldLoadingProgressInterface
- [Component:AudioPlayerInterface](https://wiki.resonite.com/Component:AudioPlayerInterface "Component:AudioPlayerInterface")
- [Component:AudioStreamInterface](https://wiki.resonite.com/Component:AudioStreamInterface "Component:AudioStreamInterface")
- [Component:VideoPlayerInterface](https://wiki.resonite.com/Component:VideoPlayerInterface "Component:VideoPlayerInterface")
- [Component:ProgressBarInterface](https://wiki.resonite.com/Component:ProgressBarInterface "Component:ProgressBarInterface")
- [Component:NamePlateInterface](https://wiki.resonite.com/Component:NamePlateInterface "Component:NamePlateInterface")
- [Component:ColorDialogInterface](https://wiki.resonite.com/Component:ColorDialogInterface "Component:ColorDialogInterface")
- [Component:NoticeDisplayInterface](https://wiki.resonite.com/Component:NoticeDisplayInterface "Component:NoticeDisplayInterface")
- [Component:TextDisplayInterface](https://wiki.resonite.com/Component:TextDisplayInterface "Component:TextDisplayInterface")
- [Component:HyperlinkDisplayInterface](https://wiki.resonite.com/Component:HyperlinkDisplayInterface "Component:HyperlinkDisplayInterface")
- [Component:DocumentInterface](https://wiki.resonite.com/Component:DocumentInterface "Component:DocumentInterface")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:WorldLoadingProgressInterface&oldid=95856](https://wiki.resonite.com/index.php?title=Component:WorldLoadingProgressInterface&oldid=95856)"

Contents