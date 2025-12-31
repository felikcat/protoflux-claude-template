# Component:ArrowMesh

> Source: https://wiki.resonite.com/Component:ArrowMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ArrowMesh&diff=97851) which are not marked for translation.

Arrow Mesh is a procedural [Asset](https://wiki.resonite.com/Type:IAsset%601 "Type:IAsset`1") mesh that generates a cylinder with a cone on the end. Like a 3d arrow. The Arrow Mesh allows for vertex color customization, as well as defining a shape and a direction, aka a Vector.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c1/ArrowMeshComponent.png/510px-ArrowMeshComponent.png)](https://wiki.resonite.com/File:ArrowMeshComponent.png) **Arrow Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

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
| `Vector` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the direction in local space of the mesh render rendering this arrow that the arrow should point towards. Also defines the length. For more information on Local Space, see [Coordinate Spaces](https://wiki.resonite.com/Coordinate_Spaces "Coordinate Spaces") |
| `Sides` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | how many sides the cone and cylinder of this arrow should have. |
| `BodyRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Determines the thickness of the base under the arrow. |
| `HeadRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Determines the radius of the arrows head's base. |
| `HeadLength` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Determines the length of the arrow's head. |
| `MinimalBodyLength` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Determines the arrow's length at minimum. In case the provided `Vector`'s magnitude is less than this number. |
| `SphereOnZero` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | whether the arrow should render as a sphere instead when the `Vector` is (0,0,0) |
| `BodyUVScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | the scale multipler of the uvs on the cylinder body. Uvs of the cylinder is the same as a procedural cylinder. |
| `BodyUVOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | the shifted offset of the uvs for the cylinder body in 2d space |
| `HeadUVScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | the scale multiplier of the uvs on the cone head. Uv of the cone is the same as a procedural cone. |
| `HeadUVOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | the shifted offset of the uvs for the cone head in 2d space |
| `BaseColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color of the vertices of the bottom edge of the arrow. |
| `TopColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color of the vertices of the top edge of the arrow. |
| `HeadColor` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | Color of the vertices of the head of the arrow. |

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

Can be used to determine the direction an object is traveling. The vector can be driven using flux and is useful for debugging in cases where the [Debug Vector Flux Node](https://wiki.resonite.com/ProtoFlux:Debug_Vector "ProtoFlux:Debug Vector") is not very practical.

The arrow mesh is also used in Gizmos to draw the 3 arrow axes in the visual.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ArrowMesh&oldid=97851](https://wiki.resonite.com/index.php?title=Component:ArrowMesh&oldid=97851)"

Contents