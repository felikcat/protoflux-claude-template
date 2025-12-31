# Component:ITexture2DAssetMetadata

> Source: https://wiki.resonite.com/Component:ITexture2DAssetMetadata

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ITexture2DAssetMetadata&diff=91537) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/2c/ITexture2DAssetMetadataComponent.png/510px-ITexture2DAssetMetadataComponent.png)](https://wiki.resonite.com/File:ITexture2DAssetMetadataComponent.png) **ITexture 2D Asset Metadata** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

This component gives the info on the size of a Texture2D.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Texture` | **[ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D")** | The texture to read data for |
| `Size` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2")** | The size of `Texture` |
| `Width` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | width of `Texture` |
| `Height` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | height of `Texture` |

Fields
Collapse

## Usage

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ITexture2DAssetMetadata&oldid=91537](https://wiki.resonite.com/index.php?title=Component:ITexture2DAssetMetadata&oldid=91537)"

Contents