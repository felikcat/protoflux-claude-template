# Component:CubemapAssetMetadata

> Source: https://wiki.resonite.com/Component:CubemapAssetMetadata

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:CubemapAssetMetadata&diff=94135) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/bc/CubemapAssetMetadataComponent.png/510px-CubemapAssetMetadataComponent.png)](https://wiki.resonite.com/File:CubemapAssetMetadataComponent.png) **Cubemap Asset Metadata** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **CubemapAssetMetadata** component is used to display info about any particular cube map provided.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Cubemap` | **[Cubemap](https://wiki.resonite.com/Type:Cubemap "Type:Cubemap")** | The cubemap to analyse. |
| `Size` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The size in pixels of the width or height of any 1 of the 6 sides. (The sides are the same size) |
| `HasMipMaps` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the cubemap has mipmap data. |
| `MipMapCount` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many mip map resolution variants the cubemap has. |
| `MemoryBytes` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Long](https://wiki.resonite.com/Type:Long "Type:Long")** | How much memory the cubemap takes up. |
| `FormattedMemoryBytes` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The bytes formatted into a readable string. |
| `Format` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[TextureFormat](https://wiki.resonite.com/Type:TextureFormat "Type:TextureFormat")** | The texture format of the cube map. |
| `ActualLoadedVariant` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The Asset variant Type currently loaded. |
| `Profile` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")** | The color profile being used for this texture when rendering it. |

Fields
Collapse

## Usage

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CubemapAssetMetadata&oldid=94135](https://wiki.resonite.com/index.php?title=Component:CubemapAssetMetadata&oldid=94135)"

Contents