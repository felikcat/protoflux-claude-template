# Component:AudioOutputDeviceSelection

> Source: https://wiki.resonite.com/Component:AudioOutputDeviceSelection

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AudioOutputDeviceSelection&diff=99005) which are not marked for translation.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/4f/AudioOutputDeviceSelectionComponent.png/510px-AudioOutputDeviceSelectionComponent.png)](https://wiki.resonite.com/File:AudioOutputDeviceSelectionComponent.png) **Audio Output Device Selection** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AudioOutputDeviceSelection** component is a Legacy component that was used to change the audio output settings.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

For an up-to-date counterpart, see [Component:SettingsDataFeed](https://wiki.resonite.com/Component:SettingsDataFeed "Component:SettingsDataFeed") and read on the concept [Data Feeds](https://wiki.resonite.com/Data_Feeds "Data Feeds").


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `SelectedDeviceIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The device index in the list of devices on the user's machine. |
| `SelectedDeviceName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the selected device. |
| `_deviceButtonRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of the list of buttons to set an audio output device. |

Fields
Collapse

## Usage

Legacy.

## Examples

Used in your local space to select your Audio Output Device.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AudioOutputDeviceSelection&oldid=99005](https://wiki.resonite.com/index.php?title=Component:AudioOutputDeviceSelection&oldid=99005)"

Contents