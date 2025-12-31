# Component:RandomAudioClipPlayer

> Source: https://wiki.resonite.com/Component:RandomAudioClipPlayer

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/15/RandomAudioClipPlayerComponent.png/510px-RandomAudioClipPlayerComponent.png)](https://wiki.resonite.com/File:RandomAudioClipPlayerComponent.png) **Random Audio Clip Player** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **RandomAudioClipPlayer** component is able to play a random audio file all the way through from a list of `Clips` and parent the resulting one shots under a slot.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ParentUnder` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to parent the one shot objects under. |
| `MinDistance` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | the distance in meters in the audio's set transform space where the audio's perceived volume stops increasing and stays constant all the way to the center. |
| `MaxDistance` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | the maximum distance in meters in the audio's set transform space in meters before it cannot be heard. |
| `RolloffMode` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [AudioRolloffMode](https://wiki.resonite.com/Type:AudioRolloffMode "Type:AudioRolloffMode") >** | An optional [AudioRolloffMode](https://wiki.resonite.com/Type:AudioRolloffMode "Type:AudioRolloffMode") |
| `Clips` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[ClipData](https://wiki.resonite.com/Type:ClipData "Type:ClipData")** | The list of [ClipData](https://wiki.resonite.com/Type:ClipData "Type:ClipData") to choose from, randomly with weights. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `Play:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Plays a random audio clip at it's current position |
| ``PlayAtPoint:Action`1<Float3>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | X | Plays a random audio clip at the provided position. |

Triggers
Collapse

## Usage

Attach to a slot and give the component some `Clips` to play. This component can be trigged via it's [sync delegates](https://wiki.resonite.com/Sync_Delegate "Sync Delegate") or by [button events](https://wiki.resonite.com/Button_Events "Button Events")

## Examples

This can be used for boopers, doorbells, or a bike horn.

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
- Component:RandomAudioClipPlayer
- [Component:MultiAudioClipPlayer](https://wiki.resonite.com/Component:MultiAudioClipPlayer "Component:MultiAudioClipPlayer")
- [Component:SimplexNoiseClip](https://wiki.resonite.com/Component:SimplexNoiseClip "Component:SimplexNoiseClip")
- [Component:TriangleWaveClip](https://wiki.resonite.com/Component:TriangleWaveClip "Component:TriangleWaveClip")
- [Component:SquareWaveClip](https://wiki.resonite.com/Component:SquareWaveClip "Component:SquareWaveClip")
- [Component:SineWaveClip](https://wiki.resonite.com/Component:SineWaveClip "Component:SineWaveClip")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RandomAudioClipPlayer&oldid=99111](https://wiki.resonite.com/index.php?title=Component:RandomAudioClipPlayer&oldid=99111)"

Contents