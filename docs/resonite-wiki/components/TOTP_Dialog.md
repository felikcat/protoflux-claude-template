# Component:TOTP Dialog

> Source: https://wiki.resonite.com/Component:TOTP_Dialog

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[File:TOTP DialogComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=TOTP_DialogComponent.png "File:TOTP DialogComponent.png") **TOTP Dialog** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TOTP\_Dialog** component, otherwise known as the temporary one time password Component, is used in the dash space for logging into Resonite via TOTP systems.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_swapRegion` | **[SlideSwapRegion](https://wiki.resonite.com/Component:SlideSwapRegion "Component:SlideSwapRegion")** | The region slider for swapping between screens on this UI screen. |
| `_state` | **[TOTP\_Dialog.State](https://wiki.resonite.com/Component:TOTP_Dialog#State)** | The screen this is currently showing. |
| `_codeField` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The text field the accepts codes in the TOTP protocol. |
| `_messageText` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text element showing messages to the user. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnContinue:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user asks to continue. |
| `CopyCodesToClipboard:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user asks to copy TOTP codes to the clipboard. |
| `OnActivate:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user activates the method. |
| `OnDeactivate:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user deactivates the method. |
| `OnClose:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the user closes the dialog |

Triggers
Collapse

## State

| Name | Value | Description |
| --- | --- | --- |
| `Initializing` | 0 | Is currently on the initalizing screen. |
| `SetupAuth` | 1 | Is currently on the setup TOTP screen. |
| `SaveRecoveryCodes` | 2 | Is currently on the save recovery codes screen. |
| `Activate` | 3 | Is currently on the activate TOTP screen. |
| `Deactivate` | 4 | Is currently on the deactivates TOTP screen. |
| `Message` | 5 | Is currently on the submit TOTP screen. |

Values

## Usage

Used in Temporary One Time Password setup.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TOTP\_Dialog&oldid=100749](https://wiki.resonite.com/index.php?title=Component:TOTP_Dialog&oldid=100749)"

Contents