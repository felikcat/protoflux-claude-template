# Component:ImageColorDistributionGraph

> Source: https://wiki.resonite.com/Component:ImageColorDistributionGraph

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ImageColorDistributionGraph&diff=97958) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/fc/ImageColorDistributionGraphComponent.png/510px-ImageColorDistributionGraphComponent.png)](https://wiki.resonite.com/File:ImageColorDistributionGraphComponent.png) **Image Color Distribution Graph** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ImageColorDistributionGraph** component is used to make mesh data for a set of points with colors and sizes based on a provided image's pixels. The mesh needs to be used with Billboard geometry to be viewed properly.

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
| `Texture` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** | The texture to analyze and use to generate the vertex graph for this mesh. |
| `ColorSpace` | **[ImageColorDistributionGraph.Space](https://wiki.resonite.com/Component:ImageColorDistributionGraph#Space)** | The color space to use for X, Y, and Z coordinates on the graph for. |
| `MaxTextureSize` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The max size of the image on one axis that this image will use when making the graph. The image gets resized internally to fit this size. |
| `BaseSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The size of any color point on the graph at minimum. |
| `AccumulateSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to add to the size of a graph point if a color is repeated with the same RGB values. |
| `MaxSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum size a color point on the graph can be. |
| `Scale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to scale the graph up or down. |
| `AlphaThreshold` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | if alpha is below this threshold, then don't add the color to the graph. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeMesh:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Bake meshes is a sync method that creates a static mesh component with this component, replaces all references to this component with the static mesh component, then deletes this component. |

Triggers
Collapse

## Space

| Name | Value | Description |
| --- | --- | --- |
| `RGB` | 0 | Convert colors in the image into RGB (Red Green Blue) values and use them as the graphs's XYZ values. |
| `HSV` | 1 | Convert colors in the image into HSV (Hue Saturation Value) values and use them as the graph's XYZ valuee. |

Values

## Usage

Attach this component to a slot, and place it into a [Mesh Renderer Component](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") with an [Unlit Material](https://wiki.resonite.com/Component:UnlitMaterial "Component:UnlitMaterial") set to use billboard geometry to view the mesh and its graph points.

## Examples

- [![An example of this component in use with an Unlit Material set to billboard geometry.](https://wiki.resonite.com/images/thumb/b/ba/ImageColorDistributionGraph_Example.png/199px-ImageColorDistributionGraph_Example.png)](https://wiki.resonite.com/File:ImageColorDistributionGraph_Example.png "An example of this component in use with an Unlit Material set to billboard geometry.")

An example of this component in use with an [Unlit Material](https://wiki.resonite.com/Component:UnlitMaterial "Component:UnlitMaterial") set to billboard geometry.


## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ImageColorDistributionGraph&oldid=97958](https://wiki.resonite.com/index.php?title=Component:ImageColorDistributionGraph&oldid=97958)"

Contents