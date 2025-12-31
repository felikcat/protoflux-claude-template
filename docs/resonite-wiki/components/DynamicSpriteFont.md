# Component:DynamicSpriteFont

> Source: https://wiki.resonite.com/Component:DynamicSpriteFont

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:DynamicSpriteFont&diff=97478) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/83/DynamicSpriteFontComponent.png/510px-DynamicSpriteFontComponent.png)](https://wiki.resonite.com/File:DynamicSpriteFontComponent.png) **Dynamic Sprite Font** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DynamicSpriteFont** component is used to construct a font asset that can be used to create custom fonts character by character.

![](https://wiki.resonite.com/images/b/b7/DangerIcon.svg)

This component can cause memory leaks! See [Issue #2771](https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/2771)

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `HighPriorityIntegration` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If true, integrating this asset (e.g. processing procedural assets) gets higher priority than assets with this flag off. An example is user laser procedural meshes. |
| `MaxSize` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The max size of a glyph in the font sheet. |
| `Glyphs` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[DynamicSpriteFont.SpriteGlyph](https://wiki.resonite.com/Component:DynamicSpriteFont#SpriteGlyph)** | A list of Font characters that should make up this dynamic font. |

Fields
Collapse

## Glyph Example

[![](https://wiki.resonite.com/images/thumb/f/f1/Freetype2_docs_glyphs_glyph-metrics-3.png/510px-Freetype2_docs_glyphs_glyph-metrics-3.png)](https://wiki.resonite.com/File:Freetype2_docs_glyphs_glyph-metrics-3.png)

## SpriteGlyph

| Name | Type | Description |
| --- | --- | --- |
| `SpriteURL` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The resource URI of the Font character. |
| `UnicodeCodepoint` | **[UInt](https://wiki.resonite.com/Type:UInt "Type:UInt")** | the Unicode number of this Font character. See [Wikipedia list of unicode characters](https://en.m.wikipedia.org/wiki/List_of_Unicode_characters). |
| `SpriteName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the Sprite. |
| `Bearing` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | See [Glyph Example](https://wiki.resonite.com/Component:DynamicSpriteFont#Glyph_Example). |
| `Advance` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | See [Glyph Example](https://wiki.resonite.com/Component:DynamicSpriteFont#Glyph_Example). |
| `Size` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | See [Glyph Example](https://wiki.resonite.com/Component:DynamicSpriteFont#Glyph_Example). |
| `Tintable` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this glyph is affectable by Font color. |

Fields

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DynamicSpriteFont&oldid=97478](https://wiki.resonite.com/index.php?title=Component:DynamicSpriteFont&oldid=97478)"

Contents