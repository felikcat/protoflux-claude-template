# Component:TalkVisualizer

> Source: https://wiki.resonite.com/Component:TalkVisualizer

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/11/TalkVisualizerComponent.png/510px-TalkVisualizerComponent.png)](https://wiki.resonite.com/File:TalkVisualizerComponent.png) **Talk Visualizer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

This component takes a float value and a colorX value, and multiplies the float value by the colorX value, and outputs a colorX.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Input` | **[RawOutput\`1](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | A value that constantly changes to visualize the color for. For example, the `Volume` field of a [Volume Meter](https://wiki.resonite.com/Component:VolumeMeter "Component:VolumeMeter"). |
| `BaseColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The original color. |
| `MaterialColor` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[Sync\`1](https://wiki.resonite.com/Type:Sync%601 "Type:Sync`1") < [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") >** | The color to drive with an amplified `BaseColor` value based on `Input` |
| `LightIntensity` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[Sync\`1](https://wiki.resonite.com/Type:Sync%601 "Type:Sync`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | How bright the output color is beyond 1 gain. |

Fields
Collapse

## Examples

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
- TalkVisualizer
- [Component:RandomAudioClipPlayer](https://wiki.resonite.com/Component:RandomAudioClipPlayer "Component:RandomAudioClipPlayer")
- [Component:MultiAudioClipPlayer](https://wiki.resonite.com/Component:MultiAudioClipPlayer "Component:MultiAudioClipPlayer")
- [Component:SimplexNoiseClip](https://wiki.resonite.com/Component:SimplexNoiseClip "Component:SimplexNoiseClip")
- [Component:TriangleWaveClip](https://wiki.resonite.com/Component:TriangleWaveClip "Component:TriangleWaveClip")
- [Component:SquareWaveClip](https://wiki.resonite.com/Component:SquareWaveClip "Component:SquareWaveClip")
- [Component:SineWaveClip](https://wiki.resonite.com/Component:SineWaveClip "Component:SineWaveClip")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TalkVisualizer&oldid=98743](https://wiki.resonite.com/index.php?title=Component:TalkVisualizer&oldid=98743)"

Contents