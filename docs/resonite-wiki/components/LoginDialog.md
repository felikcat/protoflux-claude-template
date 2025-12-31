# Component:LoginDialog

> Source: https://wiki.resonite.com/Component:LoginDialog

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[File:LoginDialogComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=LoginDialogComponent.png "File:LoginDialogComponent.png") **Login Dialog** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LoginDialog** component is used in internal systems and may be replaced at any time. It is used to handle the logging in for users and the UI for such interactions.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `RegisterOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether user should just be registered and not log in afterwards. |
| `_interactionEnabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether interacting with this component is enabled. |
| `_swapRegion` | **[SlideSwapRegion](https://wiki.resonite.com/Component:SlideSwapRegion "Component:SlideSwapRegion")** | Handles the slide animation as this dialogue changes pages. |
| `_username` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The field for entering the user's username. |
| `_email` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The field for entering the user's email address. |
| `_emailRepeat` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The field to confirm the user's email address. |
| `_password` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The field for entering the user's password. |
| `_passwordRepeat` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The field for entering the user's password again for confirmation. |
| `_recoveryCode` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The field to get a recovery code from in case of account loss. |
| `_birthMonth` | **[IntTextEditorParser](https://wiki.resonite.com/Component:IntTextEditorParser "Component:IntTextEditorParser")** | The field to enter the user's legal birth month MM. |
| `_birthDay` | **[IntTextEditorParser](https://wiki.resonite.com/Component:IntTextEditorParser "Component:IntTextEditorParser")** | The field to enter the user's legal birth day DD. |
| `_birthYear` | **[IntTextEditorParser](https://wiki.resonite.com/Component:IntTextEditorParser "Component:IntTextEditorParser")** | The field to enter the user's legal birth year YYYY. |
| `_rememberLogin` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | Whether to keep an encrypted token on disk using modern security protocols so the user can stay remembered for 30 days since last login, token refreshing every login. |
| `_resetUserId` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | Whether to reset the user ID if they are migrating an account from older platforms. |
| `_policies` | **[Checkbox](https://wiki.resonite.com/Component:Checkbox "Component:Checkbox")** | Whether the player accepts the EULA. |
| `_registerButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button for registering. |
| `_loginEmail` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The email used to log in. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnPolicesClick:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the polices button is touched. |
| `DoLogin:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the login button is touched. |
| `DoLoginSaml2:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the login via saml2 button is touched. |
| ``DoLoginSaml2:ButtonEventHandler`1<String>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | ✓ | Called when the login via saml2 button is touched. |
| `DoRegister:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the register button is touched. |
| `DoRegisterReserved:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the register reserve claim button is touched. |
| `RequestRecoveryCode:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the request recovery code button is touched. |
| `DoResetPassword:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the reset password button is touched. |
| `OnCancelRegister:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the cancel register button is touched. |
| `OpenLogin:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the open login button is touched. |
| `OpenRegister:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the open register button is touched. |
| `OpenLostPassword:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the open lost password button is touched. |
| `OnOpenMigration:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the open migration button is touched. |
| `OnDeclineMigration:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the decline migration button is touched. |

Triggers
Collapse

## Usage

Not used directly by the user. Used in the dash.

## Examples

used in dash login.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LoginDialog&oldid=105306](https://wiki.resonite.com/index.php?title=Component:LoginDialog&oldid=105306)"

Contents