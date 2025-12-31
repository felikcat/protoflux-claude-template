# Component:FlipAtUser

> Source: https://wiki.resonite.com/Component:FlipAtUser

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:FlipAtUser&diff=91477) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a9/FlipAtUserComponent.png/510px-FlipAtUserComponent.png)](https://wiki.resonite.com/File:FlipAtUserComponent.png) **Flip At User** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The FlipAtUser component can be used to make an object face towards positive or negative Z, depending on what side of it the local user is.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `UpSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | the coordinate space that is used when calculating what is "up". If set to local user space, then the up direction of this component is the up direction of the slot the user is parented under, which is usually up for that user. This can be useful if a user is in a gravity direction which doesn't match the world's up direction, and will make this orient to that user's direction for a better reading experience for example. |
| `_rotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field that is driven to make the object rotate to the user. This is automatically set to the Rotation field of the slot this component is added to. |

Fields
Collapse

## Usage

## Examples

Useful for signs or dialouge boxes.

## Related Components

[Look At User](https://wiki.resonite.com/Component:LookAtUser "Component:LookAtUser")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FlipAtUser&oldid=91477](https://wiki.resonite.com/index.php?title=Component:FlipAtUser&oldid=91477)"

Contents