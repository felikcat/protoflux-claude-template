# Component:UserInterfacePositioner

> Source: https://wiki.resonite.com/Component:UserInterfacePositioner

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/93/UserInterfacePositionerComponent.png/510px-UserInterfacePositionerComponent.png)](https://wiki.resonite.com/File:UserInterfacePositionerComponent.png) **User Interface Positioner** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UserInterfacePositioner** component causes the slot to which it is attached to track the user's position and rotation (optionally head). This is a somewhat nicer and cleaner alternative than parenting a slot directly to a user's [avatar node](https://wiki.resonite.com/Avatar "Avatar").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetUser` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user to track. |
| `UseHead` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to track to the user's head. |
| `RotateVerticalOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to act like the freeform dash or not. |
| `PositionSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The speed at which the object will track the user's position. |
| `RotationSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The speed at which the object will track the user's rotation. |
| `ActivationDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance from the user to the object at which the object will start tracking the user's position and rotation. Zero means "always track". |
| `ActivationAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The angle between the user and the object at which the object will start tracking the user's position and rotation. Zero means "always track". |
| `DeactivationDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far away the user has to be from the component for it to to stop following. |
| `DeactivationAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much of an angle deviation it has to be for it to stop following. |
| `TargetPosition` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The target position this UI is lerping to. |
| `TargetRotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The target rotation this UI is lerping to. |
| `_position` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field to drive to set the position of this UI. |
| `_rotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field to drive to set the rotation of this UI. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UserInterfacePositioner&oldid=95827](https://wiki.resonite.com/index.php?title=Component:UserInterfacePositioner&oldid=95827)"

Contents