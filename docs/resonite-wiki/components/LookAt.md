# Component:LookAt

> Source: https://wiki.resonite.com/Component:LookAt

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:LookAt&diff=105441) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b6/LookAtComponent.png/510px-LookAtComponent.png)](https://wiki.resonite.com/File:LookAtComponent.png) **Look At** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

> Transform math is difficult, so I just use parents to solve my problems
>
> — [989onan](https://wiki.resonite.com/User:989onan "User:989onan")

Look at is a component that is used to make one [slot](https://wiki.resonite.com/Slot "Slot") point to look at another slot via a SwingTwist interpolation.
Swing Twist is a concept that is too complicated to explain on this wiki, but essentially constrains the rotation on two axies when rotating to a point, locking it within a range. kind of like a turret.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

Be aware where you put this component in your slot hierarchy, as this component wants to be under the same slot (observer) that is looking at your target. If this is not the case, you might expect some local transform logical errors, like objects shaking as it fights its own rotation.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to try to look at. |
| `TargetPoint` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The 3D point to look at when `Target` is not provided. |
| `TargetPointSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The Coordinate space of `TargetPoint` |
| `Up` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The up axis of this slot, usually best to keep at (0,1,0) |
| `RotationOffset` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | How much to rotate the slot by after applying the look at (quaternion multiplying) |
| `SwingReference` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The axis to apply "Swing" rotation to. |
| `TwistReference` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The axis to apply "Twist" rotation to. |
| `MaxSwing` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum (pos/neg) amount that the slot can rotate on `SwingReference` |
| `MaxTwist` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum (pos/neg) amount that the slot can rotate on `TwistReference` |
| `_target` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to apply the rotation result to. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `SetReferenceAxis:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the set reference axis button is touched. |

Triggers
Collapse

## Usage

Attach the component to a slot and provide a `Target` or `TargetPoint` to make it look at or point at a position. It is recommended to put a slot under this component's slot to apply offsets to the rotation.

## Examples

This can be used to make a piston base and rod look at each other to stay connected when the piston moves. this can also be used to make a tracking system.

## See Also

- [Component:AutoLookAtUser](https://wiki.resonite.com/Component:AutoLookAtUser "Component:AutoLookAtUser")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LookAt&oldid=105441](https://wiki.resonite.com/index.php?title=Component:LookAt&oldid=105441)"

Contents