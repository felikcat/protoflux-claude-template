# Component:MaterialAssetMetadata

> Source: https://wiki.resonite.com/Component:MaterialAssetMetadata

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:MaterialAssetMetadata&diff=94894) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/b/b9/MaterialAssetMetadataComponent.png/510px-MaterialAssetMetadataComponent.png)](https://wiki.resonite.com/File:MaterialAssetMetadataComponent.png) **Material Asset Metadata** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **MaterialAssetMetadata** component gives variant info about materials in the form of usable values. These values are usually listed at the bottom of a material inspector but are unusable in that state.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Material` | **[Material](https://wiki.resonite.com/Type:Material "Type:Material")** | The material to get Metadata on. |
| `VariantIndex` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [UInt32](https://wiki.resonite.com/Type:UInt32 "Type:UInt32") >** | The material variant defined by GPU definitions on the shader. For example, a reflection material has a second variant for having a normal map vs without. |
| `RawVariantIndex` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [UInt32](https://wiki.resonite.com/Type:UInt32 "Type:UInt32") >** | The raw version of `VariantIndex`. |
| `VariantID` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The ID of the material variant (can be seen at the bottom of a material in the Inspector too. |
| `RawVariantID` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The raw version of `VariantID`. |
| `WaitingForApply` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this material is waiting to be applied in the render scene due to missing variants or otherwise. |

Fields
Collapse

## Usage

Can be used to get variant info and other info shown at the bottom of a material in the Inspector as actual usable values.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:MaterialAssetMetadata&oldid=94894](https://wiki.resonite.com/index.php?title=Component:MaterialAssetMetadata&oldid=94894)"

Contents