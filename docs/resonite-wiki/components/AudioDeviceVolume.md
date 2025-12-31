# Component:AudioDeviceVolume

> Source: https://wiki.resonite.com/Component:AudioDeviceVolume

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/6f/AudioDeviceVolumeComponent.png/510px-AudioDeviceVolumeComponent.png)](https://wiki.resonite.com/File:AudioDeviceVolumeComponent.png) **Audio Device Volume** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AudioDeviceVolume** component only functions in dash space. If `AudioDeviceIndex` is negative, then it uses the user's set default audio device. This component is used to manage the volume of an input device like a microphone for one example. This is a settings component.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AudioDeviceIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The audio input device by OS audio manager index to modify the volume for. |
| `Volume` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The volume the input device should have. |
| `NormalizedVolume` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The component uses this value to boost the output noise to a higher volume when it is too quiet or reduce the volume when it is too loud. |
| `Smoothing` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast to reduce or increase the volume when it gets too loud or quiet |
| `Power` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount to boost the volume overall before normalization. |

Fields
Collapse

## Usage

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AudioDeviceVolume&oldid=93144](https://wiki.resonite.com/index.php?title=Component:AudioDeviceVolume&oldid=93144)"

Contents