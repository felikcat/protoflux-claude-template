# ProtoFlux:Substring

> Source: https://wiki.resonite.com/ProtoFlux:Substring

Substring

Str

\*

StartIndex

Length

Strings

The **Substring** node allows one to get an arbitrary portion of a provided string.

## Inputs

### Str ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The string to remove a segment from.

### StartIndex ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The 0-indexed starting point of retrieval from `Str`.

### Length ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

Length of the output substring. If no node is connected to this input, the substring will continue until the end of the string.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

Strings are UTF-16 encoded, and `Length` represents the amount of UTF16 codepoints in the output string. Usage of this node on a string containing characters outside the [Basic Multilingual Plane](https://en.wikipedia.org/wiki/Plane_(Unicode)#Basic_Multilingual_Plane) may result in confusing behavior, such as the amount of characters in the output string being less than the `Length` value.


## Outputs

### \\* ( [String](https://wiki.resonite.com/Type:String "Type:String"))

A segment of `Str` starting at `StartIndex` with length `Length`. If the segment goes past the end of `Str`, the output is truncated at the end of `Str`. If `Length` is less than `1`, the output will be an [Empty String](https://wiki.resonite.com/ProtoFlux:Empty_String "ProtoFlux:Empty String").

## Examples

- [![The substring node has String input "Cheese Mobile", Start Index 4, and Length 5. The output string is "se Mo".](https://wiki.resonite.com/images/thumb/b/b8/Protoflux_example_Get_Character_Substring.webp/480px-Protoflux_example_Get_Character_Substring.webp.png)](https://wiki.resonite.com/File:Protoflux_example_Get_Character_Substring.webp "Substring being used to tell what's inside of a string in a provided segment, as well as its relation to Get Character.")

Substring being used to tell what's inside of a string in a provided segment, as well as its relation to [Get Character](https://wiki.resonite.com/ProtoFlux:Get_Character "ProtoFlux:Get Character").


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:Substring&oldid=93924](https://wiki.resonite.com/index.php?title=ProtoFlux:Substring&oldid=93924)"

Contents