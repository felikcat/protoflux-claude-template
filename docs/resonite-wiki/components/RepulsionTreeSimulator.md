# Component:RepulsionTreeSimulator

> Source: https://wiki.resonite.com/Component:RepulsionTreeSimulator

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/89/RepulsionTreeSimulatorComponent.png/510px-RepulsionTreeSimulatorComponent.png)](https://wiki.resonite.com/File:RepulsionTreeSimulatorComponent.png) **Repulsion Tree Simulator** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

_This article or section is a stub. You can help the Resonite wiki by expanding it._

The RepulsionTreeSimulator can be used alongside the [RepulsionTreeItem](https://wiki.resonite.com/Component:RepulsionTreeItem "Component:RepulsionTreeItem") component on it's children slots to create a repulsion tree simulation. A repulsion tree is a simulation that keeps a bunch of [RepulsionTreeItems](https://wiki.resonite.com/Component:RepulsionTreeItem "Component:RepulsionTreeItem") on the outside shell of a sphere. The different slots of the tree will move around as they push or pull each other in real time.

![](https://wiki.resonite.com/images/b/b7/DangerIcon.svg)

This does lots of writes to every slot under it, this is experimental and users should not use it in a populated session due to the amount of network traffic it generates.


## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `FalloffPower` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how quickly the force power diminishes by distance. |
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of this repulsion tree's sphere. |
| `Force` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how much to multiply the forces of the children objects. |

Fields
Collapse

## Behavior

## Examples

## See Also

[RepulsionTreeItem](https://wiki.resonite.com/Component:RepulsionTreeItem "Component:RepulsionTreeItem")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RepulsionTreeSimulator&oldid=91449](https://wiki.resonite.com/index.php?title=Component:RepulsionTreeSimulator&oldid=91449)"

Contents