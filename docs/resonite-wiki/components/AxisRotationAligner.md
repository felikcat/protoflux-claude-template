# Component:AxisRotationAligner

> Source: https://wiki.resonite.com/Component:AxisRotationAligner

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AxisRotationAligner&diff=96156) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/ea/AxisRotationAlignerComponent.png/510px-AxisRotationAlignerComponent.png)](https://wiki.resonite.com/File:AxisRotationAlignerComponent.png) **Axis Rotation Aligner** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AxisRotationAligner** can be used to keep a slot facing a direction relative to a space.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `LocalDirection` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | A vector direction in this slot's local space to align to `TargetDirection` via rotating this slot. |
| `TargetDirection` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The direction vector to align to. |
| `DirectionSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The coordinate space that `TargetDirection` is in. |
| `LocalRotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | A rotation offset to the alignment. |
| `_rotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation field of the slot this component is on. Is driven to do the rotation alignment. |

Fields
Collapse

## Usage

The defined `LocalDirection` will be rotated to line up with the `TargetDirection` inside `DirectionSpace`'s coordinate space.

## Examples

A common use of the **AxisRotationAligner** is to make a slot's upward direction always match the upward direction of root.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AxisRotationAligner&oldid=96156](https://wiki.resonite.com/index.php?title=Component:AxisRotationAligner&oldid=96156)"

Contents