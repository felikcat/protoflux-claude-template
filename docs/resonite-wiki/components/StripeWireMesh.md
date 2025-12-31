# Component:StripeWireMesh

> Source: https://wiki.resonite.com/Component:StripeWireMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:StripeWireMesh&diff=98085) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c9/StripeWireMeshComponent.png/510px-StripeWireMeshComponent.png)](https://wiki.resonite.com/File:StripeWireMeshComponent.png) **Stripe Wire Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **StripeWireMesh** component is used primarily in ProtoFlux wires, and generates mesh data for use with a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer").

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
| `Point0` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The start point in local space for this mesh |
| `Point1` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The end point for this mesh in local space. |
| `Tangent0` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the direction the mesh should bend after exiting start point |
| `Tangent1` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the direction the mesh should bend while entering exit point. |
| `Orientation0` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | How much to rotate the starting point edge by after applying `Tangent0` |
| `Orientation1` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | How much to rotate the end point edge by after applying `Tangent1` |
| `Steps` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | how many segments the mesh should have between `Point0` and `Point1`. |
| `Exp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how much the mesh should be forced in the direction of the start and end tangents when starting and ending it's path. |
| `Color0` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The vertex color to give the part of the mesh starting at `Point0`. Is interpolated along the mesh to `Point1` to color `Color1` |
| `Color1` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The vertex color for `Point1` to interpolate towards. |
| `UVScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | the scale of the material detail on the mesh. |
| `UVOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | the offset of the material detail on the mesh. |
| `Width0` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the width of the mesh in local space at `Point0` on the mesh. Is interpolated along the mesh to `Point1` to width `Width1` |
| `Width1` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The width in local space for `Point1` to interpolate towards. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

Attach to a slot and insert into a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") to view the geometry generated. Don't forget to add a [Material](https://wiki.resonite.com/Material "Material").

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:StripeWireMesh&oldid=98085](https://wiki.resonite.com/index.php?title=Component:StripeWireMesh&oldid=98085)"

Contents