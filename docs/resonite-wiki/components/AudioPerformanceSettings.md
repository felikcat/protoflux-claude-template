# Component:AudioPerformanceSettings

> Source: https://wiki.resonite.com/Component:AudioPerformanceSettings

Collapse **Component image**

[File:AudioPerformanceSettingsComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=AudioPerformanceSettingsComponent.png "File:AudioPerformanceSettingsComponent.png") **Audio Performance Settings** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Audio Performance Settings** component is part of the [Settings](https://wiki.resonite.com/Settings "Settings") that control audio buffers.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `MaxVoices` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The maximum voices the user is allowed to hear. |
| `OutputBufferSize` | **[AudioPerformanceSettings.AudioFrameSize](https://wiki.resonite.com/Component:AudioPerformanceSettings#AudioFrameSize)** | The output buffer size in samples. |
| `SimulationFrameSize` | **[AudioPerformanceSettings.AudioFrameSize](https://wiki.resonite.com/Component:AudioPerformanceSettings#AudioFrameSize)** | The simulation buffer size in samples. |

Fields
Collapse

## AudioFrameSize

| Name | Value | Description |
| --- | --- | --- |
| `VeryLow256` | 256 | 256 samples. |
| `Low512` | 512 | 512 samples. |
| `Medium1024` | 1024 | 1024 samples. |
| `Large2048` | 2048 | 2048 samples. |
| `VeryLarge4096` | 4096 | 4096 samples. |
| `ExtremelyLarge8192` | 8192 | 8192 samples. |
| `TestingOneSecond` | 48000 | Sets buffer to hold one second worth of samples. |

Values

## Usage

See [Settings](https://wiki.resonite.com/Settings "Settings").

## Examples

See [Settings](https://wiki.resonite.com/Settings "Settings").

## See Also

- [Settings](https://wiki.resonite.com/Settings "Settings")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AudioPerformanceSettings&oldid=101150](https://wiki.resonite.com/index.php?title=Component:AudioPerformanceSettings&oldid=101150)"

Contents