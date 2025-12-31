# Component:VisemeAnalyzer

> Source: https://wiki.resonite.com/Component:VisemeAnalyzer

Collapse **Component image**

[File:VisemeAnalyzerComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=VisemeAnalyzerComponent.png "File:VisemeAnalyzerComponent.png") **Viseme Analyzer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **VisemeAnalyzer** can be used to analyze the sounds from a user's voice, a video, an audio clip player, or any other sound source. The component does analyzing of audio to discern Viseme sounds.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Source` | **[IAudioSource](https://wiki.resonite.com/Type:IAudioSource "Type:IAudioSource")** | The audio source to analyze the audio and extract live viseme data for. |
| `RemoteSource` | **[MultiValueStream\`1](https://wiki.resonite.com/index.php?title=Type:MultiValueStream%601&action=edit&redlink=1 "Type:MultiValueStream`1 (page does not exist)") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | An alternative source of raw data for viseme data. |
| `Smoothing` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to smooth lerp all the outputs. |
| `Silence` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How quiet the audio is in general. |
| `PP` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Outputs the amount that the source audio is making a "Puh" sound. |
| `FF` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Outputs the amount that the source audio is making a "efff" sound. |
| `TH` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Outputs the amount that the source audio is making a "thuh" sound. |
| `DD` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Outputs the amount that the source audio is making a "deh" or "duh" sound. |
| `kk` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Outputs the amount that the source audio is making a "kay" sound. |
| `CH` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Outputs the amount that the source audio is making a "cuh" sound. |
| `SS` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Outputs the amount that the source audio is making a "ess" sound. |
| `nn` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Outputs the amount that the source audio is making a "enm" sound. |
| `RR` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Outputs the amount that the source audio is making a "erh" sound. |
| `aa` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Outputs the amount that the source audio is making a "ah" sound. |
| `E` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Outputs the amount that the source audio is making a "eee" sound. |
| `ih` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Outputs the amount that the source audio is making a "eh" sound. |
| `oh` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Outputs the amount that the source audio is making a "oah" sound. |
| `ou` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Outputs the amount that the source audio is making a "ooh" sound. |
| `LaughterProbability` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How likely it is that the audio source is playing laughter sounds. |

Fields
Collapse

## Usage

This should not need to be used directly by the user.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:DirectVisemeDriver](https://wiki.resonite.com/Component:DirectVisemeDriver "Component:DirectVisemeDriver")
- [Visemes](https://wiki.resonite.com/Visemes "Visemes")
- [Wikipedia on Visemes](https://en.m.wikipedia.org/wiki/Viseme)

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VisemeAnalyzer&oldid=94338](https://wiki.resonite.com/index.php?title=Component:VisemeAnalyzer&oldid=94338)"

Contents