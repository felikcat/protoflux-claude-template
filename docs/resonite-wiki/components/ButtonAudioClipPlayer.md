# Component:ButtonAudioClipPlayer

> Source: https://wiki.resonite.com/Component:ButtonAudioClipPlayer

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c7/ButtonAudioClipPlayerComponent.png/510px-ButtonAudioClipPlayerComponent.png)](https://wiki.resonite.com/File:ButtonAudioClipPlayerComponent.png) **Button Audio Clip Player** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ButtonAudioClipPlayer** plays an [AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip") from a list on press, release, and hover.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ParentUnder` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Parents the one shot sound under the specified [slot](https://wiki.resonite.com/Slot "Slot"). |
| `MinDistance` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The minimum distance for this sound. |
| `MaxDistance` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The maximum distance for this sound. |
| `RolloffMode` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [AudioRolloffMode](https://wiki.resonite.com/Type:AudioRolloffMode "Type:AudioRolloffMode") >** | The rolloff for this sound. |
| `PressedClips` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[ClipData](https://wiki.resonite.com/Type:ClipData "Type:ClipData")** | The list of pressed clip sounds. |
| `ReleasedClips` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[ClipData](https://wiki.resonite.com/Type:ClipData "Type:ClipData")** | The list of released clip sounds. |
| `HoverEnterClips` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[ClipData](https://wiki.resonite.com/Type:ClipData "Type:ClipData")** | The list of hover enter clip sounds. |
| `HoverLeaveClips` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[ClipData](https://wiki.resonite.com/Type:ClipData "Type:ClipData")** | The list of hover leave clip sounds. |

Fields
Collapse

| Name | Type | Description |
| --- | --- | --- |
| `Clip` | **\[\[Type:** [AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip") **\|** [AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip") **\]\]** | The sound to play. |
| `Weight` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | How likely this sound will play. |
| `MinVolume` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum volume this sound will play at randomly. |
| `MaxVolume` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum volume this sound will play at randomly. |
| `MinSpeed` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum speed this sound will play at randomly. |
| `MaxSpeed` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum speed this sound will play at randomly. |
| `Spatialized` | **[bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Should this sound be a 3D sound? |
| `SpatialBlend` | **[float](https://wiki.resonite.com/Type:Float "Type:Float")** | How 3D should this sound be? |
| `MinDistance` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The minimum distance this sound should play at. |
| `MaxDistance` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The maximum distance this sound should play at. |
| `RolloffMode` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [AudioRolloffMode](https://wiki.resonite.com/Type:AudioRolloffMode "Type:AudioRolloffMode") >** | The rolloff for this clip. |

Fields

## Usage

This is a powerful component that allows for customizability for your many sounds in one slot, great for boopers and [UIX](https://wiki.resonite.com/UIX "UIX") buttons that need to have a variety of sounds.

## Examples

## See Also

- [Type:IAudioSource](https://wiki.resonite.com/Type:IAudioSource "Type:IAudioSource")
- [Component:AudioClipPlayer](https://wiki.resonite.com/Component:AudioClipPlayer "Component:AudioClipPlayer")
- [Component:StaticAudioClip](https://wiki.resonite.com/Component:StaticAudioClip "Component:StaticAudioClip")
- [Component:ChannelVolumeMeter](https://wiki.resonite.com/Component:ChannelVolumeMeter "Component:ChannelVolumeMeter")
- [Component:VolumeMeter](https://wiki.resonite.com/Component:VolumeMeter "Component:VolumeMeter")
- [Component:SawtoothWaveClip](https://wiki.resonite.com/Component:SawtoothWaveClip "Component:SawtoothWaveClip")
- [Component:ValueNoiseClip](https://wiki.resonite.com/Component:ValueNoiseClip "Component:ValueNoiseClip")
- Component:ButtonAudioClipPlayer
- [Component:LerpingMultiClipPlayer](https://wiki.resonite.com/Component:LerpingMultiClipPlayer "Component:LerpingMultiClipPlayer")
- [TalkVisualizer](https://wiki.resonite.com/Component:TalkVisualizer "Component:TalkVisualizer")
- [Component:RandomAudioClipPlayer](https://wiki.resonite.com/Component:RandomAudioClipPlayer "Component:RandomAudioClipPlayer")
- [Component:MultiAudioClipPlayer](https://wiki.resonite.com/Component:MultiAudioClipPlayer "Component:MultiAudioClipPlayer")
- [Component:SimplexNoiseClip](https://wiki.resonite.com/Component:SimplexNoiseClip "Component:SimplexNoiseClip")
- [Component:TriangleWaveClip](https://wiki.resonite.com/Component:TriangleWaveClip "Component:TriangleWaveClip")
- [Component:SquareWaveClip](https://wiki.resonite.com/Component:SquareWaveClip "Component:SquareWaveClip")
- [Component:SineWaveClip](https://wiki.resonite.com/Component:SineWaveClip "Component:SineWaveClip")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ButtonAudioClipPlayer&oldid=95620](https://wiki.resonite.com/index.php?title=Component:ButtonAudioClipPlayer&oldid=95620)"

Contents