# Component:BoxTexture3D SpatialVariable

> Source: https://wiki.resonite.com/Component:BoxTexture3D_SpatialVariable

Collapse **Component image**

[File:BoxTexture3D SpatialVariableComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=BoxTexture3D_SpatialVariableComponent.png "File:BoxTexture3D SpatialVariableComponent.png") **Box Texture 3D Spatial Variable** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Box Texture 3D Spatial Variable** component is specifically for colorX spatial variables. This is a box spatial variable that provides colorX [spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") sampled from a [Texture3D](https://wiki.resonite.com/Texture3D "Texture3D").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `VariableName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the variable this has within it's field of influence for the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. |
| `Priority` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The priority this spatial variable has other others overlapping in the same space for the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. |
| `Size` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | the size of the box in which variable samplers can sample from this within. |
| `BlendDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How the gradient for this variable within it's volume determines the sampled value for the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. |
| `BlendDistanceMode` | **[SpatialVariableBlendDistanceMode](https://wiki.resonite.com/Type:SpatialVariableBlendDistanceMode "Type:SpatialVariableBlendDistanceMode")** | The mode used for blending the value with other variables for the [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables") system. |
| `Texture` | **[Texture3D](https://wiki.resonite.com/Type:Texture3D "Type:Texture3D")** | The texture to use and sample from in 3D space. Must have `IsReadable` enabled! |
| `UseNormalizedCoordinates` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | When enabled, this will squish/stretch the texture with the box. |
| `Scale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The scale of the texture in 3D space. |
| `Offset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The offset of the texture in 3D space from the slot this component is on. |
| `WrapU` | **[WrapMode](https://wiki.resonite.com/Type:WrapMode "Type:WrapMode")** | How to wrap the texture along the X axis. |
| `WrapV` | **[WrapMode](https://wiki.resonite.com/Type:WrapMode "Type:WrapMode")** | How to wrap the texture along the Y axis. |
| `WrapW` | **[WrapMode](https://wiki.resonite.com/Type:WrapMode "Type:WrapMode")** | How to wrap the texture along the Z axis. |

Fields
Collapse

## Usage

Attach to a slot and provide a size, 3d texture, and a variable name in order for this to function.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Spatial variables](https://wiki.resonite.com/Spatial_variables "Spatial variables")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BoxTexture3D\_SpatialVariable&oldid=113622](https://wiki.resonite.com/index.php?title=Component:BoxTexture3D_SpatialVariable&oldid=113622)"

Contents