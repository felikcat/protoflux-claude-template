# Component:GaussianSplatAssetMetadata

> Source: https://wiki.resonite.com/Component:GaussianSplatAssetMetadata

Collapse **Component image**

[File:GaussianSplatAssetMetadataComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=GaussianSplatAssetMetadataComponent.png "File:GaussianSplatAssetMetadataComponent.png") **Gaussian Splat Asset Metadata** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **Gaussian Splat Asset Metadata** component gives statistics on [Gaussian Splats](https://wiki.resonite.com/Gaussian_Splat "Gaussian Splat") seen in inspectors for components that generate or provide such data.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Splat` | **[GaussianSplat](https://wiki.resonite.com/Type:GaussianSplat "Type:GaussianSplat")** | The splat to get data on. |
| `SplatCount` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The number of splats in the Gaussian splat. |
| `MemoryBytes` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Long](https://wiki.resonite.com/Type:Long "Type:Long")** | The amount of memory in bytes the Gaussian splat takes up. |
| `FormattedMemoryBytes` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The amount of memory in bytes the Gaussian splat takes up when formatted. |
| `ActualLoadedVariant` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The variant of the Gaussian splat that is loaded from the cloud. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GaussianSplatAssetMetadata&oldid=113574](https://wiki.resonite.com/index.php?title=Component:GaussianSplatAssetMetadata&oldid=113574)"

Contents