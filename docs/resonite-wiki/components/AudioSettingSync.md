# Component:AudioSettingSync

> Source: https://wiki.resonite.com/Component:AudioSettingSync

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/12/AudioSettingSyncComponent.png/510px-AudioSettingSyncComponent.png)](https://wiki.resonite.com/File:AudioSettingSyncComponent.png) **Audio Setting Sync** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AudioSettingSync** component only works in dash space. This handles the settings of the game when it's values are changed.

see [Settings#Volume](https://wiki.resonite.com/Settings#Volume "Settings")

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `DefaultAudioInputDeviceIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The audio device that should be the default |
| `OverrideAudioOutputIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The audio device to use as an override for the default |
| `MasterVolume` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Controls the volume of everything in Resonite |
| `WhisperVoiceVolume` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Controls the volume of sounds outside of your whisper sphere when using whisper mode. |
| `NoiseGateThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Noise gate prevents background noises from being transmitted to other users. This setting indicates the maximum volume at which sounds will be filtered out. If too much noise is making it in, increase this setting, if your voice is not getting through, lower it. |
| `NoiseGateAttack` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | This indicates how fast the noise gate responds to an incoming sound that is louder than the threshold volume. Larger values will result in a slower volume fade in, while smaller ones will make the volume ramp up quicker. |
| `NoiseGateHold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | This controls how long it takes for the noise gate to begin to close after the microphone input volume falls below the threshold volume. |
| `NoiseGateRelease` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | This setting controls how fast the noise gate closes after the incoming audio has quieted again. |
| `NormalizationThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Using this setting you can control the threshold when the incoming audio will become amplified. If your normal speech is too quiet and it's not getting amplified, lower this setting. If random quiet noises are being amplified, increase it. |
| `VoiceNormalization` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to normalize a user's voice or not. |
| `NoiseSupression` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | This feature processes the incoming audio to filter out various undesirable noises. This can clean up audio from noisy microphones considerably, producing a cleaner voice. We strongly recommend keeping this setting on. However, it can also filter out certain noises that do not get identified as speech. |

Fields
Collapse

## Usage

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AudioSettingSync&oldid=94141](https://wiki.resonite.com/index.php?title=Component:AudioSettingSync&oldid=94141)"

Contents