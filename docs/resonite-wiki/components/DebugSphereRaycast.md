# Component:DebugSphereRaycast

> Source: https://wiki.resonite.com/Component:DebugSphereRaycast

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a7/DebugSphereRaycastComponent.png/510px-DebugSphereRaycastComponent.png)](https://wiki.resonite.com/File:DebugSphereRaycastComponent.png) **Debug Sphere Raycast** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DebugSphereRaycast** component is used to show the multiple hit normals (1 per collider) of a sweep raycast of a sphere. This essentially acts as a fat raycast, which has thickness. Unfortunately this raycast is only for Debug purposes. Is simulated on the host machine.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

When using this component, you will feel lag.


![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This game element is a debug item. Elements like this may be removed at any time without warning, and creations should not rely on it.


## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Direction` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the direction and distance the raycast should go. |
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How far the raycasts created should go. |

Fields
Collapse

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DebugSphereRaycast&oldid=96394](https://wiki.resonite.com/index.php?title=Component:DebugSphereRaycast&oldid=96394)"

Contents