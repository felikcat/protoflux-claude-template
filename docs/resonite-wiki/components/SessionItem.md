# Component:SessionItem

> Source: https://wiki.resonite.com/Component:SessionItem

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/fb/SessionItemComponent.png/510px-SessionItemComponent.png)](https://wiki.resonite.com/File:SessionItemComponent.png) **Session Item** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SessionItem** component is used to handle the session items in a world menu.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_background` | **[Image](https://wiki.resonite.com/Component:Image "Component:Image")** | The UIX image handling the background for this session item. |
| `_statusIndicator` | **[Image](https://wiki.resonite.com/Component:Image "Component:Image")** | The UIX image used to handle showing the status for this world like access level. |
| `_thumbnail` | **[Image](https://wiki.resonite.com/Component:Image "Component:Image")** | The UIX image handling the session preview thumbnail. |
| `_thumbnailTexture` | **[StaticTexture2D](https://wiki.resonite.com/Component:StaticTexture2D "Component:StaticTexture2D")** | The image handling the session preview thumbnail image data. |
| `_sessionName` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text visual being used to show the session name. |
| `_sessionHost` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text visual being used to show the session host's name. |
| `_userCount` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text visual being used to show the session user count. |
| `_joinButton` | **[Button](https://wiki.resonite.com/Component:Button "Component:Button")** | The button that can be used to join the specified session. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnJoin:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the join button is touched. |

Triggers
Collapse

## Usage

not to be used directly by the user.

## Examples

used in world menus.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SessionItem&oldid=99185](https://wiki.resonite.com/index.php?title=Component:SessionItem&oldid=99185)"

Contents