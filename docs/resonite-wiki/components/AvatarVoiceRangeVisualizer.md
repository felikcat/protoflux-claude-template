# Component:AvatarVoiceRangeVisualizer

> Source: https://wiki.resonite.com/Component:AvatarVoiceRangeVisualizer

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarVoiceRangeVisualizer&diff=93406) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/68/AvatarVoiceRangeVisualizerComponent.png/510px-AvatarVoiceRangeVisualizerComponent.png)](https://wiki.resonite.com/File:AvatarVoiceRangeVisualizerComponent.png) **AvatarVoiceRangeVisualizer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AvatarVoiceRangeVisualizer** component is used to generate and maintain the whisper bubble that appears when a user enables their whisper bubble mode.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `VolumeSource` | **[IField\`1](https://wiki.resonite.com/Type:IField%601 "Type:IField`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | A float representing audio change. Usually the `Volume` field from a [Component:VolumeMeter](https://wiki.resonite.com/Component:VolumeMeter "Component:VolumeMeter") |
| `AudioOutput` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [AudioOutput](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput") >** | An audio output to read info from to make the bubble size |
| `WhisperColorMin` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color the bubble should glow at when the user is not speaking during whisper mode. |
| `WhisperColorMax` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color the bubble should glow at when the user is speaking at max volume during whisper mode. |
| `WhisperColorRecordingMessage` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color the bubble should be when the user is recording a message. |
| `VisualRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot of the visual generated for this component to function |
| `_activeUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user controlling and updating this component's logic. |
| `_visualSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to use when driving the size of this visual to match the range of the user's whisper mode. Uses `AudioOutput`'s range for the source of the data. |
| `_visualColor` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The field to drive to a color in an inclusive range of `WhisperColorMin` and `WhisperColorMax` depending on volume output. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarVoiceRangeVisualizer&oldid=93406](https://wiki.resonite.com/index.php?title=Component:AvatarVoiceRangeVisualizer&oldid=93406)"

Contents