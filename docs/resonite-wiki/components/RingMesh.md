# Component:RingMesh

> Source: https://wiki.resonite.com/Component:RingMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:RingMesh&diff=98423) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/72/RingMeshComponent.png/510px-RingMeshComponent.png)](https://wiki.resonite.com/File:RingMeshComponent.png) **Ring Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

A ring mesh is a component that generates a ring of quads that has an `InnerRadius`, `OuterRadius`, and resolution which is the `Segments` field.

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
| `Rotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | Rotate the entire mesh by this. |
| `Segments` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | how sub divisions length wise this ring mesh has (smoothness of the arc) |
| `Arc` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how much of a circle from 0<->360 this mesh should take up. |
| `InnerRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the inner circle of this ring mesh. |
| `OuterRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the outer circle of this ring mesh. |
| `UVScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The scale of material details and colors on the mesh. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

## Examples

## Related Components

- [BevelRingMesh](https://wiki.resonite.com/Component:BevelRingMesh "Component:BevelRingMesh")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RingMesh&oldid=98423](https://wiki.resonite.com/index.php?title=Component:RingMesh&oldid=98423)"

Contents