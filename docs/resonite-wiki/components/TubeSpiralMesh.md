# Component:TubeSpiralMesh

> Source: https://wiki.resonite.com/Component:TubeSpiralMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:TubeSpiralMesh&diff=98101) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/8e/TubeSpiralMeshComponent.png/510px-TubeSpiralMeshComponent.png)](https://wiki.resonite.com/File:TubeSpiralMeshComponent.png) **Tube Spiral Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TubeSpiralMesh** component is a procedural Mesh that looks like a corkscrew often seen on the end of a wine bottle opener.

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
| `Steps` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many length wise subdivisions the tube mesh has. |
| `MaximumDistanceBetweenRings` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The distance allowed between each segment before the amount of steps are reduced. |
| `CoilCount` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How many winds around the center the coil should have. |
| `ScaleCoilCountByLength` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the distance between coils stays consistent as the length grows by adding more coils. |
| `CoilPhase` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to offset the coil starting angle. |
| `StartPoint` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The center point position of what the Spiral is spiraling around at the beginning. |
| `StartTangent` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The bend towards bias position of the Spiral at the beginning. Makes the Spiral sheer or warp towards this point at the beginning. |
| `EndPoint` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The center point position of what the Spiral is spiraling around at the end. |
| `EndTangent` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The bend towards bias position of the Spiral at the end. Makes the Spiral sheer or warp towards this point at the end. lerps from beginning. |
| `StartSpiralRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance from the center to the Spiral tube center at the beginning. |
| `EndSpiralRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance from the center to the Spiral tube center at the end. |
| `StartSpiralOrientation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation of each segment ring at the start. |
| `EndSpiralOrientation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation of each segment ring at the end. Lerps from start. |
| `Ends` | **[Ends](https://wiki.resonite.com/Type:Ends "Type:Ends")** | How the ends should be sealed if at all on the corkscrew. |
| `Shading` | **[Shading](https://wiki.resonite.com/Type:Shading "Type:Shading")** | The Shading of the screw geometry. |
| `StartTubeRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of each segment at the start. |
| `EndTubeRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of each segment at the end. Lerps from start. |
| `TubePoints` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many sides the tube has circumference wise on each segment. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

Attach to a slot and put into a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") with a material to see what it looks like.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TubeSpiralMesh&oldid=98101](https://wiki.resonite.com/index.php?title=Component:TubeSpiralMesh&oldid=98101)"

Contents