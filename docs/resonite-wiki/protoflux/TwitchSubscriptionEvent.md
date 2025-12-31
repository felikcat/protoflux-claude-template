# ProtoFlux:TwitchSubscriptionEvent

> Source: https://wiki.resonite.com/ProtoFlux:TwitchSubscriptionEvent

Twitch Subscription Event

OnSubscription

UserId

DisplayName

Message

Months

Plan

IsResub

IsGifted

GiftedBy

IsAnonymous

Interface

null

∅

Twitch

This node provides Twitch subscription information from a [TwitchInterface](https://wiki.resonite.com/Component:TwitchInterface "Component:TwitchInterface").

Note that all outputs are generated on a new Twitch chat message, and will not display any information when connected to a display node.

### OnSubscription ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Fires on receiving a new Twitch subscription event.

### UserId ( [String](https://wiki.resonite.com/Type:String "Type:String"))

Outputs the Twitch Channel ID of the subscriber.

### DisplayName ( [String](https://wiki.resonite.com/Type:String "Type:String"))

Outputs the Twitch username of the subscriber.

### Message ( [String](https://wiki.resonite.com/Type:String "Type:String"))

Outputs the contents of the message as a text string.

### Months ( [Int](https://wiki.resonite.com/Type:Int "Type:Int"))

Shows how many months the subscriber has subscribed for.

### Plan ( [SubscriptionPlan](https://wiki.resonite.com/index.php?title=Type:SubscriptionPlan&action=edit&redlink=1 "Type:SubscriptionPlan (page does not exist)"))

Shows the subscription plan type as a custom constant type called [SubscriptionPlan](https://wiki.resonite.com/index.php?title=Type:SubscriptionPlan&action=edit&redlink=1 "Type:SubscriptionPlan (page does not exist)").

### IsResub ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if the subscription is a re-subscription.

### IsGifted ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if the subscription was gifted from another Twitch user.

### GiftedBy ( [String](https://wiki.resonite.com/Type:String "Type:String"))

Shows the name of the Twitch user who gifted the subscription, if gifted.

### IsAnonymous ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Shows if the subscription was gifted from an anonymous Twitch user.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:TwitchSubscriptionEvent&oldid=110903](https://wiki.resonite.com/index.php?title=ProtoFlux:TwitchSubscriptionEvent&oldid=110903)"

Contents