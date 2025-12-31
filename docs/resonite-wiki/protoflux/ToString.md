# ProtoFlux:ToString

> Source: https://wiki.resonite.com/ProtoFlux:ToString

To String

V

\*

Format

FormatProvider

Strings

The `To String` node turns various [types](https://wiki.resonite.com/Category:Type "Category:Type"), including objects, into [strings](https://wiki.resonite.com/Type:String "Type:String"). In general, this will match the string that a [display node](https://wiki.resonite.com/ProtoFlux:Display "ProtoFlux:Display") displays. Use cases include HUDs that involve numbers, such as turning your FPS into text for a display, or readouts of objects or values.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you are looking to take a string and make it into a value instead, try [Parse](https://wiki.resonite.com/ProtoFlux:Parse "ProtoFlux:Parse").


## Inputs

### V (Generic)

The value to turn into a string.

### Format ( [String](https://wiki.resonite.com/Type:String "Type:String"))

A [Composite Format String](https://learn.microsoft.com/en-us/dotnet/standard/base-types/composite-formatting#composite-format-string).

### FormatProvider ( [IFormatProvider](https://wiki.resonite.com/index.php?title=Type:FormatProvider&action=edit&redlink=1 "Type:FormatProvider (page does not exist)"))

The locale to use for the output. Defaults to the invariant culture.

## Outputs

### \\* ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The value as a string following the format.

## Examples

- [![Four examples of converting various primitives to string. Three of the examples use Standard Numeric Format Strings.](https://wiki.resonite.com/images/thumb/b/b1/Protoflux_example_to_string.webp/480px-Protoflux_example_to_string.webp.png)](https://wiki.resonite.com/File:Protoflux_example_to_string.webp "Four examples of converting various primitives to string. Three of the examples use Standard Numeric Format Strings.")

Four examples of converting various primitives to string. Three of the examples use [Standard Numeric Format Strings](https://learn.microsoft.com/en-us/dotnet/standard/base-types/standard-numeric-format-strings).

- [![Four examples of converting various objects to string. Note how, in general, the output matches what the display node outputs.](https://wiki.resonite.com/images/thumb/c/c0/Protoflux_example_to_string_2.webp/480px-Protoflux_example_to_string_2.webp.png)](https://wiki.resonite.com/File:Protoflux_example_to_string_2.webp "Four examples of converting various objects to string. Note how, in general, the output matches what the display node outputs.")

Four examples of converting various objects to string. Note how, in general, the output matches what the display node outputs.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ToString&oldid=110843](https://wiki.resonite.com/index.php?title=ProtoFlux:ToString&oldid=110843)"

Contents