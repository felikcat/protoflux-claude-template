# Component:CurvedPlaneMesh

> Source: https://wiki.resonite.com/Component:CurvedPlaneMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:CurvedPlaneMesh&diff=106530) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/29/CurvedPlaneMeshComponent.png/510px-CurvedPlaneMeshComponent.png)](https://wiki.resonite.com/File:CurvedPlaneMeshComponent.png) **Curved Plane Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Generates a plane mesh that is curved vertically. A picture in this page of it can be seen.

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
| `Size` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | How big the curve plane mesh is, mostly a ratio |
| `Curvature` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to bend the curve plane mesh by |
| `TiltAngle` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to "rotate" the curve plane mesh length wise. |
| `AspectRatioCompensation` | **[CurvedPlaneMesh.CurvatureAspectRatioCompensation](https://wiki.resonite.com/Component:CurvedPlaneMesh#CurvatureAspectRatioCompensation)** | How to compensate for stretching due to curving the plane mesh backwards. |
| `UVScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The inverse of the size the material should appear on the surface as. |
| `UVOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | Shift the visual detail of the material around. |
| `Segments` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many bends/angles the plane should have in it's curve |
| `FlatShading` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Turn off smooth shading |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## CurvatureAspectRatioCompensation

| Name | Value | Description |
| --- | --- | --- |
| `None` | 0 | No Compensation. |
| `IncreaseHeight` | 1 | Increase the mesh size vertically to compensate. |
| `DecreaseWidth` | 2 | Decrease the mesh size width to compensate. |

Values

## Usage

Attach to a slot and insert into a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") to see the geometry. don't forget to use a [Material](https://wiki.resonite.com/Material "Material").

## Examples

The curve plane mesh is most notably used for the curvature of the VR [Dash Menu](https://wiki.resonite.com/Dash_Menu "Dash Menu").

What a curved plane mesh looks like.

[![](https://wiki.resonite.com/images/thumb/c/cb/CurvedPlaneMesh.png/500px-CurvedPlaneMesh.png)](https://wiki.resonite.com/File:CurvedPlaneMesh.png)

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CurvedPlaneMesh&oldid=106530](https://wiki.resonite.com/index.php?title=Component:CurvedPlaneMesh&oldid=106530)"

Contents