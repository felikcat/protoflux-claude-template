# Component:SphereStartEndValueSpatialVariable

> Source: https://wiki.resonite.com/Component:SphereStartEndValueSpatialVariable

Collapse **Component image**

[File:SphereStartEndValueSpatialVariable\`1Component.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=SphereStartEndValueSpatialVariable%601Component.png "File:SphereStartEndValueSpatialVariable`1Component.png") **Sphere Start End Value Spatial Variable\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Sphere Start End Value Spatial Variable\`1** component is part of the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. The start value starts at the edge of the shape and goes inwards towards the center, or the other way around depending on provided values.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `VariableName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the variable this has within it's field of influence for the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. |
| `Priority` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The priority this spatial variable has other others overlapping in the same space for the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. |
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The priority this spatial variable has other others overlapping in the same space for the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. |
| `BlendDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How the gradient for this variable within it's volume determines the sampled value for the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. |
| `BlendDistanceMode` | **[SpatialVariableBlendDistanceMode](https://wiki.resonite.com/Type:SpatialVariableBlendDistanceMode "Type:SpatialVariableBlendDistanceMode")** | The mode used for blending the value with other variables for the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. |
| `StartValue` | **T** | The value this spatial variable gives when sampled at 0%. |
| `EndValue` | **T** | The value this spatial variable gives when sampled at 100%. |
| `StartDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance at which the sampled spatial variable starts at `StartValue`. |
| `EndDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The distance at which the sampled spatial variable ends at `EndValue`. |
| `Mode` | **[SpatialVariableDistanceMode](https://wiki.resonite.com/index.php?title=Type:SpatialVariableDistanceMode&action=edit&redlink=1 "Type:SpatialVariableDistanceMode (page does not exist)")** | The mode to use when sampling the values based on distance. |

Fields
Collapse

## Usage

Attach to a slot and provide a size and variable name in order for this to function.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SphereStartEndValueSpatialVariable&oldid=106580](https://wiki.resonite.com/index.php?title=Component:SphereStartEndValueSpatialVariable&oldid=106580)"

Contents