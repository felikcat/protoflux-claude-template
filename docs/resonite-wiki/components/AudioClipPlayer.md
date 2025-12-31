# Component:AudioClipPlayer

> Source: https://wiki.resonite.com/Component:AudioClipPlayer

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AudioClipPlayer&diff=97854) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/18/AudioClipPlayerComponent.png/510px-AudioClipPlayerComponent.png)](https://wiki.resonite.com/File:AudioClipPlayerComponent.png) **Audio Clip Player** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `playback` | _direct_ **[SyncPlayback](https://wiki.resonite.com/Type:SyncPlayback "Type:SyncPlayback")** | The playback object that includes data about playtime, duration, position, and playspeed of the audio. |
| `Clip` | **[AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip")** | The AudioClip to play. This can be a [StaticAudioClip](https://wiki.resonite.com/Component:StaticAudioClip "Component:StaticAudioClip"). |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `Play:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | When called, starts playback for this component. |
| `Stop:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | When called, stops playback for this component. |
| `Pause:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | When called, pauses playback for this component. |
| `Resume:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | When called, resumes playback for this component. |

Triggers
Collapse

## Usage

Add an audio clip to the Clip field by holding a default audio clip player and clicking. then put the Audio Clip Player into an [Audio Output](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput") and hit play to hear the audio.

## Examples

This is usually used in in-game audio players like radios, vehicles, and default audio clip players to play audio constantly. It can be used to play audio and be able to scrub the audio without worrying about working with one shots which play all the way through.

## See Also

- [Component:PlaybackSynchronizer](https://wiki.resonite.com/Component:PlaybackSynchronizer "Component:PlaybackSynchronizer") for synchronizing playables
- [Type:IAudioSource](https://wiki.resonite.com/Type:IAudioSource "Type:IAudioSource")
- Component:AudioClipPlayer
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
- [Component:TriangleWaveClip](https://wiki.resonite.com/Component:TriangleWaveClip "Component:TriangleWaveClip")
- [Component:SquareWaveClip](https://wiki.resonite.com/Component:SquareWaveClip "Component:SquareWaveClip")
- [Component:SineWaveClip](https://wiki.resonite.com/Component:SineWaveClip "Component:SineWaveClip")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AudioClipPlayer&oldid=97854](https://wiki.resonite.com/index.php?title=Component:AudioClipPlayer&oldid=97854)"

Contents