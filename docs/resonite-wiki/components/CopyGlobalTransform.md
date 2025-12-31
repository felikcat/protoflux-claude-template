# Component:CopyGlobalTransform

> Source: https://wiki.resonite.com/Component:CopyGlobalTransform

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:CopyGlobalTransform&diff=91214) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/12/CopyGlobalTransformComponent.png/510px-CopyGlobalTransformComponent.png)](https://wiki.resonite.com/File:CopyGlobalTransformComponent.png) **Copy Global Transform** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The CopyGlobalTransform component is used to ensure that one object has the exact same global transform (position and rotation) as another object.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Source` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The object that serves as the transform reference. |
| `_posDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The field that is driven to match the global position of the source. This automatically gets populated with the position field of the slot that this component is added to. |
| `_rotDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The field that is driven to match the global rotation of the source. This automatically gets populated with the rotation field of the slot that this component is added to. |

Fields
Collapse

## Usage

## Examples

- [CopyGlobalTransform tutorial](https://www.youtube.com/watch?v=ODIgDRLyJRo) by [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CopyGlobalTransform&oldid=91214](https://wiki.resonite.com/index.php?title=Component:CopyGlobalTransform&oldid=91214)"

Contents