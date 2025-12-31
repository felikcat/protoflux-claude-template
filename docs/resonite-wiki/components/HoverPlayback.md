# Component:HoverPlayback

> Source: https://wiki.resonite.com/Component:HoverPlayback

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/23/HoverPlaybackComponent.png/510px-HoverPlaybackComponent.png)](https://wiki.resonite.com/File:HoverPlaybackComponent.png) **Hover Playback** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **HoverPlayback** component plays or stops a Playable when on the root of a hiearchy that has colliders and is touched/pressed.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | **[SyncPlayback](https://wiki.resonite.com/Type:SyncPlayback "Type:SyncPlayback")** | The Playback (timeline/animation) to influence. |
| `Trigger` | **[HoverPlayback.PlayTrigger](https://wiki.resonite.com/Component:HoverPlayback#PlayTrigger)** | what should trigger the playback. |
| `FromBeginning` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to play from the beginning or not. |
| `Loop` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to loop the playback. |

Fields
Collapse

## PlayTrigger

| Name | Value | Description |
| --- | --- | --- |
| `Hover` | 0 | play/pause the audio when the user hovers their laser over the collider this component is on. |
| `Touch` | 1 | play/pause the audio when the user presses primary over the collider this component is on. |

Values

## Usage

Attach to a slot or slot hiearchy with colliders, and provide a `Target`.

## Examples

Can be used for the play button on a casset player

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:HoverPlayback&oldid=97532](https://wiki.resonite.com/index.php?title=Component:HoverPlayback&oldid=97532)"

Contents