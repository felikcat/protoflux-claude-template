# Component:AudioStreamSpawner

> Source: https://wiki.resonite.com/Component:AudioStreamSpawner

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/55/AudioStreamSpawnerComponent.png/510px-AudioStreamSpawnerComponent.png)](https://wiki.resonite.com/File:AudioStreamSpawnerComponent.png) **Audio Stream Spawner** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AudioStreamSpawner** component is used as part of the dash to spawn a selected audio stream.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `BitrateKbps` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The bitrate the audio stream should be |
| `DeviceID` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | the device name of the stream we are spawning |
| `_bitrateString` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The bitrate as a string. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnStartStreaming:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Triggered by a button in order to spawn the stream in the world. |

Triggers
Collapse

## Usage

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AudioStreamSpawner&oldid=97861](https://wiki.resonite.com/index.php?title=Component:AudioStreamSpawner&oldid=97861)"

Contents