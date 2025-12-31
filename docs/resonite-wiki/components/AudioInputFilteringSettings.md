# Component:AudioInputFilteringSettings

> Source: https://wiki.resonite.com/Component:AudioInputFilteringSettings

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/13/AudioInputFilteringSettingsComponent.png/510px-AudioInputFilteringSettingsComponent.png)](https://wiki.resonite.com/File:AudioInputFilteringSettingsComponent.png) **Audio Input Filtering Settings** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Audio Settings](https://wiki.resonite.com/Settings#Audio "Settings").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `UseVoiceNormalization` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to normalize the incoming voice data. |
| `NormalizationThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | When below this volume, boost so the voice is louder. |
| `UseNoiseSuppression` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use noise suppression. |
| `NoiseGateThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The threshold that audio needs to be above for the voice to get through. |
| `NoiseGateAttack` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | This indicates how fast the noise gate responds to an incoming sound that is louder than the threshold volume. Larger values will result in a slower volume fade in, while smaller ones will make the volume ramp up quicker. |
| `NoiseGateHold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | This controls how long it takes for the noise gate to begin to close after the microphone input volume falls below the threshold volume. |
| `NoiseGateRelease` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | This setting controls how fast the noise gate closes after the incoming audio has quieted again. |

Fields
Collapse

## Usage

See [Audio Settings](https://wiki.resonite.com/Settings#Audio "Settings").

## Examples

See [Audio Settings](https://wiki.resonite.com/Settings#Audio "Settings").

## See Also

- [Audio Settings](https://wiki.resonite.com/Settings#Audio "Settings")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AudioInputFilteringSettings&oldid=96725](https://wiki.resonite.com/index.php?title=Component:AudioInputFilteringSettings&oldid=96725)"

Contents