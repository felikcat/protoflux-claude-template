# Component:BoxVertexValueSpatialVariable

> Source: https://wiki.resonite.com/Component:BoxVertexValueSpatialVariable

Collapse **Component image**

[File:BoxVertexValueSpatialVariable\`1Component.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=BoxVertexValueSpatialVariable%601Component.png "File:BoxVertexValueSpatialVariable`1Component.png") **Box Vertex Value Spatial Variable\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Box Vertex Value Spatial Variable\`1** component makes a spatial variable that provides samplers with a different value depending on what vertex of the area a sampler is closest to. This is similar to the color properties of a [box emitter](https://wiki.resonite.com/Component:BoxEmitter "Component:BoxEmitter").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `VariableName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the variable this has within it's field of influence for the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. |
| `Priority` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The priority this spatial variable has other others overlapping in the same space for the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. |
| `Size` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The size of the cube for this spatial variable's influence. |
| `BlendDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How the gradient for this variable within it's volume determines the sampled value for the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. |
| `BlendDistanceMode` | **[SpatialVariableBlendDistanceMode](https://wiki.resonite.com/Type:SpatialVariableBlendDistanceMode "Type:SpatialVariableBlendDistanceMode")** | The mode used for blending the value with other variables for the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. |
| `Value0` | **T** | The value sampled when near the 0th vertex. |
| `Value1` | **T** | The value sampled when near the 1st vertex. |
| `Value2` | **T** | The value sampled when near the 2nd vertex. |
| `Value3` | **T** | The value sampled when near the 3rd vertex. |
| `Value4` | **T** | The value sampled when near the 4th vertex. |
| `Value5` | **T** | The value sampled when near the 5th vertex. |
| `Value6` | **T** | The value sampled when near the 6th vertex. |
| `Value7` | **T** | The value sampled when near the 7th vertex. |

Fields
Collapse

## Usage

Attach to a slot and provide a size and variable name in order for this to function.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BoxVertexValueSpatialVariable&oldid=101134](https://wiki.resonite.com/index.php?title=Component:BoxVertexValueSpatialVariable&oldid=101134)"

Contents