# Component:SimpleUserSpawn

> Source: https://wiki.resonite.com/Component:SimpleUserSpawn

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:SimpleUserSpawn&diff=106342) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/67/SimpleUserSpawnComponent.png/510px-SimpleUserSpawnComponent.png)](https://wiki.resonite.com/File:SimpleUserSpawnComponent.png) **SimpleUserSpawn** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SimpleUserSpawn** component is used to have a simple way of [users](https://wiki.resonite.com/User "User") spawning into a [world](https://wiki.resonite.com/World "World"), with no optional parameters to fill in. In contrast, the [CommonSpawnArea](https://wiki.resonite.com/Component:CommonSpawnArea "Component:CommonSpawnArea") component is similar to this but with those extra options.

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |

Fields
Collapse

## Usage

A **SimpleUserSpawn** defines a simple spawn point. New and respawning users will be placed with their avatar as a child of the world's [root](https://wiki.resonite.com/Root "Root") at `0,0,0`, facing the Z- direction. The position and rotation of this component's slot have no bearing on the user's position or rotation.

## Examples

## Related Components

- [SpawnArc](https://wiki.resonite.com/SpawnArc_(Component) "SpawnArc (Component)")
- [CommonSpawnArea](https://wiki.resonite.com/CommonSpawnArea_(Component) "CommonSpawnArea (Component)")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SimpleUserSpawn&oldid=106342](https://wiki.resonite.com/index.php?title=Component:SimpleUserSpawn&oldid=106342)"

Contents