# Component:BoxConstantReferenceSpatialVariable

> Source: https://wiki.resonite.com/Component:BoxConstantReferenceSpatialVariable

Collapse **Component image**

[File:BoxConstantReferenceSpatialVariable\`1Component.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=BoxConstantReferenceSpatialVariable%601Component.png "File:BoxConstantReferenceSpatialVariable`1Component.png") **Box Constant Reference Spatial Variable\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Box Constant Reference Spatial Variable\`1** component provides a constant value regardless of position inside of it as a contribution to a [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `VariableName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the variable this has within it's field of influence for the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. |
| `Priority` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The priority this spatial variable has other others overlapping in the same space for the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. |
| `Size` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How big the box is for the area of influence. |
| `BlendDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How the gradient for this variable within it's volume determines the sampled value for the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. |
| `BlendDistanceMode` | **[SpatialVariableBlendDistanceMode](https://wiki.resonite.com/Type:SpatialVariableBlendDistanceMode "Type:SpatialVariableBlendDistanceMode")** | The mode used for blending the value with other variables for the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. |
| `Reference` | **T** | The value this spatial variable gives when sampled at 100%. |

Fields
Collapse

## Usage

Attach to a slot and provide a size and variable name in order for this to function.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BoxConstantReferenceSpatialVariable&oldid=106574](https://wiki.resonite.com/index.php?title=Component:BoxConstantReferenceSpatialVariable&oldid=106574)"

Contents