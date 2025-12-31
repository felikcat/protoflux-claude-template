# Component:BentTubeMesh

> Source: https://wiki.resonite.com/Component:BentTubeMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:BentTubeMesh&diff=97869) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2e/BentTubeMeshComponent.png/510px-BentTubeMeshComponent.png)](https://wiki.resonite.com/File:BentTubeMeshComponent.png) **Bent Tube Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Bent tube mesh is a component that makes a tube structure.

When calculating the curve, the generator uses a quadratic bezier curve formula. `StartPoint` being P0, `DirectTargetPoint` being P1, and `ActualTargetPoint` being P2.

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
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the tube (from center to outside). |
| `Sides` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many sides the tube should have around it |
| `Segments` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | how many bends from end to end the tube should have |
| `StartPoint` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Where the tube should start at in local space. Also known as P0 on a quadratic bezier curve. |
| `DirectTargetPoint` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | P1 on the quadratic bezier curve in local space. |
| `ActualTargetPoint` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | P2 on the quadratic bezier curve in local space. |
| `StartPointColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | What the color of the tube should be at the start if using a material that supports vertex colors. |
| `EndPointColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | What the color of the tube should be at the end if using a material that supports vertex colors. |
| `Ends` | **[Ends](https://wiki.resonite.com/Type:Ends "Type:Ends")** | How to handle the geometry of the ends of the tube. |
| `Shading` | **[Shading](https://wiki.resonite.com/Type:Shading "Type:Shading")** | Toggle this mesh being smooth shaded |

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

Useful for making railings, or making rails

## See Also

- [Component:BallisticPathMesh](https://wiki.resonite.com/Component:BallisticPathMesh "Component:BallisticPathMesh")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BentTubeMesh&oldid=97869](https://wiki.resonite.com/index.php?title=Component:BentTubeMesh&oldid=97869)"

Contents