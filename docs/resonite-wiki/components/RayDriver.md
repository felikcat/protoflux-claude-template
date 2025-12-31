# Component:RayDriver

> Source: https://wiki.resonite.com/Component:RayDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:RayDriver&diff=91525) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2d/RayDriverComponent.png/510px-RayDriverComponent.png)](https://wiki.resonite.com/File:RayDriverComponent.png) **Ray Driver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

A ray driver is a component that takes a start origin and a direction and drives point A and B via a RayCast, keeping the distance between the two below MaxDistance.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `MaxDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the max distance that A and B can be from each other |
| `PointA` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[Sync\`1](https://wiki.resonite.com/Type:Sync%601 "Type:Sync`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | what to drive with the local space start position of the Raycast |
| `PointB` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[Sync\`1](https://wiki.resonite.com/Type:Sync%601 "Type:Sync`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | what to drive with the local space end point of the raycast |
| `LocalOrigin` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the local space start point of the raycast |
| `LocalDirection` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the direction in local space to fire the raycast in. |

Fields
Collapse

## Usage

- [LaserPointer Tool with RayDriver](https://www.youtube.com/watch?v=uQL-jwI-NFI) by [ProbablePrime](https://wiki.resonite.com/User:ProbablePrime "User:ProbablePrime")

## Examples

Laser pointer or grapple hook. This can be used as a lighter weight version of the [Raycast driver component](https://wiki.resonite.com/Component:RaycastDriver "Component:RaycastDriver")

## Related Components

[RaycastDriver component](https://wiki.resonite.com/Component:RaycastDriver "Component:RaycastDriver")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RayDriver&oldid=91525](https://wiki.resonite.com/index.php?title=Component:RayDriver&oldid=91525)"

Contents