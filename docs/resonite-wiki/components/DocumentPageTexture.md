# Component:DocumentPageTexture

> Source: https://wiki.resonite.com/Component:DocumentPageTexture

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:DocumentPageTexture&diff=97924) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/70/DocumentPageTextureComponent.png/510px-DocumentPageTextureComponent.png)](https://wiki.resonite.com/File:DocumentPageTextureComponent.png) **Document Page Texture** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DocumentPageTexture** component generates texture data using a document file like a PDF which can be displayed using a [material](https://wiki.resonite.com/Material "Material") in a [Component:MeshRenderer](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer") or [UIX](https://wiki.resonite.com/UIX "UIX").

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
| `Size` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The size of the procedural texture in pixels. |
| `Mipmaps` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use mip maps or not. |
| `Document` | **[Document](https://wiki.resonite.com/index.php?title=Type:Document&action=edit&redlink=1 "Type:Document (page does not exist)")** | The document to display using this texture. |
| `PageIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The page in `Document` to display as the texture data. |
| `PageRegion` | **[Rect](https://wiki.resonite.com/Type:Rect "Type:Rect")** | The area of the in `Document` to display on page `PageIndex` |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `BakeTexture:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | BakeTexture first generates a [Component:StaticTexture2D](https://wiki.resonite.com/Component:StaticTexture2D "Component:StaticTexture2D") that is the same as this procedural texture. The resulting static texture replaces every reference to the original procedural texture. Lastly the original procedural texture is deleted. |

Triggers
Collapse

## Usage

This component is auto generated as part of a document viewer when importing PDF files. Simply import a PDF file into the game to generate a viewer that uses this component as part of how it works.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Type:Document](https://wiki.resonite.com/index.php?title=Type:Document&action=edit&redlink=1 "Type:Document (page does not exist)")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DocumentPageTexture&oldid=97924](https://wiki.resonite.com/index.php?title=Component:DocumentPageTexture&oldid=97924)"

Contents