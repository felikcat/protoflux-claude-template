# Component:OnlineStatistics

> Source: https://wiki.resonite.com/Component:OnlineStatistics

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:OnlineStatistics&diff=97649) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/86/OnlineStatisticsComponent.png/510px-OnlineStatisticsComponent.png)](https://wiki.resonite.com/File:OnlineStatisticsComponent.png) **Online Statistics** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **OnlineStatistics** component shows information about current session numbers and the number of users in them.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Timestamp` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime")** | The last time the component got the online statistics successfully. |
| `VisibleSessions` | _direct_ **[OnlineStatistics.SessionStats](https://wiki.resonite.com/Component:OnlineStatistics#SessionStats)** | Statistics of visible sessions. |
| `HiddenSessions` | _direct_ **[OnlineStatistics.SessionStats](https://wiki.resonite.com/Component:OnlineStatistics#SessionStats)** | Statistics of hidden sessions. |
| `ActiveVisibleSessions` | _direct_ **[OnlineStatistics.SessionStats](https://wiki.resonite.com/Component:OnlineStatistics#SessionStats)** | Statistics of visible sessions with users active in them. |
| `ActiveHiddenSessions` | _direct_ **[OnlineStatistics.SessionStats](https://wiki.resonite.com/Component:OnlineStatistics#SessionStats)** | Statistics of hidden sessions with users active in them. |
| `RegisteredOnlineUsers` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many users with a Resonite account are online |
| `TotalOnlineUsers` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many users are online in total |
| `PresentUsers` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many users are at their keyboard or in headset. |
| `AwayUsers` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many users have their status set to away? |
| `UsersInVR` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many users are in VR? |
| `UsersInScreen` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many users are in screen mode? |
| `UsersOnDesktop` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many users are on desktop? |
| `UsersOnMobile` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many users are using the mobile binary of the game? |
| `UsersInVisiblePublicSessions` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many users are in visible sessions? |
| `UsersInVisibleSemiAccessibleSessions` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many users are in semi accessible sessions like contacts or contacts plus? |
| `UsersInHiddenSessions` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many users are in hidden sessions |
| `UsersInPrivateSessions` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many users are in private sessions? |
| `UsersInPrivate` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many users are in private? |
| `UsersInLAN` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many users are in Local Access Network sessions? |
| `UsersInContacts` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many users are in contacts sessions? |
| `UsersInContactsPlus` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many users are in contacts plus sessions? |
| `UsersInRegistered` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many users are in sessions that require a logged in user? (Not nessarily resonite account because SAML) |
| `UsersInPublic` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many users are currently online in public sessions |
| `GraphicalClientUsers` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many users are not headlesses |
| `ChatClientUsers` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many users are using chat clients? (Like recon) |
| `HeadlessUsers` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many of the online users are [Headless Accounts](https://wiki.resonite.com/Headless_Client "Headless Client") |
| `BotUsers` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many users are bot accounts (occasionally 1 when the resonite bot is online) |

Fields
Collapse

## SessionStats

| Name | Type | Description |
| --- | --- | --- |
| `PublicSessions` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many public sessions are in this category? |
| `RegisteredSessions` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many sessions open only to registered users are in this category? |
| `ContactsPlusSessions` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many sessions open only to contacts of contacts are in this category? |
| `ContactsSessions` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many sessions open to only contacts of the host are in this category? |
| `LANSessions` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many sessions that are Local access network sessions are in this category? |
| `PrivateSessions` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | How many sessions that are invite only are in this category? |

Fields

## Usage

Can be used to get session statistic data or make a hermit counter.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:OnlineStatistics&oldid=97649](https://wiki.resonite.com/index.php?title=Component:OnlineStatistics&oldid=97649)"

Contents