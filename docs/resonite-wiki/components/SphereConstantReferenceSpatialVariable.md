# Component:SphereConstantReferenceSpatialVariable

> Source: https://wiki.resonite.com/Component:SphereConstantReferenceSpatialVariable

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/4/4c/SphereConstantReferenceSpatialVariable%601Component.png/510px-SphereConstantReferenceSpatialVariable%601Component.png)](https://wiki.resonite.com/File:SphereConstantReferenceSpatialVariable%601Component.png) **Sphere Constant Reference Spatial Variable\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **SphereConstantReferenceSpatialVariable** component is used to define a reference value as part of the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system without a gradient.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `VariableName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the variable this has within it's field of influence for the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. |
| `Priority` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The priority this spatial variable has other others overlapping in the same space for the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. |
| `Radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How big the sphere is for the area of influence. |
| `BlendDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How the gradient for this variable within it's volume determines the sampled value for the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. |
| `BlendDistanceMode` | **[SpatialVariableBlendDistanceMode](https://wiki.resonite.com/Type:SpatialVariableBlendDistanceMode "Type:SpatialVariableBlendDistanceMode")** | The mode used for blending the value with other variables for the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. |
| `Reference` | **T** | The value this spatial variable gives when sampled at 100%. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:SphereConstantReferenceSpatialVariable&oldid=106575](https://wiki.resonite.com/index.php?title=Component:SphereConstantReferenceSpatialVariable&oldid=106575)"

Contents