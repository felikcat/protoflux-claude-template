# Component:CylinderMesh

> Source: https://wiki.resonite.com/Component:CylinderMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:CylinderMesh&diff=97913) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/1c/CylinderMeshComponent.png/510px-CylinderMeshComponent.png)](https://wiki.resonite.com/File:CylinderMeshComponent.png) **Cylinder Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **CylinderMesh** component is used to provide a mesh to render. The mesh that it provides is a procedural 3D cylinder with a number of sides and a radius.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `OverrideBoundingBox` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Force the bounding box calculated from this component to use `OverridenBoundingBox` instead of calculating when requested. |
| `OverridenBoundingBox` | **[BoundingBox](https://wiki.resonite.com/Type:BoundingBox "Type:BoundingBox")** | the bounding box this component should say it has when `OverrideBoundingBox` is enabled. Useful for bounding box calculations with Flux, or changing the selection box for this component when rendered. |
| `Profile` | **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | The profile that the vertex colors for this mesh should be displayed in. |
| `Height` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The height of the cylinder in meters in local space. |
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the cylinder in meters in local space. |
| `Sides` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many sides the cylinder should have around it's midsection. |
| `Caps` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the cylinder should be a tube or not. |
| `FlatShading` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Disable smooth shading. |
| `UVScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The inverse of the size the material should appear on the surface as. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

Attach to a slot, and assign to a [Mesh Renderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") to see what it looks like. Don't forget to use a [Material](https://wiki.resonite.com/Material "Material").

## Examples

An example of what a default rotated cylinder mesh looks like

[![](https://wiki.resonite.com/images/thumb/2/21/Cylinder.png/500px-Cylinder.png)](https://wiki.resonite.com/File:Cylinder.png)

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CylinderMesh&oldid=97913](https://wiki.resonite.com/index.php?title=Component:CylinderMesh&oldid=97913)"

Contents