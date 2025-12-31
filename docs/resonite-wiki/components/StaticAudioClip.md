# Component:StaticAudioClip

> Source: https://wiki.resonite.com/Component:StaticAudioClip

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:StaticAudioClip&diff=99376) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/04/StaticAudioClipComponent.png/510px-StaticAudioClipComponent.png)](https://wiki.resonite.com/File:StaticAudioClipComponent.png) **Static Audio Clip** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **StaticAudioClip** component is what stores pre recorded audio data for components that play audio like [Component:AudioClipPlayer](https://wiki.resonite.com/Component:AudioClipPlayer "Component:AudioClipPlayer"). This component is auto generated when a sound file is imported into the game as part of an audio clip object.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `URL` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The audio clip data location to load. |
| `LoadMode` | **[AudioLoadMode](https://wiki.resonite.com/Type:AudioLoadMode "Type:AudioLoadMode")** | How and when to load the audio |
| `SampleRateMode` | **[SampleRateMode](https://wiki.resonite.com/Type:SampleRateMode "Type:SampleRateMode")** | How to sample the audio's audio data. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``Normalize:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Makes the volume during the audio clip consistent. |
| ``AdjustVolume:Func`2<Float, Task`1<Bool>>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [Float](https://wiki.resonite.com/Type:Float "Type:Float"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Makes the volume louder or quieter. |
| ``ExtractSides:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Split the audio into two or more clips for different audio tracks. |
| ``Denoise:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Removes noise from the audio clip |
| ``TrimSilence:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | removes the silence from the start and end of the audio clip |
| ``TrimStartSilence:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | removes the silence from the start of the clip. |
| ``TrimEndSilence:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | removes the silence from the end of the clip. |
| ``TrimStart:Func`2<Float, Task`1<Bool>>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [Float](https://wiki.resonite.com/Type:Float "Type:Float"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | cuts off audio data from the start of the audio clip. |
| ``TrimEnd:Func`2<Float, Task`1<Bool>>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [Float](https://wiki.resonite.com/Type:Float "Type:Float"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | cuts off audio data from the end of the audio clip. |
| ``FadeIn:Func`2<Float, Task`1<Bool>>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [Float](https://wiki.resonite.com/Type:Float "Type:Float"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Makes the audio fade in over x seconds. |
| ``FadeOut:Func`2<Float, Task`1<Bool>>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [Float](https://wiki.resonite.com/Type:Float "Type:Float"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Makes the audio fade out over x seconds. |
| ``MakeFadeLoop:Func`2<Float, Task`1<Bool>>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [Float](https://wiki.resonite.com/Type:Float "Type:Float"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Makes the audio loopable, using a cross fade of x seconds. |
| ``ConvertToWAV:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | converts the audio clip type to Windows audio vodec. |
| ``ConvertToVorbis:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | converts the audio clip type to Vorbis. |
| ``ConvertToFLAC:Func`1<Task`1<Bool>>`` | **[Func\`1](https://wiki.resonite.com/Type:Func%601 "Type:Func`1") < [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Converts the audio clip type to FLAC. |
| ``ApplyZitaReverb:Func`2<ZitaParameters, Task`1<Bool>>`` | **[Func\`2](https://wiki.resonite.com/Type:Func%602 "Type:Func`2") < [ZitaParameters](https://wiki.resonite.com/Type:ZitaParameters "Type:ZitaParameters"), [Task\`1](https://wiki.resonite.com/index.php?title=Type:Task%601&action=edit&redlink=1 "Type:Task`1 (page does not exist)") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >>** | X | Uses [ZitaParameters](https://wiki.resonite.com/Type:ZitaParameters "Type:ZitaParameters") to create a reverberation sound effect on this audio clip. |
| `Normalize:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Makes the volume during the audio clip consistent. |
| `ExtractSides:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Split the audio into two or more clips for different audio tracks. |
| `Denoise:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Removes noise from the audio clip |
| ``TrimSilence:ButtonEventHandler`1<FloatTextEditorParser>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [FloatTextEditorParser](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser") >** | ✓ | removes the silence from the start and end of the audio clip |
| ``TrimStartSilence:ButtonEventHandler`1<FloatTextEditorParser>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [FloatTextEditorParser](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser") >** | ✓ | removes the silence from the start of the clip. |
| ``TrimEndSilence:ButtonEventHandler`1<FloatTextEditorParser>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [FloatTextEditorParser](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser") >** | ✓ | removes the silence from the end of the clip. |
| ``TrimStart:ButtonEventHandler`1<FloatTextEditorParser>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [FloatTextEditorParser](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser") >** | ✓ | cuts off audio data from the start of the audio clip. |
| ``TrimEnd:ButtonEventHandler`1<FloatTextEditorParser>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [FloatTextEditorParser](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser") >** | ✓ | cuts off audio data from the end of the audio clip. |
| ``FadeIn:ButtonEventHandler`1<FloatTextEditorParser>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [FloatTextEditorParser](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser") >** | ✓ | Makes the audio fade in over x seconds. |
| ``FadeOut:ButtonEventHandler`1<FloatTextEditorParser>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [FloatTextEditorParser](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser") >** | ✓ | Makes the audio fade out over x seconds. |
| ``MakeLoopable:ButtonEventHandler`1<FloatTextEditorParser>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [FloatTextEditorParser](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser") >** | ✓ | Makes the audio loopable, using a cross fade of x seconds. |
| ``ConvertToWAV:ButtonEventHandler`1<FloatTextEditorParser>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [FloatTextEditorParser](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser") >** | ✓ | converts the audio clip type to Windows audio vodec. |
| ``ConvertToVorbis:ButtonEventHandler`1<FloatTextEditorParser>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [FloatTextEditorParser](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser") >** | ✓ | converts the audio clip type to Vorbis. |
| ``ConvertToFLAC:ButtonEventHandler`1<FloatTextEditorParser>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [FloatTextEditorParser](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser") >** | ✓ | Converts the audio clip type to FLAC. |

Triggers
Collapse

## Usage

## Examples

## See Also

- [Component:PlaybackSynchronizer](https://wiki.resonite.com/Component:PlaybackSynchronizer "Component:PlaybackSynchronizer") for synchronizing playables

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:StaticAudioClip&oldid=99376](https://wiki.resonite.com/index.php?title=Component:StaticAudioClip&oldid=99376)"

Contents