# Component:SyncPlaybackEditor

> Source: https://wiki.resonite.com/Component:SyncPlaybackEditor

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/66/SyncPlaybackEditorComponent.png/510px-SyncPlaybackEditorComponent.png)](https://wiki.resonite.com/File:SyncPlaybackEditorComponent.png) **Sync Playback Editor** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SyncPlaybackEditor** component is used to interact with and modify the playback of a Sync playback like a video, animation, or a sound player.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_playback` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [SyncPlayback](https://wiki.resonite.com/Type:SyncPlayback "Type:SyncPlayback") >** | The playback to edit and influence with this component. |
| `_sliderValue` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The field to drive with the current playback of `_playback` |
| `_loopToggleSprite` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The sprite URI field of the toggle loop button. Used to switch between a loop and a play once icon URI. |
| `_speedField` | **[FloatTextEditorParser](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser")** | The field used to change the speed of the playback of `_playback` |
| `_slider` | **[Slider\`1](https://wiki.resonite.com/Component:Slider%601 "Component:Slider`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The slider used to change the play head/position of `_playback`. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `Play:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Plays the playback of `_playback` |
| `Pause:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Pauses the playback of `_playback` |
| `Stop:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Stops the playback of `_playback` |
| `ToggleLoop:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Toggles the looping property of the playback of `_playback` |

Triggers
Collapse

## Usage

Used commonly in inspectors and video players to allow interaction with playback fields directly.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SyncPlaybackEditor&oldid=100739](https://wiki.resonite.com/index.php?title=Component:SyncPlaybackEditor&oldid=100739)"

Contents