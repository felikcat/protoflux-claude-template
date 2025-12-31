# Component:PlaybackPositionDriver

> Source: https://wiki.resonite.com/Component:PlaybackPositionDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:PlaybackPositionDriver&diff=96503) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/7d/PlaybackPositionDriverComponent.png/510px-PlaybackPositionDriverComponent.png)](https://wiki.resonite.com/File:PlaybackPositionDriverComponent.png) **Playback Position Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **PlaybackPositionDriver** component is used to output and/or influence the playback position of an [IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with the time position of `Source` from. If `UseNormalizedPosition` is true, this is 0<->1, else it's the amount of seconds from the start. |
| `Source` | **[IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable")** | The playable audio to get the time from. |
| `UseNormalizedPosition` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to output a 0<->1 or an amount of seconds |
| `WriteBack` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether writing to the value of the field specified by `Target` will set the playback position. See [write backs](https://wiki.resonite.com/Drives#Write_Backs "Drives"). |

Fields
Collapse

## Usage

Can be used on a timeline to get the amount of time left or played in an audio clip that is playing.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:PlaybackSynchronizer](https://wiki.resonite.com/Component:PlaybackSynchronizer "Component:PlaybackSynchronizer")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PlaybackPositionDriver&oldid=96503](https://wiki.resonite.com/index.php?title=Component:PlaybackPositionDriver&oldid=96503)"

Contents