# Component:HollowConeMesh

> Source: https://wiki.resonite.com/Component:HollowConeMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:HollowConeMesh&diff=97948) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e9/HollowConeMeshComponent.png/510px-HollowConeMeshComponent.png)](https://wiki.resonite.com/File:HollowConeMeshComponent.png) **Hollow Cone Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **HollowConeMesh** component is used to generate geometry for use with a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer"). This component generates a cone with a hollow center with internal geometry and a thickness. Similarly to the [ConeMesh](https://wiki.resonite.com/ConeMesh_(Component) "ConeMesh (Component)"), the height of this procedural mesh is determined from the center of the object.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `OverrideBoundingBox` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Force the bounding box calculated from this component to use `OverridenBoundingBox` instead of calculating when requested. |
| `OverridenBoundingBox` | **[BoundingBox](https://wiki.resonite.com/Type:BoundingBox "Type:BoundingBox")** | the bounding box this component should say it has when `OverrideBoundingBox` is enabled. Useful for bounding box calculations with Flux, or changing the selection box for this component when rendered. |
| `Profile` | **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | the profile of the colors of vertices for this mesh. |
| `Height` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how tall the hollow cone should be starting from the center |
| `OuterRadiusBase` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the radius of the bottom ring that makes up the outer tube |
| `InnerRadiusBase` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the radius if the bottom ring that makes up the inner tube |
| `OuterRadiusTop` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the radius of the top ring that makes up the outer tube |
| `InnerRadiusTop` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the radius of the top ring that makes up the inner tube |
| `Segments` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | how many faces make up each cylinder for the outside and inside. |
| `UVScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | how much to multiply the scale of the UVs for the procedural mesh. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

Attach to a slot and insert into a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") to view the geometry. Don't forget to use a [Material](https://wiki.resonite.com/Material "Material").

## Examples

[![](https://wiki.resonite.com/images/thumb/f/f3/HollowConeMesh.png/300px-HollowConeMesh.png)](https://wiki.resonite.com/File:HollowConeMesh.png) 2 HollowConeMeshes, one using an alpha material to demonstrate its hollow nature

## See Also

- [Component:ConeMesh](https://wiki.resonite.com/Component:ConeMesh "Component:ConeMesh")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:HollowConeMesh&oldid=97948](https://wiki.resonite.com/index.php?title=Component:HollowConeMesh&oldid=97948)"

Contents