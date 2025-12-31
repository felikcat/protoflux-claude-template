# Component:AudioStreamController

> Source: https://wiki.resonite.com/Component:AudioStreamController

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AudioStreamController&diff=97860) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d5/AudioStreamControllerComponent.png/510px-AudioStreamControllerComponent.png)](https://wiki.resonite.com/File:AudioStreamControllerComponent.png) **Audio Stream Controller** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AudioStreamController** component is an old legacy component.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This shouldn't be used! For a modern component that does the same thing and is customizable, see [AudioStreamInterface](https://wiki.resonite.com/Component:AudioStreamInterface "Component:AudioStreamInterface").


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Stream` | **[IAudioStream](https://wiki.resonite.com/index.php?title=Type:IAudioStream&action=edit&redlink=1 "Type:IAudioStream (page does not exist)")** | The audio stream this is controlling. |
| `AudioOutput` | **[AudioOutput](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput")** | The audio output being used to play the stream. |
| `IsPlayingForOwner` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the audio stream is playing for the user who spawned it. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnToggleBroadcast:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | X | Used to change the audio to broadcast. |
| `OnTogglePlayForOwner:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | X | Used to make the audio play for the stream owner. |

Triggers
Collapse

## Usage

Legacy.

## Examples

Legacy.

## See Also

- [Component:AudioStreamInterface](https://wiki.resonite.com/Component:AudioStreamInterface "Component:AudioStreamInterface")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AudioStreamController&oldid=97860](https://wiki.resonite.com/index.php?title=Component:AudioStreamController&oldid=97860)"

Contents