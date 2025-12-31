# Component:FontCollection

> Source: https://wiki.resonite.com/Component:FontCollection

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/ce/FontCollectionComponent.png/510px-FontCollectionComponent.png)](https://wiki.resonite.com/File:FontCollectionComponent.png) **Font Collection** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **FontCollection** component acts as a set of fonts that can be used to make one mega font. When a font in the set does not have a character for a unicode point, another font can take over.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `FontSets` | _[list](https://wiki.resonite.com/Type:SyncAssetList%601 "Type:SyncAssetList`1")_ of **[FontSet](https://wiki.resonite.com/Type:FontSet "Type:FontSet")** | The list of fonts to congregate into one huge font. |

Fields
Collapse

## Usage

Used to combine fonts

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FontCollection&oldid=94753](https://wiki.resonite.com/index.php?title=Component:FontCollection&oldid=94753)"

Contents