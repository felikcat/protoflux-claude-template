# ProtoFlux:ColorFromHexCode

> Source: https://wiki.resonite.com/ProtoFlux:ColorFromHexCode

Color From Hex Code

HexCode

Color

Parsed

Colors

Color From Hex Code is a ProtoFlux node that parses a [hex color code](https://en.wikipedia.org/wiki/Web_colors) such as "FFAEBB" into a [Color](https://wiki.resonite.com/Type:Color "Type:Color").

## Inputs

### HexCode ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The hex code to turn into a color. Turns this hex code into a color. The code must be a "#" followed by 3, 4, 6 or 8 hexadecimal digits. The 4 and 8 digit forms specify an alpha component, if not given the alpha component is taken to be 1.

## Outputs

### Color ( [Color](https://wiki.resonite.com/Type:Color "Type:Color"))

A color made from the provided hex code. This value is not defined and may have nonsense values if parsing failed (Parsed = false).

### Parsed ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

True if parsing succeeded.

## See Also

- [ColorX From Hex Code](https://wiki.resonite.com/ProtoFlux:ColorX_From_Hex_Code "ProtoFlux:ColorX From Hex Code"): for the [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") type.

## Gallery

- [How to use Color From Hex Code to turn a string hex into a color.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_Color_From_Hex_Code.webp "File:Protoflux Color From Hex Code.webp")

How to use Color From Hex Code to turn a string hex into a color.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ColorFromHexCode&oldid=109479](https://wiki.resonite.com/index.php?title=ProtoFlux:ColorFromHexCode&oldid=109479)"

Contents