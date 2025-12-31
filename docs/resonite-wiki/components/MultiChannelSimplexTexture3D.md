# Component:MultiChannelSimplexTexture3D

> Source: https://wiki.resonite.com/Component:MultiChannelSimplexTexture3D

Collapse **Component image**

[File:MultiChannelSimplexTexture3DComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=MultiChannelSimplexTexture3DComponent.png "File:MultiChannelSimplexTexture3DComponent.png") **Multi Channel Simplex Texture 3D** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **MultiChannelSimplexTexture3D** component creates a monochrome noise channel for each RGBA channel with their own settings. It is also considered a ITexture3D element.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `FilterMode` | **[TextureFilterMode](https://wiki.resonite.com/Type:TextureFilterMode "Type:TextureFilterMode")** | How to interpolate enlarged pixels when rendering the texture. |
| `AnisotropicLevel` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Used when the texture is using the Anisotropic filtering render algorithm. |
| `WrapModeU` | **[TextureWrapMode](https://wiki.resonite.com/Type:TextureWrapMode "Type:TextureWrapMode")** | How to handle wrapping for UVW sampling positions beyond the 0 to 1 range for U. |
| `WrapModeV` | **[TextureWrapMode](https://wiki.resonite.com/Type:TextureWrapMode "Type:TextureWrapMode")** | How to handle wrapping for UVW sampling positions beyond the 0 to 1 range for V. |
| `WrapModeW` | **[TextureWrapMode](https://wiki.resonite.com/Type:TextureWrapMode "Type:TextureWrapMode")** | How to handle wrapping for UVW sampling positions beyond the 0 to 1 range for W. |
| `Profile` | **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | The color space to render the image in. |
| `Size` | **[Int3](https://wiki.resonite.com/Type:Int3 "Type:Int3")** | How big the texture is in pixels. |
| `Format` | **[TextureFormat](https://wiki.resonite.com/Type:TextureFormat "Type:TextureFormat")** | What format to show the texture in. |
| `R` | _direct_ **[MultiChannelSimplexTexture3D.ChannelConfiguration](https://wiki.resonite.com/Component:MultiChannelSimplexTexture3D#ChannelConfiguration)** | The settings to use when generating the noise for the red channel. |
| `G` | _direct_ **[MultiChannelSimplexTexture3D.ChannelConfiguration](https://wiki.resonite.com/Component:MultiChannelSimplexTexture3D#ChannelConfiguration)** | The settings to use when generating the noise for the green channel. |
| `B` | _direct_ **[MultiChannelSimplexTexture3D.ChannelConfiguration](https://wiki.resonite.com/Component:MultiChannelSimplexTexture3D#ChannelConfiguration)** | The settings to use when generating the noise for the blue channel. |
| `A` | _direct_ **[MultiChannelSimplexTexture3D.ChannelConfiguration](https://wiki.resonite.com/Component:MultiChannelSimplexTexture3D#ChannelConfiguration)** | The settings to use when generating the noise for the alpha channel. |

Fields
Collapse

## ChannelConfiguration

| Name | Type | Description |
| --- | --- | --- |
| `Offset` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to shift the noise. |
| `Scale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | How much to scale up the noise to make it more gentle, or down to make it more noisy. |
| `Use4D` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use the 4D sample Map or a 1D sample map. |
| `WOffset` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to offset on the W axis to change the seed. |
| `Min` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The smallest value that can be sampled for this channel. |
| `Max` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The biggest value that can be sampled for this channel. |
| `Exp` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast/slow to make output values approach 1 as you get to 100% noise value sampled. (Sharpness) |

Fields

## Usage

Can be used to make procedural noise 4D textures for use with LUT, and volume.

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MultiChannelSimplexTexture3D&oldid=105337](https://wiki.resonite.com/index.php?title=Component:MultiChannelSimplexTexture3D&oldid=105337)"

Contents