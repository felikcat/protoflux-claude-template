# Component:SessionInfoSource

> Source: https://wiki.resonite.com/Component:SessionInfoSource

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:SessionInfoSource&diff=100861) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/aa/SessionInfoSourceComponent.webp/510px-SessionInfoSourceComponent.webp.png)](https://wiki.resonite.com/File:SessionInfoSourceComponent.webp) **SessionInfoSource** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SessionInfoSource** component can be used to receive an assortment of useful information from an inputted SessionId.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `SessionId` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The session ID to get information on. |
| `IsOpen` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the session is open. |
| `LastUpdated` | **[DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime")** | The last time the info on this component was updated. |
| `Name` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the session |
| `Description` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The session description. |
| `Tags` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | Tags that the session world has. |
| `CorrespondingRecordId` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The record ID of the world of the session |
| `CorrespondingOwnerId` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The owner UserID of the session's world. |
| `HostUserId` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The UserID of the session host. |
| `HostUsername` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The username of the session host. |
| `SanitizedHostUsername` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The username of the session host which escapes special characters. |
| `AppVersion` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The App version of the client of the session being hosted. |
| `HeadlessHost` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the session is being hosted by a headless client. |
| `SessionURLs` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | A list of other session URLs using the same world. |
| `Thumbnail` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The link for the session thumbnail in text form. |
| `JoinedUsers` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many users are in the world. |
| `ActiveUsers` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Of the people joined, how many are active/focused? |
| `TotalJoinedUsers` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many users have ever joined the world? |
| `TotalActiveUsers` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many users are active?? |
| `MaximumUsers` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The maximum users that can be in the session. |
| `MobileFriendly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the session is compatible with a mobile/quest build of the game. |
| `AccessLevel` | **[SessionAccessLevel](https://wiki.resonite.com/Type:SessionAccessLevel "Type:SessionAccessLevel")** | The sessions level of access to users joining. |
| `IsOnLAN` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the session is set to Local Access Network. |
| `AwayKickEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether away kick is enabled or not |
| `AwayKickInterval` | **[TimeSpan](https://wiki.resonite.com/Type:TimeSpan "Type:TimeSpan")** | How long till a user is kicked for being away in a session. |

Fields
Collapse

## Usage

The SessionInfoSource component can give us the name, description, tags, and many other useful pieces of information about a session from an inputted SessionId. The current SessionId can be obtained using the WorldSessionID ProtoFlux node.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SessionInfoSource&oldid=100861](https://wiki.resonite.com/index.php?title=Component:SessionInfoSource&oldid=100861)"

Contents