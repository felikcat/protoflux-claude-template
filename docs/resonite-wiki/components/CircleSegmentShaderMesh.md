# Component:CircleSegmentShaderMesh

> Source: https://wiki.resonite.com/Component:CircleSegmentShaderMesh

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/7a/CircleSegmentShaderMeshComponent.png/510px-CircleSegmentShaderMeshComponent.png)](https://wiki.resonite.com/File:CircleSegmentShaderMeshComponent.png) **Circle Segment Shader Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **CircleSegmentShaderMesh** creates a single quad that covers the bounding box area of a flat torus circle defined by the given values. This is used to render the [Component:UI\_CircleSegment](https://wiki.resonite.com/Component:UI_CircleSegment "Component:UI CircleSegment") material.

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
| `RadiusStart` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The inner radius of the circle |
| `Thickness` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How thick the circle is outwards from the inner radius |
| `AngleStart` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | What angle the circle starts at in degrees |
| `ArcLength` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The amount of degrees of the circle arch |
| `FillColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Used to color the vertices of the mesh (vertex colors) |
| `BorderColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The border color the [Component:UI\_CircleSegment](https://wiki.resonite.com/Component:UI_CircleSegment "Component:UI CircleSegment") rendering on this mesh. |
| `BorderSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The border thickness of the [Component:UI\_CircleSegment](https://wiki.resonite.com/Component:UI_CircleSegment "Component:UI CircleSegment") rendering on this mesh. |
| `RoundedCornerRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the corner rounding of the [Component:UI\_CircleSegment](https://wiki.resonite.com/Component:UI_CircleSegment "Component:UI CircleSegment") rendering on this mesh. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

Used as a mesh to render the [Component:UI\_CircleSegment](https://wiki.resonite.com/Component:UI_CircleSegment "Component:UI CircleSegment") material.

## Examples

## See Also

- [Component:UI\_CircleSegment](https://wiki.resonite.com/Component:UI_CircleSegment "Component:UI CircleSegment")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CircleSegmentShaderMesh&oldid=97892](https://wiki.resonite.com/index.php?title=Component:CircleSegmentShaderMesh&oldid=97892)"

Contents