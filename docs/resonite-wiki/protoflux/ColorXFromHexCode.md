# ProtoFlux:ColorXFromHexCode

> Source: https://wiki.resonite.com/ProtoFlux:ColorXFromHexCode

Color XFrom Hex Code

HexCode

Color

Parsed

Colors

Color From Hex Code is a ProtoFlux node that parses a [hex color code](https://en.wikipedia.org/wiki/Web_colors) such as "FFAEBB" into a [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX").

## Inputs

### HexCode ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The hex code to turn into a color. Turns this hex code into a color. The code must be a "#" followed by 3, 4, 6 or 8 hexadecimal digits. The 4 and 8 digit forms specify an alpha component, if not given the alpha component is taken to be 1.

## Outputs

### Color ( [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

A color made from the provided hex code. This value is not defined and may have nonsense values if parsing failed (Parsed = false).

Beware: the resulting color always has the [Linear color profile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile"), which is contrary to how hex color codes are usually interpreted.[\[1\]](https://wiki.resonite.com/ProtoFlux:ColorXFromHexCode#cite_note-1)

### Parsed ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

True if parsing succeeded.

## See Also

- [Color From Hex Code](https://wiki.resonite.com/ProtoFlux:Color_From_Hex_Code "ProtoFlux:Color From Hex Code"): for the [Color](https://wiki.resonite.com/Type:Color "Type:Color") type.

## References

1. [↑](https://wiki.resonite.com/ProtoFlux:ColorXFromHexCode#cite_ref-1 "Jump up")[Resonite Issue #1404: ProtoFlux ColorX From Hex Code should probably return sRGB color space instead](https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/1404)

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ColorXFromHexCode&oldid=109405](https://wiki.resonite.com/index.php?title=ProtoFlux:ColorXFromHexCode&oldid=109405)"

Contents