# Component:WorldsDataFeed

> Source: https://wiki.resonite.com/Component:WorldsDataFeed

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0a/WorldsDataFeedComponent.png/510px-WorldsDataFeedComponent.png)](https://wiki.resonite.com/File:WorldsDataFeedComponent.png) **Worlds Data Feed** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **WorldsDataFeed** is a [data feed](https://wiki.resonite.com/Data_Feed "Data Feed") that provides a list of worlds or sessions, depending on the settings.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ListOpenedWorlds` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to list open worlds.<br>**Note:** This only works in privileged contexts, such as [Userspace](https://wiki.resonite.com/Userspace "Userspace"), or worlds opened in Unsafe Mode. |
| `ListSessions` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to list sessions of worlds. |
| `MergeByWorldId` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to merge by world IDs. Used to make [Component:MergedWorldDataItemInterface](https://wiki.resonite.com/Component:MergedWorldDataItemInterface "Component:MergedWorldDataItemInterface"). |
| `MergeBySessionId` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to merge by session IDs. Used to make [Component:MergedWorldDataItemInterface](https://wiki.resonite.com/Component:MergedWorldDataItemInterface "Component:MergedWorldDataItemInterface") |
| `IncompatibleSessions` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to show incompatible sessions due to game version number/plugins. |
| `HeadlessHosts` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to list headless hosts. |
| `UserHosts` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to list normal user hosts. |
| `MinimumTotalUsers` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | List sessions that have more than this many users. |
| `MinimumTotalContacts` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | List sessions that have more than this many users that are contacts to the user. |
| `MinSessionAccessLevel` | **[SessionAccessLevel](https://wiki.resonite.com/Type:SessionAccessLevel "Type:SessionAccessLevel")** | List sessions that have a session access greater or equal to this. |
| `MaxSessionAccessLevel` | **[SessionAccessLevel](https://wiki.resonite.com/Type:SessionAccessLevel "Type:SessionAccessLevel")** | List sessions that have a session access less than or equal to this. |
| `MinUptime` | **[Double](https://wiki.resonite.com/Type:Double "Type:Double")** | A session has to be open for at least this long to be listed. |
| `MaxUptime` | **[Double](https://wiki.resonite.com/Type:Double "Type:Double")** | A session has to be open for less than this long to be listed. |

Fields
Collapse

## Usage

Used in the system of [Data Feeds](https://wiki.resonite.com/Data_Feeds "Data Feeds"). This feed provides MergedWorldDataItemInterface as well as DataFeedEntity<World> and DataFeedEntity<SessionInfo> as part of its feed.

## Examples

This feed is not currently used in official content.

## See Also

- [Data Feeds](https://wiki.resonite.com/Data_Feeds "Data Feeds")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:WorldsDataFeed&oldid=114638](https://wiki.resonite.com/index.php?title=Component:WorldsDataFeed&oldid=114638)"

Contents