# Component:SessionUserController

> Source: https://wiki.resonite.com/Component:SessionUserController

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[File:SessionUserControllerComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=SessionUserControllerComponent.png "File:SessionUserControllerComponent.png") **Session User Controller** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SessionUserController** component is used to control a user in a session granted the local user has the proper permissions.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_name` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The name of the target user. |
| `_slider` | **[Slider\`1](https://wiki.resonite.com/Component:Slider%601 "Component:Slider`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The slider used to change the volume of the target user. |
| `_mute` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button used to mute the target user. |
| `_jump` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button used to jump to the target user. |
| `_respawn` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button used to respawn the target user. |
| `_silence` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button used to silence the target user. |
| `_kick` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button used to kick the target user. |
| `_ban` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button used to ban the target user. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnMute:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the mute target user button is touched. |
| `OnJump:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the jump to target user button is touched. |
| `OnRespawn:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the respawn target user button is touched. |
| `OnSilence:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the silence target user button is touched. |
| `OnKick:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the kick target user button is touched. |
| `OnBan:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the ban target user button is touched. |

Triggers
Collapse

## Usage

Not to be used directly by the user.

## Examples

Is used in the session tab in the dash.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SessionUserController&oldid=99187](https://wiki.resonite.com/index.php?title=Component:SessionUserController&oldid=99187)"

Contents