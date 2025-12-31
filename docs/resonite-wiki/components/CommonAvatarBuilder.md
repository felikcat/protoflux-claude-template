# Component:CommonAvatarBuilder

> Source: https://wiki.resonite.com/Component:CommonAvatarBuilder

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b7/CommonAvatarBuilderComponent.png/510px-CommonAvatarBuilderComponent.png)](https://wiki.resonite.com/File:CommonAvatarBuilderComponent.png) **CommonAvatarBuilder** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Common Avatar Builder is a component that is part of every world that defines the spawning behavior and routines to do for all users when they spawn into a world. This can be used to add world settings menus, change what parts of a user get automatically set up, and so on.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `LoadCloudAvatars` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to load the User's set avatar, or load the default avatar instead. |
| `CustomAvatarTemplates` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[CommonAvatarBuilder.AvatarTemplate](https://wiki.resonite.com/Component:CommonAvatarBuilder#AvatarTemplate)** | Avatars that user's will spawn into if they don't have a cloud avatar, or optionally force them into one of these templates. |
| `AutoInject` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | A slot that will automatically be duplicated and added as a child of a user when they join the world. Certain components will use this to override user behavior when part of this slot's hierarchy, like [Avatar Audio Configuration](https://wiki.resonite.com/Component:AvatarAudioConfiguration "Component:AvatarAudioConfiguration") to name one. |
| `SetupNameBadges` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to set up the user's default name badge when they spawn |
| `SetupIconBadges` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to set up the user's default badges when they spawn. |
| `SetupServerVoice` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Only used in kiosk mode. |
| `SetupClientVoice` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Only used in kiosk mode. |
| `SetupServerTools` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Only used in kiosk mode. |
| `SetupClientTools` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Only used in kiosk mode. |
| `SetupLocomotion` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to give the user the default locomotion modules when they spawn. |
| `AllowLocomotion` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow the user to move using locomotion when they spawn. |
| `DefaultHostSilenced` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user should be default muted to the host when they spawn. |
| `DefaultClientSilenced` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user should be default muted on their end when they spawn. |
| `LocomotionModules` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot full of locomotion modules that the user will have by default after they spawn. |
| `ForceDefaultLocomotionModule` | **[ILocomotionModule](https://wiki.resonite.com/Type:ILocomotionModule "Type:ILocomotionModule")** | The locomotion to enable for the user by default when spawning rather than the one in that user's locomotion settings set in their dash. |
| `FindUserPreferredModule` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to try to spawn the user into their preferred locomotion module they set in settings. |
| `SetupItemShelves` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to add item shelves to the user when they spawn. |
| `ParentClientsToServer` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Parents users that join under the host user's slot (yes this is what it does) |
| `AlignTracking` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | used in Kiosk mode in dash space to show Debug tracking visuals |
| `EmptyAvatarSlotHandler` | **[IEmptyAvatarSlotHandler](https://wiki.resonite.com/Type:IEmptyAvatarSlotHandler "Type:IEmptyAvatarSlotHandler")** | Uses this component to handle empty slots like head and hands on a spawning avatar. |
| `FillEmptySlots` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to fill empty AvatarObjectSlots with default head and hand objects if they are missing on their loaded avatar. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``SetupPositionStream:Action`2<ValueStream`1<Float3>, Int>`` | **[Action\`2](https://wiki.resonite.com/index.php?title=Type:Action%602&action=edit&redlink=1 "Type:Action`2 (page does not exist)") < [ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >, [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | ✓ | Used internally. |
| ``SetupRotationStream:Action`2<ValueStream`1<FloatQ>, Int>`` | **[Action\`2](https://wiki.resonite.com/index.php?title=Type:Action%602&action=edit&redlink=1 "Type:Action`2 (page does not exist)") < [ValueStream\`1](https://wiki.resonite.com/index.php?title=Type:ValueStream%601&action=edit&redlink=1 "Type:ValueStream`1 (page does not exist)") < [FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ") >, [Int](https://wiki.resonite.com/Type:Int "Type:Int") >** | ✓ | Used internally. |
| ``LocomotionControllerInitialized:Action`1<LocomotionController>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [LocomotionController](https://wiki.resonite.com/Component:LocomotionController "Component:LocomotionController") >** | ✓ | Used internally. |
| `UpdateLocomotionModules:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Updates the locomotion modules on every user with the ones specified with this component. |

Triggers
Collapse

## AvatarTemplate

| Name | Type | Description |
| --- | --- | --- |
| `TemplateRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The avatar to use if this is chosen. |
| `OnlyForRole` | **[Role](https://wiki.resonite.com/Component:CommonAvatarBuilder#Role)** | What role this choice should apply to. |
| `Weight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The likelyness compared to other choices to choose this. |
| `MaxUsers` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many users at maximum could be assigned this avatar at any given moment. |
| `BlockCloudAvatar` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the user's [Favorited](https://wiki.resonite.com/Favorites "Favorites") avatar should be ignored. |

Fields

### Role

| Name | Value | Description |
| --- | --- | --- |
| `Anyone` | 0 | Anyone will get the avatar. |
| `HostOnly` | 1 | Only the host may get this avatar. |
| `GuestOnly` | 2 | Only guests may get this avatar. |

Values

## Behavior

This component gets read and executed every time a user respawns or joins into a world.

## Examples

Found under [Root](https://wiki.resonite.com/Root "Root") in every world, and is used to control user spawning.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CommonAvatarBuilder&oldid=98349](https://wiki.resonite.com/index.php?title=Component:CommonAvatarBuilder&oldid=98349)"

Contents