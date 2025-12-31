# Component:VideoTextureAssetMetadata

> Source: https://wiki.resonite.com/Component:VideoTextureAssetMetadata

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:VideoTextureAssetMetadata&diff=95844) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/19/VideoTextureAssetMetadataComponent.png/510px-VideoTextureAssetMetadataComponent.png)](https://wiki.resonite.com/File:VideoTextureAssetMetadataComponent.png) **Video Texture Asset Metadata** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **VideoTextureAssetMetadata** component turns the data at the bottom of an inspector on a video asset Type component into usable values which can be used elsewhere.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Texture` | **[VideoTexture](https://wiki.resonite.com/Type:VideoTexture "Type:VideoTexture")** | The video texture to get information on. |
| `Size` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int2](https://wiki.resonite.com/Type:Int2 "Type:Int2")** | The size of the `Texture` in pixels. |
| `Width` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The width of `Texture` in pixels. |
| `Height` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The height of `Texture` in pixels. |
| `HasAlpha` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether `Texture` is transparent. |
| `Length` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The duration of `Texture`. |
| `PlaybackEngine` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The playback engine `Texture` is using. |

Fields
Collapse

## Usage

Attach to a slot and provide a `Texture` to get information on in order for it to work.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:VideoTextureProvider](https://wiki.resonite.com/Component:VideoTextureProvider "Component:VideoTextureProvider")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VideoTextureAssetMetadata&oldid=95844](https://wiki.resonite.com/index.php?title=Component:VideoTextureAssetMetadata&oldid=95844)"

Contents