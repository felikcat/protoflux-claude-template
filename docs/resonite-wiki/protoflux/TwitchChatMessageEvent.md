# ProtoFlux:TwitchChatMessageEvent

> Source: https://wiki.resonite.com/ProtoFlux:TwitchChatMessageEvent

Twitch Chat Message Event

OnMessage

Message

UserId

DisplayName

Color

IsHighlighted

IsSubscriber

IsModerator

IsBroadcaster

IsTurbo

IsVIP

CheerBadge

CheerAmount

Bits

BitsDollars

SubscribedMonthCount

CustomRewardId

Interface

null

∅

Twitch

This node provides Twitch chat message information from a [TwitchInterface](https://wiki.resonite.com/Component:TwitchInterface "Component:TwitchInterface").

Note that all outputs are generated on a new Twitch chat message, and will not display any information when connected to a display node.

## Outputs

### OnMessage ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Fires on receiving a new Twitch chat message.

### Message ( [String](https://wiki.resonite.com/Type:String "Type:String"))

Outputs the contents of the message as a text string.

### UserId ( [String](https://wiki.resonite.com/Type:String "Type:String"))

Outputs the Twitch Channel ID of the message sender.

### DisplayName ( [String](https://wiki.resonite.com/Type:String "Type:String"))

Outputs the Twitch username of the message sender.

### Color ( [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

Outputs the Twitch chat color of the message sender.

### IsHighlighted ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if the chat message is highlighted.

### IsSubscriber ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if the chat message sender is subscribed to the Twitch channel.

### IsModerator ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if the chat message sender is a moderator of the Twitch channel.

### IsBroadcaster ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if the chat message sender is from the Twitch channel, or broadcaster.

### IsTurbo ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if the chat message sender is subscribed to Twitch Turbo.

### IsVIP ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if the chat message sender is a VIP in the Twitch channel.

### CheerBadge ( [BadgeColor](https://wiki.resonite.com/index.php?title=Type:BadgeColor&action=edit&redlink=1 "Type:BadgeColor (page does not exist)"))

Shows the current cheer chat badge of the chat message sender.

### CheerAmount ( [Int](https://wiki.resonite.com/Type:Int "Type:Int"))

Shows the cheer amount if the chat message includes any bits.

### Bits ( [Int](https://wiki.resonite.com/Type:Int "Type:Int"))

Shows the bit amount if the chat message includes any.

### BitsDollars ( [Double](https://wiki.resonite.com/Type:Double "Type:Double"))

Shows the bit amount in USD (United States Dollars), as a [double](https://wiki.resonite.com/Type:Double "Type:Double") value.

### SubscribedMonthCount ( [Int](https://wiki.resonite.com/Type:Int "Type:Int"))

Shows the amount of months the chat message sender is subscribed to the channel.

### CustomRewardId ( [String](https://wiki.resonite.com/Type:String "Type:String"))

If the chat message was sent with a custom reward redeem, shows the ID of the custom reward.
This will only output the custom reward ID if the redeem has the "Require Viewer to Enter Text" option enabled.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:TwitchChatMessageEvent&oldid=110895](https://wiki.resonite.com/index.php?title=ProtoFlux:TwitchChatMessageEvent&oldid=110895)"

Contents