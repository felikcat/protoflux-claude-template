# Component:UserOnlineStatusSync

> Source: https://wiki.resonite.com/Component:UserOnlineStatusSync

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d0/UserOnlineStatusSyncComponent.png/510px-UserOnlineStatusSyncComponent.png)](https://wiki.resonite.com/File:UserOnlineStatusSyncComponent.png) **UserOnlineStatusSync** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UserOnlineStatusSync** component only works in [userspace](https://wiki.resonite.com/Userspace "Userspace"). It provides the [online status](https://wiki.resonite.com/index.php?title=Online_status&action=edit&redlink=1 "Online status (page does not exist)") that your account currently has.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `OnlineStatus` | **[OnlineStatus](https://wiki.resonite.com/index.php?title=Type:OnlineStatus&action=edit&redlink=1 "Type:OnlineStatus (page does not exist)")** | The online status of the local user. |

Fields
Collapse

## Usage

Attach to a slot that will be in [userspace](https://wiki.resonite.com/Userspace "Userspace") (like a [facet](https://wiki.resonite.com/Facet "Facet")) and bring it into userspace in order for it to begin working.

## Examples

The OnlineStatus and OnlineStatusV2 facet in [Resonite Essentials](https://wiki.resonite.com/Resonite_Essentials "Resonite Essentials") use UserOnlineStatusSync for setting the status and keeping the status synced:

- `resrec:///G-Resonite/R-49769871-ecfc-4d4d-a13c-0c72d4cd4ed6`
- `resrec:///G-Resonite/R-c605cdd7-305a-4446-87ca-3d537d9c2176`

## See Also

- [Facets](https://wiki.resonite.com/Facets "Facets")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UserOnlineStatusSync&oldid=100129](https://wiki.resonite.com/index.php?title=Component:UserOnlineStatusSync&oldid=100129)"

Contents