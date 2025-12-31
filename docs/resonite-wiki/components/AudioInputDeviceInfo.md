# Component:AudioInputDeviceInfo

> Source: https://wiki.resonite.com/Component:AudioInputDeviceInfo

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AudioInputDeviceInfo&diff=100811) which are not marked for translation.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/15/AudioInputDeviceInfoComponent.png/510px-AudioInputDeviceInfoComponent.png)](https://wiki.resonite.com/File:AudioInputDeviceInfoComponent.png) **Audio Input Device Info** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AudioDeviceIndexFinder** component only works in user space, and is used to find an audio device by name and get info about it.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `DeviceIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The device index if found |
| `DeviceName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | the name to use when looking for a device |
| `IsAppDefault` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this device is resonite's current default |
| `IsSystemDefault` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this device is the user's OS current default |
| `DeviceType` | **[AudioInputType](https://wiki.resonite.com/Type:AudioInputType "Type:AudioInputType")** | The type of audio device this is. |

Fields
Collapse

## Usage

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AudioInputDeviceInfo&oldid=100811](https://wiki.resonite.com/index.php?title=Component:AudioInputDeviceInfo&oldid=100811)"

Contents