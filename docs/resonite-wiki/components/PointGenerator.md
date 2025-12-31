# Component:PointGenerator

> Source: https://wiki.resonite.com/Component:PointGenerator

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:PointGenerator&diff=91189) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/ff/PointGeneratorComponent.png/510px-PointGeneratorComponent.png)](https://wiki.resonite.com/File:PointGeneratorComponent.png) **Point Generator** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Generates points only at a single point which is the position of the slot this component is on.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |

Fields
Collapse

## Usage

Used in a [Common Spawn Area](https://wiki.resonite.com/Component:CommonSpawnArea "Component:CommonSpawnArea") to define in what kind of spawn area shape users should initially spawn into. In this case, it spawns them at the exact location of the component's slot.

## Examples

Can be used to spawn the user very precicely, like how players would spawn in some old PVP games or the positions for players in CSGO.

## Related Components

- [Component:CommonSpawnArea](https://wiki.resonite.com/Component:CommonSpawnArea "Component:CommonSpawnArea")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PointGenerator&oldid=91189](https://wiki.resonite.com/index.php?title=Component:PointGenerator&oldid=91189)"

Contents