# Component:AvatarAnchorTouchTrigger

> Source: https://wiki.resonite.com/Component:AvatarAnchorTouchTrigger

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarAnchorTouchTrigger&diff=98328) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/9f/AvatarAnchorTouchTriggerComponent.png/510px-AvatarAnchorTouchTriggerComponent.png)](https://wiki.resonite.com/File:AvatarAnchorTouchTriggerComponent.png) **AvatarAnchorTouchTrigger** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Used often for a way of entering and exiting an [Avatar Anchor](https://wiki.resonite.com/Component:AvatarAnchor "Component:AvatarAnchor") when the user wants to.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Anchor` | **[AvatarAnchor](https://wiki.resonite.com/Component:AvatarAnchor "Component:AvatarAnchor")** | The anchor to enter after confirming the enter anchor. |
| `EnterText` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The text for when the user is being prompted to enter the anchor. |
| `ExitText` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The text for when the user is being prompted to exit the anchor. |
| `Enter` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow this component to be used for entering the anchor. |
| `Exit` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow this component to be used for exiting the anchor. |
| `AcceptOutOfSightTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to allow interaction with this component if it is out of the user's view. |
| `AcceptPhysicalTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow [Component:TipTouchSources](https://wiki.resonite.com/Component:TipTouchSource "Component:TipTouchSource") to interact with/activate this component. |
| `AcceptRemoteTouch` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this component allows interaction via the user's interaction laser. |
| `Vibrate` | **[VibratePreset](https://wiki.resonite.com/Type:VibratePreset "Type:VibratePreset")** | What kind of haptics vibration feedback to send to the user's controller when bringing up the enter or exiting prompt. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnEnterConfirm:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles a user clicking on the anchor and confirming they want to enter. |
| `OnExitConfirm:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles a user clicking on the anchor and confirming they want to exit. |

Triggers
Collapse

## Behavior

This needs a collider on the same slot to allow for clicking and bringing up the prompt. The `EnterText` and `ExitText` fields are usually driven by a component. The component automatically translates the dialogues for them in their context menu to their selected locale language.

## Examples

## See Also

[Avatar Anchor](https://wiki.resonite.com/Component:AvatarAnchor "Component:AvatarAnchor")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarAnchorTouchTrigger&oldid=98328](https://wiki.resonite.com/index.php?title=Component:AvatarAnchorTouchTrigger&oldid=98328)"

Contents