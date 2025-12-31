# Component:PlatformInfo

> Source: https://wiki.resonite.com/Component:PlatformInfo

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/59/PlatformInfoComponent.png/510px-PlatformInfoComponent.png)](https://wiki.resonite.com/File:PlatformInfoComponent.png) **Platform Info** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **PlatformInfo** component is used where data about the platform that [FrooxEngine](https://wiki.resonite.com/FrooxEngine "FrooxEngine") is running under (In this case, [Resonite](https://wiki.resonite.com/Resonite "Resonite")) for the purpose of providing info to users like social links and language like Abbreviations and ways to refer to the platform.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `PlatformName` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the platform. |
| `ShortNamePrefix` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The short name of the platform, used in record strings. |
| `Abbreviation` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The abreviation of the platform, useful for referring to it in casual conversation. |
| `Domain` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The website of the plaform. |
| `Email` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The platform's email address. |
| `DiscordInviteUrl` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The URL to get to the platform's Discord. |
| `PoliciesPage` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The TOS of the platform. |
| `PatreonUrl` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The Patreon URL of the platform. |
| `GitHubProfile` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The Github profile of the platform. |
| `GitHubIssuesRepository` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The Github issues page of the platform. |
| `AuthScheme` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The authorization scheme of the platform. |
| `AppScheme` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The app scheme of the platform. |
| `DBScheme` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The data base scheme of the platform. used in asset urls. |
| `SessionScheme` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The session scheme of the platform. used in session links. |
| `RecordScheme` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The record scheme of the platform. used in item link urls. |
| `UserSessionScheme` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The user session scheme of the platform. |

Fields
Collapse

## Usage

Can be used to get up to date information on the platform ( [Resonite](https://wiki.resonite.com/Resonite "Resonite")) in real time for in use in items or worlds.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PlatformInfo&oldid=96916](https://wiki.resonite.com/index.php?title=Component:PlatformInfo&oldid=96916)"

Contents