# Component:PlatformColorPalette

> Source: https://wiki.resonite.com/Component:PlatformColorPalette

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/65/PlatformColorPaletteComponent.png/510px-PlatformColorPaletteComponent.png)](https://wiki.resonite.com/File:PlatformColorPaletteComponent.png) **Platform Color Palette** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **PlatformColorPalette** component is a quick way of getting the colors of [Resonite's](https://wiki.resonite.com/Resonite "Resonite") [Branding](https://wiki.resonite.com/Branding "Branding"). This also provides you with both the color values in [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") form and [Hex](https://en.wikipedia.org/wiki/Web_colors) form.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Neutrals` | _direct_ **[PlatformColorPalette.Grayscale](https://wiki.resonite.com/Component:PlatformColorPalette#Grayscale)** | A list of neutral color and hexes used for UI backgrounds in resonite. |
| `Hero` | _direct_ **[PlatformColorPalette.Colors](https://wiki.resonite.com/Component:PlatformColorPalette#Colors)** | A list of color and hexes used for bright colored buttons and text like yellow for selected inspector slots or used in other cases. |
| `Sub` | _direct_ **[PlatformColorPalette.Colors](https://wiki.resonite.com/Component:PlatformColorPalette#Colors)** | A darker color and hexes set used for buttons or UI that are darker due to being selected or used in other cases. |
| `Dark` | _direct_ **[PlatformColorPalette.Colors](https://wiki.resonite.com/Component:PlatformColorPalette#Colors)** | A dark color and hexes set used for buttons or UI that is disabled or used in other cases. |

Fields
Collapse

## Grayscale

| Name | Type | Description |
| --- | --- | --- |
| `DarkHex` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The dark hex code for this color type group |
| `MidHex` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The mid hex code for this color type group |
| `LightHex` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The light hex code for this color type group. |
| `Dark` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The dark color for this color type group. |
| `Mid` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The mid color for this color type group. |
| `Light` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The light color for this color type group. |

Fields

## Colors

| Name | Type | Description |
| --- | --- | --- |
| `YellowHex` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The yellow hex code for this color group. |
| `GreenHex` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The green hex code for this color group. |
| `RedHex` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The red hex code for this color group. |
| `PurpleHex` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The purple hex code for this color group. |
| `CyanHex` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The cyan hex code for this color group. |
| `OrangeHex` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[String](https://wiki.resonite.com/Type:String "Type:String")** | The orange hex code for this color group. |
| `Yellow` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The yellow color for this color group. |
| `Green` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The green color for this color group. |
| `Red` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The red color for this color group. |
| `Purple` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The purple color for this color group. |
| `Cyan` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The cyan color for this color group. |
| `Orange` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX")** | The orange color for this color group. |

Fields

## Usage

Attach to a slot and take any value as a source for a drive to drive a UI with Resonite's branding.

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## See Also

- The colors are in [Resonite's Branding](https://wiki.resonite.com/Branding "Branding").
- These colors can be applied to text by using [Text Formatting](https://wiki.resonite.com/Text_Formatting "Text Formatting").

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PlatformColorPalette&oldid=97670](https://wiki.resonite.com/index.php?title=Component:PlatformColorPalette&oldid=97670)"

Contents