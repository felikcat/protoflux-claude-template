# Component:LerpingMultiClipPlayer

> Source: https://wiki.resonite.com/Component:LerpingMultiClipPlayer

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:LerpingMultiClipPlayer&diff=97591) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/39/LerpingMultiClipPlayerComponent.png/510px-LerpingMultiClipPlayerComponent.png)](https://wiki.resonite.com/File:LerpingMultiClipPlayerComponent.png) **Lerping Multi Clip Player** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LerpingMultiClipPlayer** component is an [IAudioSource](https://wiki.resonite.com/Type:IAudioSource "Type:IAudioSource") type that transitions between different audio clips (tracks) by lerping the volume and speed from one audio to the other using `Lerp`.

When an audio is lerped to, the audio will continue to loop till `Lerp` is moved to another clips range.

If `Lerp` is not within a clip range, this component will provide silent audio.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Lerp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The reference value to use to lerp between different tracks with different values. This does not have to be 0-1, and can be any value. |
| `Tracks` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[LerpingMultiClipPlayer.Track](https://wiki.resonite.com/Component:LerpingMultiClipPlayer#Track)** | A list of track's to lerp between using `Lerp`. |

Fields
Collapse

## Track

| Name | Type | Description |
| --- | --- | --- |
| `Clip` | **[AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip")** | The audio clip to play if `Lerp` is within `StartPosition` and `EndPosition`. |
| `StartPosition` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | What the starting point of this track's range is. |
| `EndPosition` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | What the ending point of this track's range is. |
| `StartSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | What the speed should be at the start of this track's range, lerped. |
| `EndSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | What the speed should be at the end of this track's range, lerped. |
| `StartVolumeTransitionRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much of this track's position range to fade the audio in for. |
| `EndVolumeTransitionRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much of this track's position range to fade the audio out for. |

Fields

## Usage

Can be used to make looping noises that play over a video at different positions in the playtime.

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
- Component:LerpingMultiClipPlayer
- [TalkVisualizer](https://wiki.resonite.com/Component:TalkVisualizer "Component:TalkVisualizer")
- [Component:RandomAudioClipPlayer](https://wiki.resonite.com/Component:RandomAudioClipPlayer "Component:RandomAudioClipPlayer")
- [Component:MultiAudioClipPlayer](https://wiki.resonite.com/Component:MultiAudioClipPlayer "Component:MultiAudioClipPlayer")
- [Component:SimplexNoiseClip](https://wiki.resonite.com/Component:SimplexNoiseClip "Component:SimplexNoiseClip")
- [Component:TriangleWaveClip](https://wiki.resonite.com/Component:TriangleWaveClip "Component:TriangleWaveClip")
- [Component:SquareWaveClip](https://wiki.resonite.com/Component:SquareWaveClip "Component:SquareWaveClip")
- [Component:SineWaveClip](https://wiki.resonite.com/Component:SineWaveClip "Component:SineWaveClip")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LerpingMultiClipPlayer&oldid=97591](https://wiki.resonite.com/index.php?title=Component:LerpingMultiClipPlayer&oldid=97591)"

Contents