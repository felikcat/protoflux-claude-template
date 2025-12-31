# Component:ChannelVolumeMeter

> Source: https://wiki.resonite.com/Component:ChannelVolumeMeter

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/bb/ChannelVolumeMeterComponent.png/510px-ChannelVolumeMeterComponent.png)](https://wiki.resonite.com/File:ChannelVolumeMeterComponent.png) **Channel Volume Meter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Channel Volume meter is a component that is used to read the volume of an audio source with multiple channels. The amount of channels can vary from 1, 2, and even to beyond 4. Usually this component is used to split the Left and Right audio volumes of an `.OGG` clip.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Smoothing` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to smooth the value changes of the outputs in `ChannelVolumes` |
| `Power` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Raise `ChannelVolumes` to this exponent. 1 will leave `ChannelVolumes` unchanged. |
| `Method` | **[VolumeMeterMethod](https://wiki.resonite.com/Type:VolumeMeterMethod "Type:VolumeMeterMethod")** | Whether the outputted value should be the current volume, or the change in volume over time (delta) |
| `Source` | **[IAudioSource](https://wiki.resonite.com/Type:IAudioSource "Type:IAudioSource")** | The source to read the audio volumes for each channel from. |
| `CurrentChannels` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many channels `Source` has. |
| `ChannelVolumes` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[RawOutput\`1](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The output volumes of each channel `Source` has. |
| `DoNotRemoveExcessFields` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Don't remove excess fields whenever a new audio clip is inserted and the fields are outside the amount of channels the audio clip has. |

Fields
Collapse

## Usage

## Examples

This can be used for audio visualizers, or to read the individual volume of the left and right volume of an OGG for L and R speaker visualization.

## See Also

- [Type:IAudioSource](https://wiki.resonite.com/Type:IAudioSource "Type:IAudioSource")
- [Component:AudioClipPlayer](https://wiki.resonite.com/Component:AudioClipPlayer "Component:AudioClipPlayer")
- [Component:StaticAudioClip](https://wiki.resonite.com/Component:StaticAudioClip "Component:StaticAudioClip")
- Component:ChannelVolumeMeter
- [Component:VolumeMeter](https://wiki.resonite.com/Component:VolumeMeter "Component:VolumeMeter")
- [Component:SawtoothWaveClip](https://wiki.resonite.com/Component:SawtoothWaveClip "Component:SawtoothWaveClip")
- [Component:ValueNoiseClip](https://wiki.resonite.com/Component:ValueNoiseClip "Component:ValueNoiseClip")
- [Component:ButtonAudioClipPlayer](https://wiki.resonite.com/Component:ButtonAudioClipPlayer "Component:ButtonAudioClipPlayer")
- [Component:LerpingMultiClipPlayer](https://wiki.resonite.com/Component:LerpingMultiClipPlayer "Component:LerpingMultiClipPlayer")
- [TalkVisualizer](https://wiki.resonite.com/Component:TalkVisualizer "Component:TalkVisualizer")
- [Component:RandomAudioClipPlayer](https://wiki.resonite.com/Component:RandomAudioClipPlayer "Component:RandomAudioClipPlayer")
- [Component:MultiAudioClipPlayer](https://wiki.resonite.com/Component:MultiAudioClipPlayer "Component:MultiAudioClipPlayer")
- [Component:SimplexNoiseClip](https://wiki.resonite.com/Component:SimplexNoiseClip "Component:SimplexNoiseClip")
- [Component:TriangleWaveClip](https://wiki.resonite.com/Component:TriangleWaveClip "Component:TriangleWaveClip")
- [Component:SquareWaveClip](https://wiki.resonite.com/Component:SquareWaveClip "Component:SquareWaveClip")
- [Component:SineWaveClip](https://wiki.resonite.com/Component:SineWaveClip "Component:SineWaveClip")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ChannelVolumeMeter&oldid=95619](https://wiki.resonite.com/index.php?title=Component:ChannelVolumeMeter&oldid=95619)"

Contents