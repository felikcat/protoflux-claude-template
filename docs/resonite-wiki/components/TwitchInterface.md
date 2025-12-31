# Component:TwitchInterface

> Source: https://wiki.resonite.com/Component:TwitchInterface

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/9b/TwitchInterfaceComponent.png/510px-TwitchInterfaceComponent.png)](https://wiki.resonite.com/File:TwitchInterfaceComponent.png) **Twitch Interface** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Twitch interface is a component that is used to allow resonite to communicate to and recieve twitch API events from twitch for a given `Channel` through a [User](https://wiki.resonite.com/Type:User "Type:User").

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetUser` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user to handle sending and receiving network packets to and from twitch. User will need to have agreed to communicate with Twitch for this component to work. |
| `Channel` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The twitch channel to get communications from. |
| `Connected` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the connection to `Channel` is a success and is communicating. |
| `StreamLive` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether `Channel` is currently streaming. |
| `ViewerCount` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many viewers are viewing `Channel`'s stream. |
| `FollowTimeoutSeconds` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How many seconds to wait before allowing another follow event through. |

Fields
Collapse

## Behavior

## Examples

This component is used in [Twitch ProtoFlux Nodes](https://wiki.resonite.com/Category:ProtoFlux:Network:Twitch "Category:ProtoFlux:Network:Twitch") to allow them to function.

## See Also

[Twitch ProtoFlux Nodes](https://wiki.resonite.com/Category:ProtoFlux:Network:Twitch "Category:ProtoFlux:Network:Twitch")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TwitchInterface&oldid=91495](https://wiki.resonite.com/index.php?title=Component:TwitchInterface&oldid=91495)"

Contents