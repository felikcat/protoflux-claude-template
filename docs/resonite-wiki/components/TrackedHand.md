# Component:TrackedHand

> Source: https://wiki.resonite.com/Component:TrackedHand

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/35/TrackedHandComponent.png/510px-TrackedHandComponent.png)](https://wiki.resonite.com/File:TrackedHandComponent.png) **Tracked Hand** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TrackedHand** component controls the grabbing and updating of a hand including camera based hand tracking of a user.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `User` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user this tracked hand belongs to. |
| `HandChirality` | **[Chirality](https://wiki.resonite.com/Type:Chirality "Type:Chirality")** | The hand side this tracked hand corresponds to. |
| `_grabber` | **[Grabber](https://wiki.resonite.com/Component:Grabber "Component:Grabber")** | The grabber component this hand is controlling. |

Fields
Collapse

## Examples

Automatically added to the user root of a user when they spawn.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TrackedHand&oldid=95774](https://wiki.resonite.com/index.php?title=Component:TrackedHand&oldid=95774)"

Contents