# Component:CloudServerStatus

> Source: https://wiki.resonite.com/Component:CloudServerStatus

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:CloudServerStatus&diff=98409) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b8/CloudServerStatusComponent.png/510px-CloudServerStatusComponent.png)](https://wiki.resonite.com/File:CloudServerStatusComponent.png) **Cloud Server Status** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **CloudServerStatus** component gets live data about the Resonite cloud by getting the ping data the game engine is sending and receiving from the cloud.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Status` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[ServerStatus](https://wiki.resonite.com/index.php?title=Type:ServerStatus&action=edit&redlink=1 "Type:ServerStatus (page does not exist)")** | The current cloud status. |
| `ResponseTimeMilliseconds` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How long in milliseconds it took for the server to respond to the last ping. |
| `LastServerUpdateTime` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime")** | The last time the server updated |
| `LastServerStateFetch` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime")** | The last time the server status was fetched. |
| `LastLocalServerResponseTime` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime")** | The last time the client got a response from the server. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CloudServerStatus&oldid=98409](https://wiki.resonite.com/index.php?title=Component:CloudServerStatus&oldid=98409)"

Contents