# Component:MultiAudioClipPlayer

> Source: https://wiki.resonite.com/Component:MultiAudioClipPlayer

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:MultiAudioClipPlayer&diff=98002) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/61/MultiAudioClipPlayerComponent.png/510px-MultiAudioClipPlayerComponent.png)](https://wiki.resonite.com/File:MultiAudioClipPlayerComponent.png) **Multi Audio Clip Player** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

TODO: instead of being written by [me](https://wiki.resonite.com/User:989onan "User:989onan") with 2 brain cells of math this should be rewritten with actual math terms.

The MultiAudioClipPlayer is a component able to make a group of audios play at the exact same time with a timeline. How the math is determined is made by taking each track and checking their play length in seconds. Next a math equation is done to find how much to repeat each Audio Clip by, so they end at the same time. Then it makes this component's playback length where all the audio clips would end. This could be used as a way of doing said math equation.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `playback` | _direct_ **[SyncPlayback](https://wiki.resonite.com/Type:SyncPlayback "Type:SyncPlayback")** | the position of the multi audio clip player |
| `Tracks` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[MultiAudioClipPlayer.Track](https://wiki.resonite.com/Component:MultiAudioClipPlayer#Track)** | the different tracks this Multi Audio Clip is playing. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `Play:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Starts playback of the audio clips |
| `Stop:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Stops playback of the audio clips and sets playhead back to beginning. |
| `Pause:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Pauses playback of the audio clips. |
| `Resume:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Resumes playback of the audio clips at current position. |

Triggers
Collapse

## Usage

Add a group of tracks to the tracks list to make them part of the player. The player can be referenced by [Type:IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable") capable nodes such as [Media ProtoFlux Nodes](https://wiki.resonite.com/Category:ProtoFlux:Media "Category:ProtoFlux:Media") and Components that take such. This component can also be put into an [Audio Output Component](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput") to be heard by the user.

## Track

| Name | Type | Description |
| --- | --- | --- |
| `Clip` | **[AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip")** | The Clip to play for this track. |
| `Volume` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How loud the track should be. |
| `RelativeSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast the Clip is compared to the speed of `playback` |

Fields

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
- Component:MultiAudioClipPlayer
- [Component:SimplexNoiseClip](https://wiki.resonite.com/Component:SimplexNoiseClip "Component:SimplexNoiseClip")
- [Component:TriangleWaveClip](https://wiki.resonite.com/Component:TriangleWaveClip "Component:TriangleWaveClip")
- [Component:SquareWaveClip](https://wiki.resonite.com/Component:SquareWaveClip "Component:SquareWaveClip")
- [Component:SineWaveClip](https://wiki.resonite.com/Component:SineWaveClip "Component:SineWaveClip")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MultiAudioClipPlayer&oldid=98002](https://wiki.resonite.com/index.php?title=Component:MultiAudioClipPlayer&oldid=98002)"

Contents