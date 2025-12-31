# ProtoFlux:TwitchRaidEvent

> Source: https://wiki.resonite.com/ProtoFlux:TwitchRaidEvent

Twitch Raid Event

OnRaid

UserId

DisplayName

Color

ViewerCount

IsSubscriber

Interface

null

∅

Twitch

This node provides Twitch raid information from a [TwitchInterface](https://wiki.resonite.com/Component:TwitchInterface "Component:TwitchInterface").

Note that all outputs are generated on a new Twitch raid event, and will not display any information when connected to a display node.

## Outputs

### OnRaid ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Fires on receiving a new Twitch raid.

### UserId ( [String](https://wiki.resonite.com/Type:String "Type:String"))

Outputs the Twitch Channel ID of the raider.

### DisplayName ( [String](https://wiki.resonite.com/Type:String "Type:String"))

Outputs the Twitch username of the raider.

### Color ( [Color](https://wiki.resonite.com/Type:Color "Type:Color"))

Outputs the Twitch chat color of the raider.

### ViewerCount ( [Int](https://wiki.resonite.com/Type:Int "Type:Int"))

Shows the amount of viewers who are raiding with the raider.

### IsSubscriber ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if the raider is subscribed to the Twitch channel.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:TwitchRaidEvent&oldid=110899](https://wiki.resonite.com/index.php?title=ProtoFlux:TwitchRaidEvent&oldid=110899)"

Contents