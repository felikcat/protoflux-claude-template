# Component:EyeRotationDriver

> Source: https://wiki.resonite.com/Component:EyeRotationDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:EyeRotationDriver&diff=97486) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/08/EyeRotationDriverComponent.png/510px-EyeRotationDriverComponent.png)](https://wiki.resonite.com/File:EyeRotationDriverComponent.png) **EyeRotationDriver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

_This article or section is a stub. You can help the Resonite wiki by expanding it._

The **EyeRotationDriver** component can control the rotation of slots using the data from an [EyeManager](https://wiki.resonite.com/Component:EyeManager "Component:EyeManager").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `EyeManager` | **[EyeManager](https://wiki.resonite.com/Component:EyeManager "Component:EyeManager")** | The source of the eye rotation data. |
| `EyeMotionScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to multiply the target rotation by before applying it to an [Eye](https://wiki.resonite.com/Component:EyeRotationDriver#Eye). |
| `EyeMotionExp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The exponent. This makes the eye rotate more or less as it reaches higher rotation target values. |
| `MaxSwing` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum amount the eyes can rotate in degrees from forward facing. |
| `Eyes` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[EyeRotationDriver.Eye](https://wiki.resonite.com/Component:EyeRotationDriver#Eye)** | A list of eyes to drive the rotation of. |

Fields
Collapse

## Eye

| Name | Type | Description |
| --- | --- | --- |
| `Side` | **[EyeSide](https://wiki.resonite.com/Type:EyeSide "Type:EyeSide")** | Left or right eye. |
| `Root` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | the slot of this eye that should be rotated |
| `Up` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The up direction of `Root` in local space. |
| `Forward` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The forward direction of `Root` in local space. |
| `Rotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation field of `Root` to drive. |

Fields

==

## Usage

Set up automatically on avatars that are made using the [Avatar Creator](https://wiki.resonite.com/Avatar_Creator "Avatar Creator").

## Examples

## See Also

- [Component:EyeManager](https://wiki.resonite.com/Component:EyeManager "Component:EyeManager")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:EyeRotationDriver&oldid=97486](https://wiki.resonite.com/index.php?title=Component:EyeRotationDriver&oldid=97486)"

Contents