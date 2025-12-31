# Component:BoxPointGenerator

> Source: https://wiki.resonite.com/Component:BoxPointGenerator

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:BoxPointGenerator&diff=91188) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/56/BoxPointGeneratorComponent.png/510px-BoxPointGeneratorComponent.png)](https://wiki.resonite.com/File:BoxPointGeneratorComponent.png) **Box Point Generator** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

A generator for points arranged in a box with a given length, width, and height.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Size` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How big the box should be for generating points. |
| `Shell` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether points should only be spawned on the surface of the box or not. |

Fields
Collapse

## Usage

Used in a [Common Spawn Area](https://wiki.resonite.com/Component:CommonSpawnArea "Component:CommonSpawnArea") to define in what kind of spawn area shape users should initially spawn into.

## Examples

Can be used to spawn users on the outside of a cube world, with gravity on all 5 sides, at any place on the cube by making `Size` the size of the cube, and enabling `Shell`

## Related Components

- [Component:CommonSpawnArea](https://wiki.resonite.com/Component:CommonSpawnArea "Component:CommonSpawnArea")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BoxPointGenerator&oldid=91188](https://wiki.resonite.com/index.php?title=Component:BoxPointGenerator&oldid=91188)"

Contents