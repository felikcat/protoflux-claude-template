# Component:AudioClipAssetMetadata

> Source: https://wiki.resonite.com/Component:AudioClipAssetMetadata

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AudioClipAssetMetadata&diff=92149) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/9f/AudioClipAssetMetadataComponent.png/510px-AudioClipAssetMetadataComponent.png)](https://wiki.resonite.com/File:AudioClipAssetMetadataComponent.png) **Audio Clip Asset Metadata** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Audio Clip Asset Metadata is a component that will populate itself with different small bits of information about an audio clip, also known as metadata.
The metadata will be the default values until an audio clip is provided, which will then populate the data.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AudioClip` | **[AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip")** | The audio clip to read metadata from |
| `SampleRate` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The Hz the audio is sampled at. |
| `Channels` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[ChannelConfiguration](https://wiki.resonite.com/index.php?title=Type:ChannelConfiguration&action=edit&redlink=1 "Type:ChannelConfiguration (page does not exist)")** | The audio channel configuration the audio was recorded in. |
| `ChannelCount` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many channels are in the audio recording. usually 1 channel for mono or 2 channels for L and R Stereo. |
| `SampleCount` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | how many total samples the audio clip has |
| `Duration` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Double](https://wiki.resonite.com/Type:Double "Type:Double")** | How long the audio clip is in seconds. |
| `Extension` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | the extension of the file type the audio was recorded in. |
| `CodecInfo` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The codec the audio is written in like WAV or FLAC and the quality of the audio. |
| `FullyDecoded` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If the audio is loaded or not and decoded (Waveform visible) |

Fields
Collapse

## Usage

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AudioClipAssetMetadata&oldid=92149](https://wiki.resonite.com/index.php?title=Component:AudioClipAssetMetadata&oldid=92149)"

Contents