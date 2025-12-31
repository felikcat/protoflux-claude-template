# Component:UserJoinAudioIndicator

> Source: https://wiki.resonite.com/Component:UserJoinAudioIndicator

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:UserJoinAudioIndicator&diff=95828) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/41/UserJoinAudioIndicatorComponent.png/510px-UserJoinAudioIndicatorComponent.png)](https://wiki.resonite.com/File:UserJoinAudioIndicatorComponent.png) **User Join Audio Indicator** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UserJoinAudioIndicator** component plays an audio clip when a user joins and leaves a session.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `JoinedClips` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[AssetRef\`1](https://wiki.resonite.com/index.php?title=Type:AssetRef%601&action=edit&redlink=1 "Type:AssetRef`1 (page does not exist)") < [AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip") >** | A list of random audio clips to choose from when a user joins the session. Each one will have a different weight. |
| `LeftClips` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[AssetRef\`1](https://wiki.resonite.com/index.php?title=Type:AssetRef%601&action=edit&redlink=1 "Type:AssetRef`1 (page does not exist)") < [AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip") >** | A list of random audio clips to choose from when a user leaves the session. Each one will have a different weight. |
| `Spatialize` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to play the sounds from the slot this component is on or globally. |
| `Volume` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How loud the audio clips should be by default. |

Fields
Collapse

## Usage

Attach to a slot and provide some audio clips to play. The next time a user joins or leaves the session, a clip from the corresponding list will play.

## Examples

Can be used for world join notifiers or for an elevator ding when a user arrives.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UserJoinAudioIndicator&oldid=95828](https://wiki.resonite.com/index.php?title=Component:UserJoinAudioIndicator&oldid=95828)"

Contents