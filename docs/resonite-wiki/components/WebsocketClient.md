# Component:WebsocketClient

> Source: https://wiki.resonite.com/Component:WebsocketClient

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/df/WebsocketClient.png/510px-WebsocketClient.png)](https://wiki.resonite.com/File:WebsocketClient.png) **Websocket Client** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `URL` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The Websocket server to target - either secure (`wss://`) or insecure (`ws://`) |
| `HandlingUser` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user who will be responsible for establishing the connection, and transmitting data. |
| `AccessReason` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | A descriptive string explaining why this connection request should be granted |
| `ConnectRetryInterval` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How often to retry the connection, if it fails for reasons other than being rejected by the user. |
| `IsConnected` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | A read-only value indicating if this client has successfully connected to the target specified in `URL` |

Fields
Collapse

## Usage

This component must be used in conjunction with the Websocket Protoflux Nodes - it only exists to store state, and does not function on its own.

`User` should be a user that expects to be hosting the Websocket connection
Assignments should generally be made in the following order, depending on which one is the most applicable:

- **The user wearing the avatar containing this Protoflux**
- **A specifically defined user who is expected to be present for this connection to function**
- The user who spawned the object containing this Protoflux
- The user who is currently interacting with the object
- The host of the session

You should not select a user who is not expecting the object to connect to an external service. It is possible they will deny the connection (especially if `AccessReason` isn't sufficiently convincing), which will cause the connection to fail.

`AccessReason` should provide a clear and concise reason for wanting to connect to the external service - It should include an obvious title or description of the object that is attempting to establish the connection, so that the user is aware of what item in the world is prompting the connection.

The object should have some way of indicating that it did not successfully connect to the target service, and that it will not function as intended, if at all.

The websocket times out and disconnects if the remote server does not send any traffic (including heartbeat messages) at least every 60 seconds, for long running connections be sure to configure the keepalive interval on the server side.

## Examples

## Related Issues

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:WebsocketClient&oldid=78732](https://wiki.resonite.com/index.php?title=Component:WebsocketClient&oldid=78732)"

Contents