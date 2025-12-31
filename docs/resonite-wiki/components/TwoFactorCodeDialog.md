# Component:TwoFactorCodeDialog

> Source: https://wiki.resonite.com/Component:TwoFactorCodeDialog

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[File:TwoFactorCodeDialogComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=TwoFactorCodeDialogComponent.png "File:TwoFactorCodeDialogComponent.png") **Two Factor Code Dialog** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TwoFactorCodeDialog** component is used to accept and process a 2FA code from a user when logging into Resonite.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_code` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The text field used to enter the 2FA code. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnConfirm:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user hits the confirm code button. |

Triggers
Collapse

## Usage

Not to be used by the user directly.

## Examples

Used during log in via 2FA when logging into Resonite.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TwoFactorCodeDialog&oldid=100748](https://wiki.resonite.com/index.php?title=Component:TwoFactorCodeDialog&oldid=100748)"

Contents