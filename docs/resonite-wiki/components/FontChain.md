# Component:FontChain

> Source: https://wiki.resonite.com/Component:FontChain

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/f/fd/FontChainComponent.png/510px-FontChainComponent.png)](https://wiki.resonite.com/File:FontChainComponent.png) **Font Chain** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **FontChain** component provides an easy way to use "Fallback" fonts for a main font, usually in the event that the main font does not contain certain Unicode characters. Any place where a [StaticFont](https://wiki.resonite.com/Component:StaticFont "Component:StaticFont") can be used, a FontChain can be used.

The `MainFont` defines which font will be primarily used for the text. For any characters of a text that do not exist in the main font, all the `FallbackFonts` will be searched through, in order, to find a matching character. Only if all fallback fonts do not contain the character will a "true fallback" of a box will appear.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `MainFont` | **[Font](https://wiki.resonite.com/index.php?title=Type:Font&action=edit&redlink=1 "Type:Font (page does not exist)")** | The main font to use. |
| `FallbackFonts` | _[list](https://wiki.resonite.com/Type:SyncAssetList%601 "Type:SyncAssetList`1")_ of **[Font](https://wiki.resonite.com/index.php?title=Type:Font&action=edit&redlink=1 "Type:Font (page does not exist)")** | The fallback fonts to use. |

Fields
Collapse

## Usage

Useful for example for Avali-Scratch, where numbers don't have a character. or for fonts where characters don't exist.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:StaticFont](https://wiki.resonite.com/Component:StaticFont "Component:StaticFont")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FontChain&oldid=93742](https://wiki.resonite.com/index.php?title=Component:FontChain&oldid=93742)"

Contents