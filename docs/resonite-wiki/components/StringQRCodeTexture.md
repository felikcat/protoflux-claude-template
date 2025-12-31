# Component:StringQRCodeTexture

> Source: https://wiki.resonite.com/Component:StringQRCodeTexture

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:StringQRCodeTexture&diff=98083) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a3/StringQRCodeTextureComponent.png/510px-StringQRCodeTextureComponent.png)](https://wiki.resonite.com/File:StringQRCodeTextureComponent.png) **String QRCode Texture** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **StringQRCodeTexture** Component is used to encode string data like URLs and text into a QR code texture.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `FilterMode` | **[TextureFilterMode](https://wiki.resonite.com/Type:TextureFilterMode "Type:TextureFilterMode")** | How to handle the interpolation between pixels. |
| `AnisotropicLevel` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The levels of Anisotropic filtering distances when using Anisotropic for `FilterMode` |
| `WrapModeU` | **[TextureWrapMode](https://wiki.resonite.com/Type:TextureWrapMode "Type:TextureWrapMode")** | How to repeat or mirror the texture along the X axis. this goes into affect when X values are outside of the range \[0.0 to 1.0\]. |
| `WrapModeV` | **[TextureWrapMode](https://wiki.resonite.com/Type:TextureWrapMode "Type:TextureWrapMode")** | How to repeat or mirror the texture along the Y axis. this goes into affect when Y values are outside of the range \[0.0 to 1.0\]. |
| `MipmapBias` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Whether to see lower resolution versions of the texture closer up or not (MipMaps). |
| `Profile` | **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | The color profile to use for this texture's rendering. |
| `Format` | **[TextureFormat](https://wiki.resonite.com/Type:TextureFormat "Type:TextureFormat")** | TextureFormat describes how Texture's pixel are stored in the VRAM. |
| `Payload` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The string to encode into the QR code. |
| `ECCLevel` | **[ECCLevel](https://wiki.resonite.com/Type:ECCLevel "Type:ECCLevel")** | The level of error correction to encode (for use with a dirty QR code for higher values) |
| `Color0` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The background color of the QR code |
| `Color1` | **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The color of the usually black squares of the QRCode |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeTexture:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | BakeTexture first generates a [Component:StaticTexture2D](https://wiki.resonite.com/Component:StaticTexture2D "Component:StaticTexture2D") that is the same as this procedural texture. The resulting static texture replaces every reference to the original procedural texture. Lastly the original procedural texture is deleted. |

Triggers
Collapse

## Usage

Attach to a slot and insert into a [material](https://wiki.resonite.com/Material "Material") to view the result. Don't forget to provide a `Payload`.

## Examples

QR code generated from an URL:

[![On the right, the QR code generator component with on the left its generated texture showing a QR code.](https://wiki.resonite.com/images/thumb/4/46/QRCodeExampleUrl.png/500px-QRCodeExampleUrl.png)](https://wiki.resonite.com/File:QRCodeExampleUrl.png)

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:StringQRCodeTexture&oldid=98083](https://wiki.resonite.com/index.php?title=Component:StringQRCodeTexture&oldid=98083)"

Contents