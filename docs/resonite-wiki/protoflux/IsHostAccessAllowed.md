# ProtoFlux:IsHostAccessAllowed

> Source: https://wiki.resonite.com/ProtoFlux:IsHostAccessAllowed

Is Host Access Allowed

Host

\*

Port

Scope

Network

The `Is Host Access Allowed` node takes in a Host IP address, an accessible port of that address, and the scope of what type of connection this is. When everything is accurate, this node will return if the user has the host access to a service. This relates to the [settings](https://wiki.resonite.com/Settings#Security "Settings") in the [Dash](https://wiki.resonite.com/Dash "Dash") that a user can look through to see what services they have access to.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

This node is useful for allowing you to interchange the host and port separately, but if you want to just have the Uri version for convenience, use [Is Host Access Allowed Url](https://wiki.resonite.com/ProtoFlux:Is_Host_Access_Allowed_Url "ProtoFlux:Is Host Access Allowed Url") instead.


If you provide a scheme (also called a protocol) inside the host string, it will be overridden by the scope every time, as the scope takes priority to determine the type of the network connection. A scheme looks like `https://` or `ws://`.

## Inputs

### Host ( [string](https://wiki.resonite.com/Type:String "Type:String"))

The IP address to connect to.

### Port ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The Port Number used to access this IP address.

### Scope ( [HostAccessScope](https://wiki.resonite.com/Type:HostAccessScope "Type:HostAccessScope"))

The access type used for this network connection.

## Outputs

### \\* ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

The result if this local user has access to the service connected using the exact IP address (Host), Port number, and correct connection type.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:IsHostAccessAllowed&oldid=110121](https://wiki.resonite.com/index.php?title=ProtoFlux:IsHostAccessAllowed&oldid=110121)"

Contents