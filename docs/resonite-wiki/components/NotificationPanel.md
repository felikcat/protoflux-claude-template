# Component:NotificationPanel

> Source: https://wiki.resonite.com/Component:NotificationPanel

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[File:NotificationPanelComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=NotificationPanelComponent.png "File:NotificationPanelComponent.png") **Notification Panel** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **NotificationPanel** component is used in user space to show the User their notifications.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `DisplayDuration` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How long to show notifications for. |
| `Dash` | **[UserspaceRadiantDash](https://wiki.resonite.com/Component:UserspaceRadiantDash "Component:UserspaceRadiantDash")** | The component for the dash in the same world. |
| `_canvas` | **[Canvas](https://wiki.resonite.com/Component:Canvas "Component:Canvas")** | The canvas Component showing notifications. |
| `_notificationClip` | **[AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip")** | The audio to play on a new notification made. |
| `_contactRequestClip` | **[AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip")** | The audio to play on a new contact request being made. |
| `_inviteClip` | **[AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip")** | The audio to play on an invite clip being made. |
| `_sociableClip` | **[AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip")** | The audio to play when a friend goes to social status. |
| `_userJoinClip` | **[AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip")** | The audio to play when a user joins. |
| `_userLeaveClip` | **[AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip")** | The audio to play when a user leaves. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``OnNotificationPressed:ButtonEventHandler`1<String>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | ✓ | Called when a notification element is touched. |

Triggers
Collapse

## Usage

Used internally.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:NotificationPanel&oldid=105341](https://wiki.resonite.com/index.php?title=Component:NotificationPanel&oldid=105341)"

Contents