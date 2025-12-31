# Component:SquarePointGenerator

> Source: https://wiki.resonite.com/Component:SquarePointGenerator

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:SquarePointGenerator&diff=91191) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/f1/SquarePointGeneratorComponent.png/510px-SquarePointGeneratorComponent.png)](https://wiki.resonite.com/File:SquarePointGeneratorComponent.png) **Square Point Generator** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

A generator for points arranged in a rectangle with a given length and width.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Size` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | A flat rectangle size for generating points in |
| `Shell` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to spawn users on only the perimeter or not. |

Fields
Collapse

## Usage

Used in a [Common Spawn Area](https://wiki.resonite.com/Component:CommonSpawnArea "Component:CommonSpawnArea") to define in what kind of spawn area shape users should initially spawn into.

## Examples

Can be used in cases where a circle spawn area is too inaccurate to spawn users in. This can happen in cases like: Hallway spawns, elevator spawns, or any room that is square or rectangular.

## Related Components

- [Component:CommonSpawnArea](https://wiki.resonite.com/Component:CommonSpawnArea "Component:CommonSpawnArea")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SquarePointGenerator&oldid=91191](https://wiki.resonite.com/index.php?title=Component:SquarePointGenerator&oldid=91191)"

Contents