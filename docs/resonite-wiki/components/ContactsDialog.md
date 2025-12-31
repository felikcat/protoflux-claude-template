# Component:ContactsDialog

> Source: https://wiki.resonite.com/Component:ContactsDialog

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[File:ContactsDialogComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ContactsDialogComponent.png "File:ContactsDialogComponent.png") **Contacts Dialog** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ContactsDialog** component is used in the contacts screen of the [Dash Menu](https://wiki.resonite.com/Dash_Menu "Dash Menu") to search, view, and talk to contacts.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_searchBar` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The search bar to search for users. |
| `_listRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The list of contacts. |
| `_sessionsRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot where the list of sessions from the selected user will be. |
| `_messagesRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot where the list of messages from the selected user will be. |
| `_status` | **[Image](https://wiki.resonite.com/Component:Image "Component:Image")** | The image icon being used for the selected user's status. |
| `_avatar` | **[Image](https://wiki.resonite.com/Component:Image "Component:Image")** | The image icon being used for the selected user's avatar image. |
| `_username` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text for the selected user's username. |
| `_userActionsRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot to store buttons for performing actions on the selected user. |
| `_sendMessageButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button for sending the currently typed message to the selected user. |
| `_sendVoiceMessageButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button for sending a voice message to the currently selected user. |
| `_sendMessageTextField` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The text field to type messages to send to users. |
| `_messagesScrollRect` | **[ScrollRect](https://wiki.resonite.com/Component:ScrollRect "Component:ScrollRect")** | The scroll rectangle component for the scroll area for messages to and from the selected user. |
| `_inviteButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Invite the selected user to the currently focused session if possible. |
| `_requestInviteButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Ask for an invite from the selected user. |
| `_banAllButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Ban the selected user from all sessions that the current local user will host. |
| `_banSessionButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | Ban the selected user from the current focused session. |
| `_unblockedButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to unblock the currently selected user. |
| `_avatarBlockButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to block the currently selected user's avatar. |
| `_mutualBlockButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to do a mutual block with the currently selected user. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``SearchTextChanged:Action`1<TextEditor>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") >** | ✓ | The action to run and pass a text editor as an argument when changing the search text. |
| `OnRemoveContact:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The method to run when removing a contact. |
| `OnAddContact:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The method to run when adding a contact. |
| `OnBanFromAll:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The method to run when banning all on a contact. |
| `OnUnblock:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The method to run when unblocking a contact. |
| `OnAvatarBlock:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The method to run when blocking the avatar of a contact. |
| `OnMutualBlock:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The method to run when mutual blocking a contact. |
| `OnBanFromCurrent:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The method to run when banning a contact from the current session. |
| `OnIgnoreRequest:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The method to run when ignoring a contact request. |
| `OnInviteContact:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The method to run when inviting a contact. |
| `OnRequestInvite:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The method to run when requesting a contact from a user. |
| `OnSendMessage:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The method to run when sending a message to a user. |
| `OnStartRecordingVoiceMessage:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The method to run when starting a voice message to send a message to a user. |
| `OnStopRecordingVoiceMessage:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | The method to run when sending a voice message to a user. |
| ``MessageSubmitPressed:Action`1<TextEditor>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [TextEditor](https://wiki.resonite.com/Component:TextEditor "Component:TextEditor") >** | ✓ | The method to run when submitting a message to a user. |

Triggers
Collapse

## Usage

Not used by the user. Exists as the dash's Contacts tab.

## Examples

Contacts tab in the [Dash Menu](https://wiki.resonite.com/Dash_Menu "Dash Menu")

## See Also

- [Dash Menu](https://wiki.resonite.com/Dash_Menu "Dash Menu")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ContactsDialog&oldid=98812](https://wiki.resonite.com/index.php?title=Component:ContactsDialog&oldid=98812)"

Contents