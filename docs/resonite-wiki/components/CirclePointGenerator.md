# Component:CirclePointGenerator

> Source: https://wiki.resonite.com/Component:CirclePointGenerator

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:CirclePointGenerator&diff=91187) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/54/CirclePointGeneratorComponent.png/510px-CirclePointGeneratorComponent.png)](https://wiki.resonite.com/File:CirclePointGeneratorComponent.png) **Circle Point Generator** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

A generator for points arranged in a circle with a given radius.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance from center to outside that this point generator should make points. |
| `Shell` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Generate the points for this generator only along the outside edge. |

Fields
Collapse

## Usage

Used in a [Common Spawn Area](https://wiki.resonite.com/Component:CommonSpawnArea "Component:CommonSpawnArea") to define in what kind of spawn area shape users should initially spawn into.

## Examples

Used in the default spawn area object in any flat grid world.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CirclePointGenerator&oldid=91187](https://wiki.resonite.com/index.php?title=Component:CirclePointGenerator&oldid=91187)"

Contents