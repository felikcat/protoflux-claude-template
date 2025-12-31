# Component:PointClusterMesh

> Source: https://wiki.resonite.com/Component:PointClusterMesh

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:PointClusterMesh&diff=112350) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/1b/PointClusterMeshComponent.png/510px-PointClusterMeshComponent.png)](https://wiki.resonite.com/File:PointClusterMeshComponent.png) **Point Cluster Mesh** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **PointClusterMesh** component generates a randomized cluster of points in a cloud. These points can be displayed via a [Mesh Renderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") using a [Unlit Material](https://wiki.resonite.com/Component:UnlitMaterial "Component:UnlitMaterial") with at least it's `UseBillboardGeometry` field set to true.

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
| `Distribution` | **[PointClusterMesh.DistributionType](https://wiki.resonite.com/Component:PointClusterMesh#DistributionType)** |  |
| `Colors` | **[PointClusterMesh.ColorMode](https://wiki.resonite.com/Component:PointClusterMesh#ColorMode)** |  |
| `TextureColorSource` | **[ITexture](https://wiki.resonite.com/Type:ITexture "Type:ITexture")** |  |
| `HeightScaleSource` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** |  |
| `TextureIntensityClip` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** |  |
| `TextureAlphaClip` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** |  |
| `MaxClipAttempts` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** |  |
| `HeightmapExp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** |  |
| `Seed` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The number to use to seed the generation of random points. |
| `Points` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The number of points to generate. |
| `Atlas` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [AtlasInfo](https://wiki.resonite.com/Component:AtlasInfo "Component:AtlasInfo") >** |  |
| `Scale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The scale of the generated mesh. |
| `RangeExp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** |  |
| `JitterRange` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The maximum value to randomly offset each point. |
| `Color0` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** |  |
| `Color1` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** |  |
| `ColorLerpScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** |  |
| `ColorGap` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** |  |
| `SimplexNoiseScale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** |  |
| `SimplexNoiseOffset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** |  |
| `UniformSize` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether all points should always be uniformly scaled. |
| `MinSize` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The minimum size of a point. |
| `MaxSize` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The maximum size of a point. |
| `MinRotation` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum rotation of a point. |
| `MaxRotation` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum rotation of a point. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Usage

This is used for the colored orbs in the sky of the [Resonite Cloud Home](https://wiki.resonite.com/Resonite_Cloud_Home "Resonite Cloud Home").

## Examples

## See Also

[Component:PointMesh](https://wiki.resonite.com/Component:PointMesh "Component:PointMesh")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PointClusterMesh&oldid=112350](https://wiki.resonite.com/index.php?title=Component:PointClusterMesh&oldid=112350)"

Contents