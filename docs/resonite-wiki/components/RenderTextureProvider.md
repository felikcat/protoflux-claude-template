# Component:RenderTextureProvider

> Source: https://wiki.resonite.com/Component:RenderTextureProvider

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/eb/RenderTextureProviderComponent.png/510px-RenderTextureProviderComponent.png)](https://wiki.resonite.com/File:RenderTextureProviderComponent.png) **Render Texture Provider** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **RenderTextureProvider** component is used as a target for rendering [Component:Camera](https://wiki.resonite.com/Component:Camera "Component:Camera") or [Component:CameraPortal](https://wiki.resonite.com/Component:CameraPortal "Component:CameraPortal") data onto. This component can be used as a texture for any material.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Size` | **[Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2")** | The size the camera renders in `width` and `height` |
| `Depth` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Precision, in bits, of the depth buffer used for rendering. Possibly values are 0, 16, 24 and 32. |
| `FilterMode` | **[TextureFilterMode](https://wiki.resonite.com/Type:TextureFilterMode "Type:TextureFilterMode")** | How to handle the interpolation between pixels. |
| `AnisotropicLevel` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The levels of Anisotropic filtering distances when using Anisotropic for `FilterMode` |
| `WrapModeU` | **[TextureWrapMode](https://wiki.resonite.com/Type:TextureWrapMode "Type:TextureWrapMode")** | How to repeat or mirror the texture along the X axis. this goes into affect when X values are outside of the range \[0.0 to 1.0\]. |
| `WrapModeV` | **[TextureWrapMode](https://wiki.resonite.com/Type:TextureWrapMode "Type:TextureWrapMode")** | How to repeat or mirror the texture along the Y axis. this goes into affect when Y values are outside of the range \[0.0 to 1.0\]. |

Fields
Collapse

## Usage

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

**RenderTextureProvider** will not wrap with a Depth value above 0, be sure to set it to 0 if you want to create repeating patterns! see: [This comment on issue #1265 for clarification.](https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/1265#issuecomment-3125085062)

Attach to a slot and use as a render texture for any component that accepts it. The texture color data will now exist. Insert into any [material](https://wiki.resonite.com/Material "Material") to view.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See also

- [Component:Camera](https://wiki.resonite.com/Component:Camera "Component:Camera")
- [Component:CameraPortal](https://wiki.resonite.com/Component:CameraPortal "Component:CameraPortal")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RenderTextureProvider&oldid=108571](https://wiki.resonite.com/index.php?title=Component:RenderTextureProvider&oldid=108571)"

Contents