# Component:Texture3DAssetMetadata

> Source: https://wiki.resonite.com/Component:Texture3DAssetMetadata

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/5b/Texture3DAssetMetadataComponent.png/510px-Texture3DAssetMetadataComponent.png)](https://wiki.resonite.com/File:Texture3DAssetMetadataComponent.png) **Texture 3D Asset Metadata** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Texture3DAssetMetadata** component is able to retrieve the [3D texture](https://wiki.resonite.com/Texture3D "Texture3D") data like size, memory, and format usually seen at the bottom of an inspector on a particular component as usable values.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Texture` | **[Texture3D](https://wiki.resonite.com/Type:Texture3D "Type:Texture3D")** | The texture to get Asset Metadata for. |
| `Size` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int3](https://wiki.resonite.com/Type:Int3 "Type:Int3")** | The size of `Texture` in pixels. |
| `Width` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The width of `Texture` in pixels. |
| `Height` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The height of `Texture` in pixels. |
| `Depth` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The depth or Z of `Texture` in pixels. |
| `MemoryBytes` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Long](https://wiki.resonite.com/Type:Long "Type:Long")** | How many bytes of memory `Texture` takes up. |
| `FormattedMemoryBytes` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The bytes that `Texture` uses in easy to read human format. |
| `Format` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[TextureFormat](https://wiki.resonite.com/Type:TextureFormat "Type:TextureFormat")** | The format that `Texture` is kept in. |
| `ActualLoadedVariant` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The variant of `Texture` that has been loaded, which can be different on a client due to graphics settings or variants are being calculated on the cloud. |
| `Profile` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | The color space `Texture` is rendered in. |

Fields
Collapse

## Usage

Attach to a slot and provide a texture to `Texture` and the component will change it's Outputs to the data in that provided texture.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:Texture2DAssetMetadata](https://wiki.resonite.com/Component:Texture2DAssetMetadata "Component:Texture2DAssetMetadata")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:Texture3DAssetMetadata&oldid=113615](https://wiki.resonite.com/index.php?title=Component:Texture3DAssetMetadata&oldid=113615)"

Contents