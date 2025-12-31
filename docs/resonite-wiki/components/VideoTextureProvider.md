# Component:VideoTextureProvider

> Source: https://wiki.resonite.com/Component:VideoTextureProvider

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:VideoTextureProvider&diff=100808) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/5d/VideoTextureProviderComponent.png/510px-VideoTextureProviderComponent.png)](https://wiki.resonite.com/File:VideoTextureProviderComponent.png) **Video Texture Provider** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **VideoTextureProvider** component is used to display and play video. This component importantly implements both [ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D") and [IAudioSource](https://wiki.resonite.com/Type:IAudioSource "Type:IAudioSource") which means it can be used as both a texture and a source of audio like a [StaticAudioClip](https://wiki.resonite.com/Component:StaticAudioClip "Component:StaticAudioClip")

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Playback` | _direct_ **[SyncPlayback](https://wiki.resonite.com/Type:SyncPlayback "Type:SyncPlayback")** | controls the playback of both the audio and visual elements of this component at the same time. |
| `URL` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The website or file source of the video. Like a youtube video or a file on a machine. |
| `Stream` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this video should stream the data or cache it |
| `Volume` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The volume of the video when being used as an [IAudioSource](https://wiki.resonite.com/Type:IAudioSource "Type:IAudioSource") in an audio player. |
| `ForcePlaybackEngine` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The engine to use for playback like UnityPlaybackEngine or LibVLC. |
| `ForceVideoStreamingServiceParsing` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to force parsing a streaming service like Twitch. |
| `VideoTitle` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The field to populate with the name of the video that has been loaded. |
| `CurrentPlaybackEngine` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The current engine being used for playback |
| `CurrentClockError` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount of seconds the player may have in error due to lag or otherwise. |
| `FilterMode` | **[TextureFilterMode](https://wiki.resonite.com/Type:TextureFilterMode "Type:TextureFilterMode")** | How to handle the interpolation between pixels. |
| `AnisotropicLevel` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The levels of Anisotropic filtering distances when using Anisotropic for `FilterMode` |
| `WrapModeU` | **[TextureWrapMode](https://wiki.resonite.com/Type:TextureWrapMode "Type:TextureWrapMode")** | How to repeat or mirror the texture along the X axis. this goes into affect when X values are outside of the range \[0.0 to 1.0\]. |
| `WrapModeV` | **[TextureWrapMode](https://wiki.resonite.com/Type:TextureWrapMode "Type:TextureWrapMode")** | How to repeat or mirror the texture along the Y axis. this goes into affect when Y values are outside of the range \[0.0 to 1.0\]. |
| `AudioTrackIndex` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | the audio track that the video player should use to play |
| `PreferAudioOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether to parse the video source as audio only rather than video and audio. An example of an audio only is an MP3 file type. |
| `MaxWidth` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | The max pixels on the x axis that will be rendered when using this as a texture. |
| `MaxHeight` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | The max pixels on the y axis that will be rendered when using this as a texture. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `UseAutomatic:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Switches the playback engine to automatic. |
| `UseUnityNative:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Switches the playback engine to Unity's native library for playing videos. |
| `UseLibVLC:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Switches the playback engine to Library video library codec. |

Triggers
Collapse

## Usage

This component is often seen with [Video Players](https://wiki.resonite.com/Video_Player "Video Player"), as they implement [ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D") (meaning they are also a texture) and also implement IAudioSource (Which mean that are also like an audio clip) and can be used by users in different ways (i.e. Multiple screens and speakers sharing one Video Player texture).

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:PlaybackSynchronizer](https://wiki.resonite.com/Component:PlaybackSynchronizer "Component:PlaybackSynchronizer") for synchronizing playables
- [Video\_Player](https://wiki.resonite.com/Video_Player "Video Player") for a user friendly article

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VideoTextureProvider&oldid=100808](https://wiki.resonite.com/index.php?title=Component:VideoTextureProvider&oldid=100808)"

Contents