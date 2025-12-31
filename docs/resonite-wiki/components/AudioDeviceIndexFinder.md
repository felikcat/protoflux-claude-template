# Component:AudioDeviceIndexFinder

> Source: https://wiki.resonite.com/Component:AudioDeviceIndexFinder

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AudioDeviceIndexFinder&diff=93276) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/97/AudioDeviceIndexFinderComponent.png/510px-AudioDeviceIndexFinderComponent.png)](https://wiki.resonite.com/File:AudioDeviceIndexFinderComponent.png) **Audio Device Index Finder** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AudioDeviceIndexFinder** component only works in user space, and is used to find an audio device by name.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `DeviceIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The device index if found |
| `DeviceName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | the name to use when looking for a device |
| `CaseSensitive` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the matching with `DeviceName` is case sensitive |
| `AllowPartialMatch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the matching with `DeviceName` allows a partial match. |

Fields
Collapse

## Usage

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AudioDeviceIndexFinder&oldid=93276](https://wiki.resonite.com/index.php?title=Component:AudioDeviceIndexFinder&oldid=93276)"

Contents