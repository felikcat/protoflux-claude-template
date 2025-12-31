# Component:CrossMesh

> Source: https://wiki.resonite.com/Component:CrossMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:CrossMesh&diff=97909) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/0b/CrossMeshComponent.png/510px-CrossMeshComponent.png)](https://wiki.resonite.com/File:CrossMeshComponent.png) **Cross Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **CrossMesh** component is a 3D mesh made of 3 crossing boxes of equal thickness and length. It can be rotated, and the bars can be lengthened and thickened/thinned.

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
| `Size` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The size of the cross from end to end in local space. |
| `BarRatio` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | This multiplied by size is how thick each bar is in local space. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

Attach to a slot, and assign to a [Mesh Renderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") to see what it looks like. Don't forget to use a material.

## Examples

Can be used to mark a point with a rotation like markers for debug testing.

An example of what a default rotated cross mesh looks like

[![](https://wiki.resonite.com/images/thumb/4/4d/CrossMesh.png/500px-CrossMesh.png)](https://wiki.resonite.com/File:CrossMesh.png)

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CrossMesh&oldid=97909](https://wiki.resonite.com/index.php?title=Component:CrossMesh&oldid=97909)"

Contents