# Component:MirrorTransform

> Source: https://wiki.resonite.com/Component:MirrorTransform

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:MirrorTransform&diff=93035) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a7/MirrorTransformComponent.png/510px-MirrorTransformComponent.png)](https://wiki.resonite.com/File:MirrorTransformComponent.png) **Mirror Transform** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The Mirror Transform drives the position of the slot to mirror the position of an inputted slot across the normal of a plane.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `MirrorSource` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to get the mirror data from. |
| `MirrorPlane` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to use as the position to mirror across. |
| `MirrorOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | An offset from the `MirrorPlane` to mirror across. |
| `MirrorNormal` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The direction to mirror from. |
| `AllowWriteBack` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow changing the target fields of `_position` or `_rotation` to change the position and rotation of `MirrorSource`. |
| `_position` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field to drive with the mirrored mirror data. Usually the Position field of the slot this component is on. |
| `_rotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation field to drive with the mirrored mirror data. Usually the Rotation field of the slot this component is on. |

Fields
Collapse

## Usage

Attach to a slot and provide `MirrorSource`, `MirrorPlane`, and `MirrorNormal` for this component to start working.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MirrorTransform&oldid=93035](https://wiki.resonite.com/index.php?title=Component:MirrorTransform&oldid=93035)"

Contents