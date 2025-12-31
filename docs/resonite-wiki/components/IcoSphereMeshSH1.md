# Component:IcoSphereMeshSH1

> Source: https://wiki.resonite.com/Component:IcoSphereMeshSH1

Collapse **Component image**

[File:IcoSphereMeshSH1Component.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=IcoSphereMeshSH1Component.png "File:IcoSphereMeshSH1Component.png") **Ico Sphere Mesh SH1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Ico Sphere Mesh SH1** component creates Ico Sphere data using Sphercal harmonics.

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
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The radius of the ico sphere visual. |
| `Subdivisions` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How detailed the mesh is. |
| `FlatShading` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the mesh should be flat shaded. |
| `FlatFaceExtrude` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to puff up the mesh. |
| `FlatFaceScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to scale up the faces of the mesh. |
| `Colors` | **[SphericalHarmonicsL1\`1](https://wiki.resonite.com/Type:SphericalHarmonicsL1%601 "Type:SphericalHarmonicsL1`1") < [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") >** | The spherical harmonic colors to use. |
| `RadiusMultiplier` | **[SphericalHarmonicsL1\`1](https://wiki.resonite.com/Type:SphericalHarmonicsL1%601 "Type:SphericalHarmonicsL1`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | The spherical harmonics to use to influence the mesh radius at different spots. |
| `NegativeRadiusInvertsColor` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether negative colors invert the mesh geometry. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:IcoSphereMeshSH1&oldid=98454](https://wiki.resonite.com/index.php?title=Component:IcoSphereMeshSH1&oldid=98454)"

Contents