# Component:AutoLookAtUser

> Source: https://wiki.resonite.com/Component:AutoLookAtUser

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a5/AutoLookAtUserComponent.png/510px-AutoLookAtUserComponent.png)](https://wiki.resonite.com/File:AutoLookAtUserComponent.png) **Auto Look At User** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

> Transform math is difficult, so I just use parents to solve my problems
>
> — [989onan](https://wiki.resonite.com/User:989onan "User:989onan")

The AutoLookAtUser component can be used to make a slot rotate towards a given user or some user that is close to it.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `RetargetDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance that the current target needs to be from the slot for it to pick a new target. |
| `LerpSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The speed at which the slot rotates towards its target. |
| `TargetedUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user that the slot is currently looking at. |
| `AutoTarget` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not the component should pick its own target. |
| `ExcludeActiveUser` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If this is true and the slot with this component is parented to a user, it won't look at that user. |
| `SwingReference` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The first axis in which to restrict rotation essentially. |
| `TwistReference` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The second axis in which to restrict rotation essentially, for best results, make this axis perpendicular to `SwingReference`. |
| `MaxSwing` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this can rotate on the `SwingReference` axis. |
| `MaxTwist` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much this can rotate on the `TwistReference` axis. |
| `_rotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation field to drive with this component's calculations. Usually this is the slot that this component is on. |

Fields
Collapse

## Examples

This can be used to make guards that look at the user when they get close. This can also be used to make UI or nametags that look at the user, or automated turrets.

In Reality, Swing and Twist are a more complicated subject, and is best to just put a slot under this component's slot to apply offsets to the rotation.

## Related Issues

None right now.

## Related Components

- [Component:LookAt](https://wiki.resonite.com/Component:LookAt "Component:LookAt")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AutoLookAtUser&oldid=105440](https://wiki.resonite.com/index.php?title=Component:AutoLookAtUser&oldid=105440)"

Contents