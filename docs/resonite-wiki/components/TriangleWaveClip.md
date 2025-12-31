# Component:TriangleWaveClip

> Source: https://wiki.resonite.com/Component:TriangleWaveClip

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:TriangleWaveClip&diff=98098) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/4a/TriangleWaveClipComponent.png/510px-TriangleWaveClipComponent.png)](https://wiki.resonite.com/File:TriangleWaveClipComponent.png) **Triangle Wave Clip** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TriangleWaveClip** component is used to make a buzzing like repeating sound clip, which can be used to make audio clips that make a repeating noise.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This component takes time to change it's pitch and loudness when it's properties are changed. When doing real time adjustments, It is recommended to make the audio loud and low pitched by default and then adjust the speed and volume of the audio player to adjust in real time.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `Frequency` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The pitch of the clip. |
| `Amplitude` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The loudness of the clip. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeClip:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Turns the audio into a [Component:StaticAudioClip](https://wiki.resonite.com/Component:StaticAudioClip "Component:StaticAudioClip"). |

Triggers
Collapse

## Usage

Attach to a slot and provide a `Frequency` and `Amplitude`, then insert into a [Component:AudioClipPlayer](https://wiki.resonite.com/Component:AudioClipPlayer "Component:AudioClipPlayer") to hear it.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Type:IAudioSource](https://wiki.resonite.com/Type:IAudioSource "Type:IAudioSource")
- [Component:AudioClipPlayer](https://wiki.resonite.com/Component:AudioClipPlayer "Component:AudioClipPlayer")
- [Component:StaticAudioClip](https://wiki.resonite.com/Component:StaticAudioClip "Component:StaticAudioClip")
- [Component:ChannelVolumeMeter](https://wiki.resonite.com/Component:ChannelVolumeMeter "Component:ChannelVolumeMeter")
- [Component:VolumeMeter](https://wiki.resonite.com/Component:VolumeMeter "Component:VolumeMeter")
- [Component:SawtoothWaveClip](https://wiki.resonite.com/Component:SawtoothWaveClip "Component:SawtoothWaveClip")
- [Component:ValueNoiseClip](https://wiki.resonite.com/Component:ValueNoiseClip "Component:ValueNoiseClip")
- [Component:ButtonAudioClipPlayer](https://wiki.resonite.com/Component:ButtonAudioClipPlayer "Component:ButtonAudioClipPlayer")
- [Component:LerpingMultiClipPlayer](https://wiki.resonite.com/Component:LerpingMultiClipPlayer "Component:LerpingMultiClipPlayer")
- [TalkVisualizer](https://wiki.resonite.com/Component:TalkVisualizer "Component:TalkVisualizer")
- [Component:RandomAudioClipPlayer](https://wiki.resonite.com/Component:RandomAudioClipPlayer "Component:RandomAudioClipPlayer")
- [Component:MultiAudioClipPlayer](https://wiki.resonite.com/Component:MultiAudioClipPlayer "Component:MultiAudioClipPlayer")
- [Component:SimplexNoiseClip](https://wiki.resonite.com/Component:SimplexNoiseClip "Component:SimplexNoiseClip")
- Component:TriangleWaveClip
- [Component:SquareWaveClip](https://wiki.resonite.com/Component:SquareWaveClip "Component:SquareWaveClip")
- [Component:SineWaveClip](https://wiki.resonite.com/Component:SineWaveClip "Component:SineWaveClip")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TriangleWaveClip&oldid=98098](https://wiki.resonite.com/index.php?title=Component:TriangleWaveClip&oldid=98098)"

Contents