# Component:ContactItem

> Source: https://wiki.resonite.com/Component:ContactItem

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/ed/ContactItemComponent.png/510px-ContactItemComponent.png)](https://wiki.resonite.com/File:ContactItemComponent.png) **Contact Item** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ContactItem** component is used in the contacts tab of the [Dash Menu](https://wiki.resonite.com/Dash_Menu "Dash Menu") to be a contact in the list of contacts on that screen.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_background` | **[Image](https://wiki.resonite.com/Component:Image "Component:Image")** | The background element of the contact item. |
| `_statusIndicator` | **[Image](https://wiki.resonite.com/Component:Image "Component:Image")** | The image used to indicate the user status of the contact item. |
| `_thumbnail` | **[Image](https://wiki.resonite.com/Component:Image "Component:Image")** | The thumbnail Component of that user's profile picture. |
| `_thumbnailTexture` | **[StaticTexture2D](https://wiki.resonite.com/Component:StaticTexture2D "Component:StaticTexture2D")** | The texture being used to show a user's profile picture. |
| `_username` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text showing the user's username. |
| `_status` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text showing the user's status. |
| `_unreadCount` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text showing the number of unread messages from the user. |
| `_joinButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button that can be used to join the user. |
| `_rawUsername` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The raw string of the user's username without ignore tags. |
| `_alternateNames` | _direct_ **[SyncFieldList\`1](https://wiki.resonite.com/Type:SyncFieldList%601 "Type:SyncFieldList`1") < [String](https://wiki.resonite.com/Type:String "Type:String") >** | A list of names the user may have had before. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnJoin:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | What to run when joining the user that corrosponds to this contact item. |

Triggers
Collapse

## Usage

See [Dash Menu](https://wiki.resonite.com/Dash_Menu "Dash Menu").

## Examples

See [Dash Menu](https://wiki.resonite.com/Dash_Menu "Dash Menu").

## See Also

- [Dash Menu](https://wiki.resonite.com/Dash_Menu "Dash Menu")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ContactItem&oldid=98390](https://wiki.resonite.com/index.php?title=Component:ContactItem&oldid=98390)"

Contents