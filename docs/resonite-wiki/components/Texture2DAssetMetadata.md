# Component:Texture2DAssetMetadata

> Source: https://wiki.resonite.com/Component:Texture2DAssetMetadata

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:Texture2DAssetMetadata&diff=95725) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/51/Texture2DAssetMetadataComponent.png/510px-Texture2DAssetMetadataComponent.png)](https://wiki.resonite.com/File:Texture2DAssetMetadataComponent.png) **Texture 2D Asset Metadata** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Texture2DAssetMetadata** component converts the metadata often seen on texture components in an inspector into data that can be pulled into other systems as actual numbers and values.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Texture` | **[Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D")** | The texture to get metadata on. |
| `Size` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2")** | How big `Texture` is in pixels as a width height pair. |
| `Width` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How wide `Texture` is in pixels. |
| `Height` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How tall `Texture` is in pixels. |
| `HasMipMaps` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether `Texture` has mipmaps. |
| `MipMapCount` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many mipmap levels `Texture` has. |
| `MemoryBytes` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Long](https://wiki.resonite.com/Type:Long "Type:Long")** | How many bytes of memory `Texture` takes up. |
| `FormattedMemoryBytes` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The bytes of memory `Texture` takes up formatted into an easy to read format. |
| `Format` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[TextureFormat](https://wiki.resonite.com/Type:TextureFormat "Type:TextureFormat")** | The format `Texture` is encoded in. |
| `ActualLoadedVariant` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The actual variant of `Texture` that is loaded on the client. |
| `Profile` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | The color profile `Texture` is being rendered in. |

Fields
Collapse

## Usage

Attach to a slot and provide an asset to `Texture` to start getting values and using the component.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:Texture3DAssetMetadata](https://wiki.resonite.com/Component:Texture3DAssetMetadata "Component:Texture3DAssetMetadata")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Texture2DAssetMetadata&oldid=95725](https://wiki.resonite.com/index.php?title=Component:Texture2DAssetMetadata&oldid=95725)"

Contents