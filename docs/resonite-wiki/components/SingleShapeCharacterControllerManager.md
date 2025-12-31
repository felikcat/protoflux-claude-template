# Component:SingleShapeCharacterControllerManager

> Source: https://wiki.resonite.com/Component:SingleShapeCharacterControllerManager

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/6f/SingleShapeCharacterControllerManagerComponent.png/510px-SingleShapeCharacterControllerManagerComponent.png)](https://wiki.resonite.com/File:SingleShapeCharacterControllerManagerComponent.png) **Single Shape Character Controller Manager** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SingleShapeCharacterControllerManager** component is used by locomotions to change the shape of a [Capsule Collider](https://wiki.resonite.com/Component:CapsuleCollider "Component:CapsuleCollider") based on a user's standing height and current height.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `UseUserHeadHeightWhenAvailable` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use the user's head height to do calculations when possible. |
| `HeadHeightOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to add/subtract from the user's head to make the top of the capsule. |
| `CrouchTargetWidth` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How wide the capsule should become when crouching. |
| `CrouchStart` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum height the user's head has to be for them to be crouching. |
| `CrouchEnd` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum height the user's head has to be for them to be crouching. |
| `DefaultHeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The user's default head height. |
| `DefaultWidth` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The collider's width when standing. |
| `RootAtBottom` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the bottom end of the capsule should be at the slot rather than the slot being at the middle. |
| `TargetHeight` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The slot to drive to influence the capsule collider's height. |
| `TargetWidth` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The slot to drive to influence the capsule collider's radius. |
| `TargetOffset` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The slot to drive to influence the capsule collider's center offset. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

Used in the default locomotions and is needed for a locomotion to adjust the character collider for a user properly.

## See Also

- [Type:ILocomotionModule](https://wiki.resonite.com/Type:ILocomotionModule "Type:ILocomotionModule")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SingleShapeCharacterControllerManager&oldid=95668](https://wiki.resonite.com/index.php?title=Component:SingleShapeCharacterControllerManager&oldid=95668)"

Contents