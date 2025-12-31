# ProtoFlux:RequestHostAccess

> Source: https://wiki.resonite.com/ProtoFlux:RequestHostAccess

Request Host Access

\*

OnGranted

Host

OnDenied

Port

OnIgnored

Scope

Reason

Network

The `Request Host Access` node takes in a Host IP address, an accessible port of that address, the scope of what type of connection this is, and the reason why this user should connect to this service. When everything is accurate, this node will fire an event depending if this local user has successfully connected to the host service. This relates to the [settings](https://wiki.resonite.com/Settings#Security "Settings") in the [Dash](https://wiki.resonite.com/Dash "Dash") that a user can look through to see what services they have access to.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

This node is useful for allowing you to interchange the host and port separately, but if you want to just have the Uri version for convenience, use [Request Host Access Url](https://wiki.resonite.com/ProtoFlux:Request_Host_Access_Url "ProtoFlux:Request Host Access Url") instead.


If you provide a scheme (also called a protocol) inside the host string, it will be overridden by the scope every time, as the scope takes priority to determine the type of the network connection. A scheme looks like `https://` or `ws://`.

## Inputs

### \\* ( [Async Call](https://wiki.resonite.com/Impulses "Impulses"))

Calls an impulse to request the host's access to a service.

### Host ( [string](https://wiki.resonite.com/Type:String "Type:String"))

The IP address to connect to.

### Port ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The Port Number used to access this IP address.

### Scope ( [HostAccessScope](https://wiki.resonite.com/Type:HostAccessScope "Type:HostAccessScope"))

The access type used for this network connection.

### Reason ( [string](https://wiki.resonite.com/Type:String "Type:String"))

The reason to why this user should allow access to the host's service.

## Outputs

### OnGranted ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the local user has accepted the host access to the service. This adds to thier list of host accesses in the [settings](https://wiki.resonite.com/Settings#Security "Settings") in the [Dash](https://wiki.resonite.com/Dash "Dash").

### OnDenied ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the local user has declined the host access to the service.

### OnIgnored ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the local user has clicked the close button on the pop-up dialoge that asks for the host access, or somehow avoided the notification through other means.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:RequestHostAccess&oldid=110601](https://wiki.resonite.com/index.php?title=ProtoFlux:RequestHostAccess&oldid=110601)"

Contents