# Component:SmoothTransform

> Source: https://wiki.resonite.com/Component:SmoothTransform

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:SmoothTransform&diff=91480) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e3/SmoothTransformComponent.png/510px-SmoothTransformComponent.png)](https://wiki.resonite.com/File:SmoothTransformComponent.png) **Smooth Transform** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Smooth transform is a component that is used to create a "lag behind" or "trailing" effect on slots or objects that follow another object. The slot this controls will try to return to it's rest position, iteratively getting closer and closer until in eventuality reaching it's target location at rest.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `InterpolationSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The coordinate space that should be used to check the delta of the transforms in. If set to user space and parented under the user's hand, this slot will only lag behind (or smooth) when the user moves their hand, but not when they walk around. This can also be set to a slot for similar effects without a user. |
| `TargetPosition` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The local transform position that this slot is trying to get to. |
| `TargetRotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | the local transform rotation that this slot is trying to get to. |
| `TargetScale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The local transform scale that this slot is trying to get to. |
| `Position` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position field to drive with the smoothed value (auto filled with the position field of the slot this is on. |
| `Rotation` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation field to drive with the smoothed value (auto filled with the rotation field of the slot this is on. |
| `Scale` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The scale field to drive with the smoothed value (auto filled with the scale field of the slot this is on. |
| `SmoothSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast or slow this slot is at catching up to it's target location. Not a set number of seconds since this component iteratively smooths. |
| `_updateIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Whether to do this smooth transform before or after other smooth transforms in the same slot hiearchy. |

Fields
Collapse

## Usage

## Examples

Useful in making a little fairy that follows the user around. Or a trail of orbs that float along side the user. Or floating accessories/horns/trinkets that are attached to a user that follow them around. Or an object that loosely follows a racing ship.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SmoothTransform&oldid=91480](https://wiki.resonite.com/index.php?title=Component:SmoothTransform&oldid=91480)"

Contents