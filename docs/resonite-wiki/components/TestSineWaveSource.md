# Component:TestSineWaveSource

> Source: https://wiki.resonite.com/Component:TestSineWaveSource

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/83/TestSineWaveSourceComponent.png/510px-TestSineWaveSourceComponent.png)](https://wiki.resonite.com/File:TestSineWaveSourceComponent.png) **Test Sine Wave Source** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TestSineWaveSource** component acts the same as a [SineWaveClip](https://wiki.resonite.com/Component:SineWaveClip "Component:SineWaveClip") if it were continuously playing as an [AudioClipPlayer](https://wiki.resonite.com/Component:AudioClipPlayer "Component:AudioClipPlayer"). The main difference though is it allows constant and quick changes in `Frequency` and `Amplitude` without needing time to recalculate.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Frequency` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The pitch of the audio streamed whistle tone. |
| `Amplitude` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The loudness of the streamed whistle tone. |

Fields
Collapse

## Usage

Attach to a slot and insert into a [Component:AudioOutput](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput") to hear the streamed whistle tone.

## Examples

Can be used to test frequencies or be used for a whistle type instrument with quick changes without having to change the speed or volume of a [Component:AudioClipPlayer](https://wiki.resonite.com/Component:AudioClipPlayer "Component:AudioClipPlayer")

## See Also

- [Component:SineWaveClip](https://wiki.resonite.com/Component:SineWaveClip "Component:SineWaveClip")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TestSineWaveSource&oldid=95694](https://wiki.resonite.com/index.php?title=Component:TestSineWaveSource&oldid=95694)"

Contents