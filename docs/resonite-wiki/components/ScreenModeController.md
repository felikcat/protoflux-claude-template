# Component:ScreenModeController

> Source: https://wiki.resonite.com/Component:ScreenModeController

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[File:ScreenModeControllerComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ScreenModeControllerComponent.png "File:ScreenModeControllerComponent.png") **Screen Mode Controller** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ScreenModeController** component is used to control the interactions of the user within user space also known as the dash world.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_dash` | **[UserspaceRadiantDash](https://wiki.resonite.com/Component:UserspaceRadiantDash "Component:UserspaceRadiantDash")** | The dash of the dash world. |
| `_muteSound` | **[AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip")** | The audio clip to play when the user mutes themselves. |
| `_unmuteSound` | **[AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip")** | The audio clip to play when the user unmutes themselves. |
| `_startTalkSound` | **[AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip")** | The audio clip to play when the user starts to record a voice message. |
| `_stopTalkSound` | **[AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip")** | The audio clip to play when the user stops recording a voice message. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ScreenModeController&oldid=106554](https://wiki.resonite.com/index.php?title=Component:ScreenModeController&oldid=106554)"

Contents