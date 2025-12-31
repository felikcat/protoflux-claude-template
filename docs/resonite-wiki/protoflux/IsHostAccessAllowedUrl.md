# ProtoFlux:IsHostAccessAllowedUrl

> Source: https://wiki.resonite.com/ProtoFlux:IsHostAccessAllowedUrl

Is Host Access Allowed

Host

\*

Scope

Network

The `Is Host Access Allowed Url` node takes in a host IP address (and optionally accessible port of that address if provided), and the scope of what type of connection this is. When everything is accurate, this node will return if the user has the host access to a service. This relates to the [settings](https://wiki.resonite.com/Settings#Security "Settings") in the [Dash](https://wiki.resonite.com/Dash "Dash") that a user can look through to see what services they have access to.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

This node is useful for convenience of having the host and port combined, but if you want to just have the Host IP Address and Port Number separate, use [Is Host Access Allowed](https://wiki.resonite.com/ProtoFlux:Is_Host_Access_Allowed "ProtoFlux:Is Host Access Allowed") instead.


If you provide a scheme (also called a protocol) inside the Url, it will be overridden by the scope every time, as the scope takes priority to determine the type of the network connection. A scheme looks like `https://` or `ws://`.

## Inputs

### Host ( [Uri](https://wiki.resonite.com/Type:Uri "Type:Uri"))

The IP address and Port Number to connect to.

### Scope ( [HostAccessScope](https://wiki.resonite.com/Type:HostAccessScope "Type:HostAccessScope"))

The access type used for this network connection.

## Outputs

### \\* ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

The result if this local user has access to the service connected using the exact IP address (Host) (with optional Port Number if provided), and correct connection type.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:IsHostAccessAllowedUrl&oldid=110123](https://wiki.resonite.com/index.php?title=ProtoFlux:IsHostAccessAllowedUrl&oldid=110123)"

Contents