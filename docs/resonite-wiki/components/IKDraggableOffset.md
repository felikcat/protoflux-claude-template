# Component:IKDraggableOffset

> Source: https://wiki.resonite.com/Component:IKDraggableOffset

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/9f/IKDraggableOffsetComponent.png/510px-IKDraggableOffsetComponent.png)](https://wiki.resonite.com/File:IKDraggableOffsetComponent.png) **IKDraggable Offset** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **IKDraggableOffset** component is generated as part of newly imported humanoid avatars. It allows users to grab (meaning it's an [IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable")) and move parts of a model to test how it moves before making it an avatar.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Solver` | **[IKSolver](https://wiki.resonite.com/Type:IKSolver "Type:IKSolver")** | The IK solver that this is currently controlling. See IKSolver for what this could be. |
| `PositionTarget` | **[Sync\`1](https://wiki.resonite.com/Type:Sync%601 "Type:Sync`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | The position field to influence when grabbing. |
| `RotationTarget` | **[Sync\`1](https://wiki.resonite.com/Type:Sync%601 "Type:Sync`1") < [FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ") >** | The rotation field to influence when grabbing. |
| `Weight` | **[Sync\`1](https://wiki.resonite.com/Type:Sync%601 "Type:Sync`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The weight field to influence when grabbing. |
| `_grabber` | **[Grabber](https://wiki.resonite.com/Component:Grabber "Component:Grabber")** | The grabber component currently grabbing this. |
| `_grabbingUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user currently grabbing this. |
| `_holdSlot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot currently holding this component's slot for grabbing. |
| `_posOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position offset this component is applying to `Solver`. |
| `_rotOffset` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation offset this component is applying to `Solver`. |

Fields
Collapse

## Usage

This should not be used by the player, and is generated with newly imported humanoid avatars.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:VRIK](https://wiki.resonite.com/Component:VRIK "Component:VRIK")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:IKDraggableOffset&oldid=92452](https://wiki.resonite.com/index.php?title=Component:IKDraggableOffset&oldid=92452)"

Contents