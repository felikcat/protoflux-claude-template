# Component:UserInspectorItem

> Source: https://wiki.resonite.com/Component:UserInspectorItem

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d0/UserInspectorItemComponent.png/510px-UserInspectorItemComponent.png)](https://wiki.resonite.com/File:UserInspectorItemComponent.png) **User Inspector Item** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UserInspectorItem** component is used to display user items of the [User Inspector](https://wiki.resonite.com/User_Inspector "User Inspector").

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_user` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user this item points to. |
| `_userNameText` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The text field to display the user's name. |
| `_expander` | **[Expander](https://wiki.resonite.com/Component:Expander "Component:Expander")** | The component used to expand items under the user like stream groups. |
| `_expanderIndicator` | **[TextExpandIndicator](https://wiki.resonite.com/Component:TextExpandIndicator "Component:TextExpandIndicator")** | The indicator component used to show the expand/collapse arrow. |
| `_childContainer` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to display child items of this user item. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OpenUser:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Is called when the user is opened by a user. |
| `OpenComponents:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Is called when the user components are opened up. |
| ``OpenStream:ButtonEventHandler`1<Ushort>`` | **[ButtonEventHandler\`1](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler%601&action=edit&redlink=1 "Type:ButtonEventHandler`1 (page does not exist)") < [Ushort](https://wiki.resonite.com/Type:Ushort "Type:Ushort") >** | ✓ | Is called when a specific stream on a user is opened up. |

Triggers
Collapse

## Usage

See [User Inspector](https://wiki.resonite.com/User_Inspector "User Inspector").

## Examples

See [User Inspector](https://wiki.resonite.com/User_Inspector "User Inspector").

## See Also

- [User Inspector](https://wiki.resonite.com/User_Inspector "User Inspector")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UserInspectorItem&oldid=100795](https://wiki.resonite.com/index.php?title=Component:UserInspectorItem&oldid=100795)"

Contents