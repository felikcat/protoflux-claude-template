# Component:BoxConstantValueSpatialVariable

> Source: https://wiki.resonite.com/Component:BoxConstantValueSpatialVariable

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/49/BoxConstantValueSpatialVariable%601Component.png/510px-BoxConstantValueSpatialVariable%601Component.png)](https://wiki.resonite.com/File:BoxConstantValueSpatialVariable%601Component.png) **Box Constant Value Spatial Variable\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Box Constant Value Spatial Variable\`1** component is a [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") variable where the value is the same throughout the whole volume.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `VariableName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the variable this has within it's field of influence for the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. |
| `Priority` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The priority this spatial variable has other others overlapping in the same space for the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. |
| `Size` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The size of the cube area to allow sampling within. |
| `BlendDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How the gradient for this variable within it's volume determines the sampled value for the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. |
| `BlendDistanceMode` | **[SpatialVariableBlendDistanceMode](https://wiki.resonite.com/Type:SpatialVariableBlendDistanceMode "Type:SpatialVariableBlendDistanceMode")** | The mode used for blending the value with other variables for the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. |
| `Value` | **T** | The value this spatial variable gives when sampled at 100%. |

Fields
Collapse

## Usage

Attach to a slot and provide a size and variable name in order for this to function.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BoxConstantValueSpatialVariable&oldid=101112](https://wiki.resonite.com/index.php?title=Component:BoxConstantValueSpatialVariable&oldid=101112)"

Contents