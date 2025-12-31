# Component:SpherePointGenerator

> Source: https://wiki.resonite.com/Component:SpherePointGenerator

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:SpherePointGenerator&diff=91190) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/17/SpherePointGeneratorComponent.png/510px-SpherePointGeneratorComponent.png)](https://wiki.resonite.com/File:SpherePointGeneratorComponent.png) **Sphere Point Generator** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

A generator for points arranged in a sphere with a given radius. Used in [Common Spawn Areas](https://wiki.resonite.com/Component:CommonSpawnArea "Component:CommonSpawnArea") usually.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How big the sphere should be for generating points in |
| `Shell` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether or not to generate points on the outside edge rather than inside the sphere too. |

Fields
Collapse

## Usage

Used in a [Common Spawn Area](https://wiki.resonite.com/Component:CommonSpawnArea "Component:CommonSpawnArea") to define in what kind of spawn area shape users should initially spawn into.

## Examples

Can be used to spawn users inside of a zero gravity arena, or on the surface of a round planet, or on the inside of a dyson sphere at a random point.

## Related Components

- [Component:CommonSpawnArea](https://wiki.resonite.com/Component:CommonSpawnArea "Component:CommonSpawnArea")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SpherePointGenerator&oldid=91190](https://wiki.resonite.com/index.php?title=Component:SpherePointGenerator&oldid=91190)"

Contents