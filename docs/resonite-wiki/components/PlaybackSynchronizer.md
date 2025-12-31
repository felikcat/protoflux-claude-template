# Component:PlaybackSynchronizer

> Source: https://wiki.resonite.com/Component:PlaybackSynchronizer

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/ed/PlaybackSynchronizerComponent.png/510px-PlaybackSynchronizerComponent.png)](https://wiki.resonite.com/File:PlaybackSynchronizerComponent.png) **Playback Synchronizer** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **PlaybackSynchronizer** component is used to make two Audio Clips play together in unison, play at the same time, or to synchronize.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[SyncPlayback](https://wiki.resonite.com/Type:SyncPlayback "Type:SyncPlayback")** | The playable to synchronize the playback position with the position of `Source`. |
| `Source` | **[IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable")** | The playable that will drive `Target`'s playback |
| `UseNormalizedPosition` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to speed up or slow down the playback of `Target` if the duration doesn't match. |
| `PositionOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How many seconds/normalized position to offset the `Target`'s synchronization with `Source`'s position. |
| `PositionRate` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to multiply `Source`'s position before driving `Target`'s position with it. |

Fields
Collapse

## Usage

This can be used with any playable like an [Component:Animator](https://wiki.resonite.com/Component:Animator "Component:Animator") or otherwise with another animator or audio. It can also be used to synchronize Videos with each other. This can be useful when you want animations/videos to sync up with audio, in perfect unison without having to worry about networking.

## Examples

Used in [989onan's](https://wiki.resonite.com/User:989onan "User:989onan") MMD player and Emote System to sync audio with the dance when the user is dancing with the system.

## See Also

- [Component:PlaybackPositionDriver](https://wiki.resonite.com/Component:PlaybackPositionDriver "Component:PlaybackPositionDriver")
- [Type:AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PlaybackSynchronizer&oldid=93836](https://wiki.resonite.com/index.php?title=Component:PlaybackSynchronizer&oldid=93836)"

Contents