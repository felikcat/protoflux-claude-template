# ProtoFlux:WebsocketTextMessageSender

> Source: https://wiki.resonite.com/ProtoFlux:WebsocketTextMessageSender

Websocket Text Message Sender

\*

OnSendStart

Client

OnSent

Data

OnSendError

Websockets

This node allows you to send text messages to a WebSocket server via a [WebSocketClient](https://wiki.resonite.com/WebsocketClient_(Component) "WebsocketClient (Component)").

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

An [Call](https://wiki.resonite.com/Impulses "Impulses") to trigger the node.

### Client ( [WebsocketClient](https://wiki.resonite.com/WebsocketClient_(Component) "WebsocketClient (Component)"))

A [WebSocketClient](https://wiki.resonite.com/WebsocketClient_(Component) "WebsocketClient (Component)") component.

### Data ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The data to be sent to the server.

## Outputs

### OnSendStart ( [SyncResumption](https://wiki.resonite.com/Impulses\#ASync "Impulses") (Async))

An [Async impulse](https://wiki.resonite.com/Impulses#ASync "Impulses") that is triggered when starting the send the data.

### OnSent

A [continuation impulse](https://wiki.resonite.com/Impulses "Impulses") triggered when the data is sent successfully.

### OnSendError ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

A [Continuation](https://wiki.resonite.com/Impulses "Impulses") that is triggered when the data couldn't be sent.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:WebsocketTextMessageSender&oldid=111113](https://wiki.resonite.com/index.php?title=ProtoFlux:WebsocketTextMessageSender&oldid=111113)"

Contents