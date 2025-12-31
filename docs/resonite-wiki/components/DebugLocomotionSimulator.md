# Component:DebugLocomotionSimulator

> Source: https://wiki.resonite.com/Component:DebugLocomotionSimulator

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/30/DebugLocomotionSimulatorComponent.png/510px-DebugLocomotionSimulatorComponent.png)](https://wiki.resonite.com/File:DebugLocomotionSimulatorComponent.png) **Debug Locomotion Simulator** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DebugLocomotionSimulator** component is used to draw Debug visuals for a virtual locomotion simulator that drives the procedural animation system.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This game element is a debug item. Elements like this may be removed at any time without warning, and creations should not rely on it.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TrackPosition` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to keep track of this Debug locomotion's progressively moving position. |
| `State` | **[LocomotionState](https://wiki.resonite.com/index.php?title=Type:LocomotionState&action=edit&redlink=1 "Type:LocomotionState (page does not exist)")** | The kind of locomotion this is debugging |
| `MovementSpeed` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How fast the locomotion should be moving. |
| `AngularSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast this locomotion should be turning. |
| `RotateDirection` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the locomotion should rotate its movement direction. |
| `OffsetRoot` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this locomotion should be offsetting from root as a starting position |

Fields
Collapse

## Examples

Used in some Frooxius devlog videos where he shows the in progress procedural animation system.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DebugLocomotionSimulator&oldid=96402](https://wiki.resonite.com/index.php?title=Component:DebugLocomotionSimulator&oldid=96402)"

Contents