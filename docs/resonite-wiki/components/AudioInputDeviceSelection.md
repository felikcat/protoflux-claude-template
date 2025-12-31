# Component:AudioInputDeviceSelection

> Source: https://wiki.resonite.com/Component:AudioInputDeviceSelection

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AudioInputDeviceSelection&diff=99007) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/ec/AudioInputDeviceSelectionComponent.png/510px-AudioInputDeviceSelectionComponent.png)](https://wiki.resonite.com/File:AudioInputDeviceSelectionComponent.png) **Audio Input Device Selection** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AudioInputDeviceSelection** component is a Legacy component part of the old settings UI.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

For an up-to-date counterpart, see [Component:SettingsDataFeed](https://wiki.resonite.com/Component:SettingsDataFeed "Component:SettingsDataFeed") and read on the concept [Data Feeds](https://wiki.resonite.com/Data_Feeds "Data Feeds").


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `SelectedDeviceIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The current selected. |
| `SelectedDeviceName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the currently selected device. |
| `UseFilteredData` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to filter the incoming audio. |
| `_deviceButtonRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to place device selection buttons. |
| `_audioStream` | **[LocalAudioDeviceStream](https://wiki.resonite.com/Component:LocalAudioDeviceStream "Component:LocalAudioDeviceStream")** | The audio stream of the currently selected audio device. |
| `_audioOutput` | **[AudioOutput](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput")** | The audio output being used to preview the audio input device. |
| `_deviceVolume` | **[VolumeMeter](https://wiki.resonite.com/Component:VolumeMeter "Component:VolumeMeter")** | The component being used to analyze the incoming audio of the selected input device and turn it into volume. |
| `_volumeBar` | **[ProgressBar](https://wiki.resonite.com/Component:ProgressBar "Component:ProgressBar")** | The bar being used to preview the input audio device volume. |

Fields
Collapse

## Usage

Used in your Local Space settings to select your Audio Input device.

## Examples

Legacy.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AudioInputDeviceSelection&oldid=99007](https://wiki.resonite.com/index.php?title=Component:AudioInputDeviceSelection&oldid=99007)"

Contents