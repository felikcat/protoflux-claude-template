# Component:LegacyVideoPlayer

> Source: https://wiki.resonite.com/Component:LegacyVideoPlayer

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/4a/LegacyVideoPlayerComponent.png/510px-LegacyVideoPlayerComponent.png)](https://wiki.resonite.com/File:LegacyVideoPlayerComponent.png) **Legacy Video Player** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Legacy Video Player** component is used to construct and control legacy video players.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `StereoLayout` | **[StereoLayout](https://wiki.resonite.com/Type:StereoLayout "Type:StereoLayout")** | The layout of the stereo audio for the video player. |
| `SizeCompensation` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How to compensate for video size. |
| `videoProvider` | **[VideoTexture](https://wiki.resonite.com/Type:VideoTexture "Type:VideoTexture")** | The video provider component giving the audio and visual data for the video. |
| `_style` | **[LegacyUIStyle](https://wiki.resonite.com/Component:LegacyUIStyle "Component:LegacyUIStyle")** | The legacy ui style component being used for this video player. |
| `_indicatorTextureUrl` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The field to drive to control the video player's texture url |
| `_indicatorTint` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The field to drive to control the video player's indictor's tint |
| `_colliderSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive to control the video player's collider size |
| `_frameWidth` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive to control the video player's border frame width |
| `_frameHeight` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive to control the video player's border frame height |
| `_frameMaterial` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[PBS\_RimMetallic](https://wiki.resonite.com/PBS_RimMetallic "PBS RimMetallic")** | The field to drive to control the video player's frame material |
| `_displayMaterial` | **[UnlitMaterial](https://wiki.resonite.com/Component:UnlitMaterial "Component:UnlitMaterial")** | This stores the video player's display material. |
| `_displayMaterialTexture` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[AssetRef\`1](https://wiki.resonite.com/index.php?title=Type:AssetRef%601&action=edit&redlink=1 "Type:AssetRef`1 (page does not exist)") < [ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D") >** | The field to drive to control the video player's display material texture. |
| `_displaySize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The field to drive to control the video player's display section size. |
| `_mainAudioOutput` | **[AudioOutput](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput")** | This stores the video player's main audio output. |
| `_timelineSlider` | **[LegacySlider](https://wiki.resonite.com/Component:LegacySlider "Component:LegacySlider")** | This stores the video player's timeline slider. |
| `_timelinePosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive to control the video player's timeline playhead position. |
| `_timelineWidth` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive to control the video player's timeline ui width. |
| `_positionDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive to control the video player's ui position. |
| `_volumeSlider` | **[LegacySlider](https://wiki.resonite.com/Component:LegacySlider "Component:LegacySlider")** | This stores the video player's volume slider. |
| `_volumePosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive to control the video player's volume amount. |
| `_volumeWidth` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive to control the video player's volume ui width. |
| `_volumeDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive to control the video player's volume for the audio output component. |
| `_buttonsWidth` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive to control the video player's button container widths. |
| `_buttonsHeight` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive to control the video player's button container height. |
| `_buttonsPosition` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive to control the video player's button container position. |
| `_playButtonColor` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The field to drive to control the video player's play button color. |
| `_pauseButtonColor` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The field to drive to control the video player's pause button color. |
| `_stopButtonColor` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The field to drive to control the video player's stop button color. |
| `_loopButtonColor` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The field to drive to control the video player's loop button color. |
| `_audio3DButtonColor` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The field to drive to control the video player's 3d audio button. |
| `_exportable` | **[VideoExportable](https://wiki.resonite.com/Component:VideoExportable "Component:VideoExportable")** | The component that is used to make this video player exportable. |
| `_assetProxy` | **[AssetProxy\`1](https://wiki.resonite.com/Component:AssetProxy%601 "Component:AssetProxy`1") < [VideoTexture](https://wiki.resonite.com/Type:VideoTexture "Type:VideoTexture") >** | The component that is used to allow this video to be dropped into asset fields for videos. |
| `_referenceProxy` | **[ReferenceProxy](https://wiki.resonite.com/Component:ReferenceProxy "Component:ReferenceProxy")** | The component that allows this video to be dropped into texture and audio fields or receivers. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnIndicatorTouched:TouchEvent` | **[TouchEvent](https://wiki.resonite.com/index.php?title=Type:TouchEvent&action=edit&redlink=1 "Type:TouchEvent (page does not exist)")** | ✓ | Called when the indicator button is touched. |
| `OnPlayTouched:TouchEvent` | **[TouchEvent](https://wiki.resonite.com/index.php?title=Type:TouchEvent&action=edit&redlink=1 "Type:TouchEvent (page does not exist)")** | ✓ | Called when the play button is touched. |
| `OnPauseTouched:TouchEvent` | **[TouchEvent](https://wiki.resonite.com/index.php?title=Type:TouchEvent&action=edit&redlink=1 "Type:TouchEvent (page does not exist)")** | ✓ | Called when the pause button is touched. |
| `OnStopTouched:TouchEvent` | **[TouchEvent](https://wiki.resonite.com/index.php?title=Type:TouchEvent&action=edit&redlink=1 "Type:TouchEvent (page does not exist)")** | ✓ | Called when the stop button is touched. |
| `OnLoopTouched:TouchEvent` | **[TouchEvent](https://wiki.resonite.com/index.php?title=Type:TouchEvent&action=edit&redlink=1 "Type:TouchEvent (page does not exist)")** | ✓ | Called when the loop button is touched. |
| `OnAudio3DTouched:TouchEvent` | **[TouchEvent](https://wiki.resonite.com/index.php?title=Type:TouchEvent&action=edit&redlink=1 "Type:TouchEvent (page does not exist)")** | ✓ | Called when the spatialize audio button is touched. |
| ``VolumeUp:Action`1<LegacySlider>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [LegacySlider](https://wiki.resonite.com/Component:LegacySlider "Component:LegacySlider") >** | ✓ | Called when the volume up button is touched. |
| ``VolumeDown:Action`1<LegacySlider>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [LegacySlider](https://wiki.resonite.com/Component:LegacySlider "Component:LegacySlider") >** | ✓ | Called when the volume down button is touched. |
| ``FastForward:Action`1<LegacySlider>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [LegacySlider](https://wiki.resonite.com/Component:LegacySlider "Component:LegacySlider") >** | ✓ | Called when the fast forward button is touched. |
| ``FastBackward:Action`1<LegacySlider>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [LegacySlider](https://wiki.resonite.com/Component:LegacySlider "Component:LegacySlider") >** | ✓ | Called when the fast backwards button is touched. |

Triggers
Collapse

## Usage

Used in legacy content. do not use in new content.

## Examples

used in legacy content.

## See Also

- [Video Player](https://wiki.resonite.com/Video_Player "Video Player")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyVideoPlayer&oldid=103802](https://wiki.resonite.com/index.php?title=Component:LegacyVideoPlayer&oldid=103802)"

Contents