# Component:VideoPlayerInterface

> Source: https://wiki.resonite.com/Component:VideoPlayerInterface

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/35/VideoPlayerInterfaceComponent.png/510px-VideoPlayerInterfaceComponent.png)](https://wiki.resonite.com/File:VideoPlayerInterfaceComponent.png) **Video Player Interface** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **VideoPlayerInterface** component is a [favoritable](https://wiki.resonite.com/Favorites "Favorites") item that is used to specify the UI elements of a custom [Video Player](https://wiki.resonite.com/Video_Player "Video Player").

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
| `URL` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Uri](https://wiki.resonite.com/Type:Uri "Type:Uri") >** | The field to fill with the URL of the imported video asset. |
| `Stream` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The field to fill with whether this video player is showing stream. |
| `VideoClip` | **[AssetRef\`1](https://wiki.resonite.com/index.php?title=Type:AssetRef%601&action=edit&redlink=1 "Type:AssetRef`1 (page does not exist)") < [VideoTexture](https://wiki.resonite.com/Type:VideoTexture "Type:VideoTexture") >** | The field to fill with what the video being displayed is. |
| `VideoClipTexture` | **[AssetRef\`1](https://wiki.resonite.com/index.php?title=Type:AssetRef%601&action=edit&redlink=1 "Type:AssetRef`1 (page does not exist)") < [ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D") >** | The field to fill (Usually a material texture field) with the showing video texture. |
| `AspectRatio` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The field to fill with what the video's aspect ratio is. |
| `DefaultVideoClip` | **[VideoTexture](https://wiki.resonite.com/Type:VideoTexture "Type:VideoTexture")** | The default video texture to use if one isn't filled in. |
| `StereoRenderingEnabled` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The field to fill with whether the video is a stero video (3D) |
| `StereoLayout` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [StereoLayout](https://wiki.resonite.com/Type:StereoLayout "Type:StereoLayout") >** | The field to fill with the kind of stero image layout the image has. |
| `StereoTransformLeft` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float4](https://wiki.resonite.com/Type:Float4 "Type:Float4") >** | The field to fill with what the rectangle area for the left eye should be. |
| `StereoTransformRight` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float4](https://wiki.resonite.com/Type:Float4 "Type:Float4") >** | The field to fill with what the rectangle area for the right eye should be. |
| `StereoTransformScaleLeft` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2") >** | The field to fill with what the UV scale for the left eye should be. |
| `StereoTransformOffsetLeft` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2") >** | The field to fill with what the UV offset for the left eye should be. |
| `StereoTransformScaleRight` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2") >** | The field to fill with what the UV scale for the right eye should be. |
| `StereoTransformOffsetRight` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2") >** | The field to fill with what the UV offset for the right eye should be. |
| `PanoramicRenderingEnabled` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The field to fill with whether the video is a 360 video |
| `PanoramicHorizontalFOV` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The field to fill with the video's horizontal 360 video FOV. |
| `PanoramicVerticalFOV` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The field to fill with the video's vertical 360 video FOV. |
| `PanoramicProjection` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [PanoramicProjection](https://wiki.resonite.com/Type:PanoramicProjection "Type:PanoramicProjection") >** | The field to fill with what the video's panoramic texture arrangement is. |

Fields
Collapse

## Usage

Use either the existing Resonite video player under [Resonite Essentials](https://wiki.resonite.com/Resonite_Essentials "Resonite Essentials") or make a UI by attaching the component and making one from scratch. Then save the item with this component to the inventory and [favorite](https://wiki.resonite.com/Favorites "Favorites") it so it becomes the default player upon restarting.

## Examples

The default Resonite player that is part of the user's default [Favorites](https://wiki.resonite.com/Favorites "Favorites")

## See Also

- [Favorites](https://wiki.resonite.com/Favorites "Favorites")
- [Component:WorldLoadingProgressInterface](https://wiki.resonite.com/Component:WorldLoadingProgressInterface "Component:WorldLoadingProgressInterface")
- [Component:AudioPlayerInterface](https://wiki.resonite.com/Component:AudioPlayerInterface "Component:AudioPlayerInterface")
- [Component:AudioStreamInterface](https://wiki.resonite.com/Component:AudioStreamInterface "Component:AudioStreamInterface")
- Component:VideoPlayerInterface
- [Component:ProgressBarInterface](https://wiki.resonite.com/Component:ProgressBarInterface "Component:ProgressBarInterface")
- [Component:NamePlateInterface](https://wiki.resonite.com/Component:NamePlateInterface "Component:NamePlateInterface")
- [Component:ColorDialogInterface](https://wiki.resonite.com/Component:ColorDialogInterface "Component:ColorDialogInterface")
- [Component:NoticeDisplayInterface](https://wiki.resonite.com/Component:NoticeDisplayInterface "Component:NoticeDisplayInterface")
- [Component:TextDisplayInterface](https://wiki.resonite.com/Component:TextDisplayInterface "Component:TextDisplayInterface")
- [Component:HyperlinkDisplayInterface](https://wiki.resonite.com/Component:HyperlinkDisplayInterface "Component:HyperlinkDisplayInterface")
- [Component:DocumentInterface](https://wiki.resonite.com/Component:DocumentInterface "Component:DocumentInterface")
- [Video Player](https://wiki.resonite.com/Video_Player "Video Player")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VideoPlayerInterface&oldid=95841](https://wiki.resonite.com/index.php?title=Component:VideoPlayerInterface&oldid=95841)"

Contents