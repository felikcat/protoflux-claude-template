# Component:Laser

> Source: https://wiki.resonite.com/Component:Laser

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/76/LaserComponent.png/510px-LaserComponent.png)](https://wiki.resonite.com/File:LaserComponent.png) **Laser** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Laser** component creates a simple red laser when attached that raycasts the enviroment.

When added to a slot the Laser component creates a [MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer"), a [SegmentMesh](https://wiki.resonite.com/Component:SegmentMesh "Component:SegmentMesh"), a [RayDriver](https://wiki.resonite.com/Component:RayDriver "Component:RayDriver"), and a red [PBS RimMetallic](https://wiki.resonite.com/PBS_RimMetallic "PBS RimMetallic").

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_material` | **[PBS\_RimMetallic](https://wiki.resonite.com/PBS_RimMetallic "PBS RimMetallic")** | The material to use for the laser. |
| `_rayDriver` | **[RayDriver](https://wiki.resonite.com/Component:RayDriver "Component:RayDriver")** | The ray driver driving the generated segment mesh. |
| `_meshRenderer` | **[MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer")** | The mesh renderer rendering the segment mesh for this laser pointer type component. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Laser&oldid=94803](https://wiki.resonite.com/index.php?title=Component:Laser&oldid=94803)"

Contents