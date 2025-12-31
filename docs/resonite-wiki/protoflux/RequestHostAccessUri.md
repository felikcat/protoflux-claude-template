# ProtoFlux:RequestHostAccessUri

> Source: https://wiki.resonite.com/ProtoFlux:RequestHostAccessUri

Request Host Access

\*

OnGranted

Host

OnDenied

Reason

OnIgnored

Scope

Network

The `Request Host Access Url` node takes in a Host IP address (and optionally accessible port of that address if provided), the scope of what type of connection this is, and the reason why this user should connect to this service. When everything is accurate, this node will fire an event depending if this local user has successfully connected to the host service. This relates to the [settings](https://wiki.resonite.com/Settings#Security "Settings") in the [Dash](https://wiki.resonite.com/Dash "Dash") that a user can look through to see what services they have access to.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

This node is useful for convenience of having the host and port combined, but if you want to just have the Host IP Address and Port Number separate, use [Request Host Access](https://wiki.resonite.com/ProtoFlux:Request_Host_Access "ProtoFlux:Request Host Access") instead.


If you provide a scheme (also called a protocol) inside the Url, it will be overridden by the scope every time, as the scope takes priority to determine the type of the network connection. A scheme looks like `https://` or `ws://`.

## Inputs

### \\* ( [Async Call](https://wiki.resonite.com/Impulses "Impulses"))

Calls an impulse to request the host's access to a service.

### Host ( [Uri](https://wiki.resonite.com/Type:Uri "Type:Uri"))

The IP address and Port Number to connect to.

### Scope ( [HostAccessScope](https://wiki.resonite.com/Type:HostAccessScope "Type:HostAccessScope"))

The access type used for this network connection.

### Reason ( [string](https://wiki.resonite.com/Type:String "Type:String"))

The reason to why this user should allow access to the host's service.

## Outputs

### OnGranted ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the local user has accepted the host access to the service. This adds to their list of host accesses in the [settings](https://wiki.resonite.com/Settings#Security "Settings") in the [Dash](https://wiki.resonite.com/Dash "Dash").

### OnDenied ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the local user has declined the host access to the service.

### OnIgnored ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the local user has clicked the close button on the pop-up dialogue that asks for the host access, or somehow avoided the notification through other means.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:RequestHostAccessUri&oldid=110603](https://wiki.resonite.com/index.php?title=ProtoFlux:RequestHostAccessUri&oldid=110603)"

Contents