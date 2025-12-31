# Component:TubeWireMesh

> Source: https://wiki.resonite.com/Component:TubeWireMesh

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/24/TubeWireMeshComponent.png/510px-TubeWireMeshComponent.png)](https://wiki.resonite.com/File:TubeWireMeshComponent.png) **Tube Wire Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **TubeWireMesh** component acts as a source of procedural Mesh data. This creates a mesh like the [Component:StripeWireMesh](https://wiki.resonite.com/Component:StripeWireMesh "Component:StripeWireMesh") but is a tube instead.

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
| `Point0` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The starting point for the tube mesh. |
| `Point1` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The ending point for the tube mesh. |
| `Tangent0` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The bend towards point at the beginning. |
| `Tangent1` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The bend towards point at the end. |
| `Orientation0` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation of the end cap at the beginning of the tube. |
| `Orientation1` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation of the end cap at the end of the tube. |
| `Steps` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many length wise subdivisions there is. |
| `Exp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to stretch mesh geometry towards the tangent points. |
| `Color0` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the vertex colors at the starting point. |
| `Color1` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the vertex colors at the ending point. |
| `UVScale` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The scale of the texture detail on this mesh's surface. |
| `UVOffset` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The offset of the texture detail on this mesh's surface. |
| `Radius0` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The starting radius of the tube. |
| `Radius1` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The ending radius of the tube. |
| `Ends` | **[Ends](https://wiki.resonite.com/Type:Ends "Type:Ends")** | How to seal the ends of the mesh, if at all. |
| `Shading` | **[Shading](https://wiki.resonite.com/Type:Shading "Type:Shading")** | How to shade the tube. |
| `Points` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many subdivisions circumference wise the tube has. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

Attach to a slot, then insert into a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") with a material to view what this mesh looks like.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:StripeWireMesh](https://wiki.resonite.com/Component:StripeWireMesh "Component:StripeWireMesh")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:TubeWireMesh&oldid=98102](https://wiki.resonite.com/index.php?title=Component:TubeWireMesh&oldid=98102)"

Contents