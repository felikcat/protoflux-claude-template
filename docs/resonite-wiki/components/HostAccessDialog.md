# Component:HostAccessDialog

> Source: https://wiki.resonite.com/Component:HostAccessDialog

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/9d/HostAccessDialogComponent.png/510px-HostAccessDialogComponent.png)](https://wiki.resonite.com/File:HostAccessDialogComponent.png) **Host Access Dialog** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Request Host Access ProtoFlux Node](https://wiki.resonite.com/ProtoFlux:Request_Host_Access "ProtoFlux:Request Host Access").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Host` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The host destination string being accessed. |
| `Port` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The port being asked for access. |
| `AccessType` | **[HostAccessScope](https://wiki.resonite.com/Type:HostAccessScope "Type:HostAccessScope")** | The access type wanted for the port. |
| `_hostText` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text field used to show the server wanting access for. |
| `_reasonText` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The reason for accessing the server. |
| `_allowButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to allow the server to be accessed through your client. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `Deny:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Denies the current request. |
| `Allow:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Accepts the current request. |

Triggers
Collapse

## Usage

Not used directly by the user.

## Examples

The grant access dialogue when protoflux needing access.

## See Also

- [ProtoFlux:Request Host Access](https://wiki.resonite.com/ProtoFlux:Request_Host_Access "ProtoFlux:Request Host Access")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:HostAccessDialog&oldid=98815](https://wiki.resonite.com/index.php?title=Component:HostAccessDialog&oldid=98815)"

Contents