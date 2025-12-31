# Component:InviteRequestItem

> Source: https://wiki.resonite.com/Component:InviteRequestItem

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[File:InviteRequestItemComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=InviteRequestItemComponent.png "File:InviteRequestItemComponent.png") **Invite Request Item** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Invite Request Item** component is used to handle the visual and behavior of invite requests received in chats from other users.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ContactDialog` | **[ContactsDialog](https://wiki.resonite.com/Component:ContactsDialog "Component:ContactsDialog")** | The dialog component that this is under. |
| `HeaderText` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text field that makes up the header for this request in the chat. |
| `InviteButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to invite the user or forward the invite to the next in command. |
| `AddContactButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button to add the user who is asking for an invite as a contact. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `SendDirectInvite:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles sending a direct invite to the asking user. |
| `ForwardInviteRequestToHost:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles forwarding the invite request to the host. |
| `GrantInvite:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles accepting the invite request. |
| `AddAsContact:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles adding the asking user as a contact. |
| `AddHostAsContact:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles adding the host who is receiving the invite as a contact. |
| `AddAsHeadlessContact:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles adding the headless host who is receiving the invite as a contact. |

Triggers
Collapse

## Usage

Not used directly by the user, but is used in the contacts screen.

## Examples

Invite requests and messages.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:InviteRequestItem&oldid=98935](https://wiki.resonite.com/index.php?title=Component:InviteRequestItem&oldid=98935)"

Contents