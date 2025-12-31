# Component:IsPlayingDriver

> Source: https://wiki.resonite.com/Component:IsPlayingDriver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/bd/IsPlayingDriverComponent.png/510px-IsPlayingDriverComponent.png)](https://wiki.resonite.com/File:IsPlayingDriverComponent.png) **Is Playing Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **IsPlayingDriver** component checks if a particular [SyncPlayback](https://wiki.resonite.com/Type:SyncPlayback "Type:SyncPlayback") is currently playing, and drives a set of [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") to reflect this status.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Playback` | **[SyncPlayback](https://wiki.resonite.com/Type:SyncPlayback "Type:SyncPlayback")** | The playback to check if it is playing |
| `Targets` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[FieldDrive\`1](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | The set of booleans to drive to whether or not `Playback` is playing or not. |

Fields
Collapse

## Usage

Attach to a slot and provide a value for `Playback` then any boolean in the list of `Targets` will drive to whether or not `Playback` is currently playing.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:PlaybackStateDriver](https://wiki.resonite.com/Component:PlaybackStateDriver "Component:PlaybackStateDriver")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:IsPlayingDriver&oldid=92455](https://wiki.resonite.com/index.php?title=Component:IsPlayingDriver&oldid=92455)"

Contents