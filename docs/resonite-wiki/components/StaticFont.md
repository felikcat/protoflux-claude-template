# Component:StaticFont

> Source: https://wiki.resonite.com/Component:StaticFont

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:StaticFont&diff=96655) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/14/StaticFontComponent.png/510px-StaticFontComponent.png)](https://wiki.resonite.com/File:StaticFontComponent.png) **Static Font** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

![](https://wiki.resonite.com/images/b/b7/DangerIcon.svg)

Adjusting some properties on this component can cause memory leaks! See [Issue #88](https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/88)

The **StaticFont** component is used to store data on a font set like Avali Scratch, Times New Roman, Hieroglyphs, Arial, and Monospaced fonts (monospaced fonts help people with dyslexia).

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `URL` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The location of where to load the font from. |
| `Padding` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many pixels of padding should be used between letters in the font. |
| `PixelRange` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Sets the distance field range in output pixels. |
| `GlyphEmSize` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Sets the size of the glyphs in the atlas in pixels per em. |
| `MipMaps` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to display lower res versions of the font when it is further away to save on performance. |
| `MipMapFiltering` | **[Filtering](https://wiki.resonite.com/Type:Filtering "Type:Filtering")** | How to filter transitions between mipmaps when it is viewed at incremental distances further away. |
| `LODBias` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Whether to see lower res versions at smaller distances to save performance. |

Fields
Collapse

## Usage

This component is auto generated when importing new font files. Simply find a font file (.TTF or similar) and drop it into the Resonite game window or import through the file browser in the dash. The game will then generate this component on a font object, with the `URL` field filled with a valid font resource.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- [Component:FontChain](https://wiki.resonite.com/Component:FontChain "Component:FontChain") for filling missing glyphs.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:StaticFont&oldid=96655](https://wiki.resonite.com/index.php?title=Component:StaticFont&oldid=96655)"

Contents