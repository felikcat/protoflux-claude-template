# ProtoFlux:IndexOfString

> Source: https://wiki.resonite.com/ProtoFlux:IndexOfString

Index Of String

Str

\*

Part

StartIndex

SearchFromEnd

ComparisonType

Strings

Index Of String is a ProtoFlux node that gives a index of where a string occurs in another string.

The output is at where it starts.

## Inputs

### Str ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The string to search for Part ( [String](https://wiki.resonite.com/Type:String "Type:String")) in.

### Part ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The string to look for inside of Str ( [String](https://wiki.resonite.com/Type:String "Type:String")). Returns `-1` if not found.

### StartIndex ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The position after which to start searching. Default `0`.

### SearchFromEnd ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Whether this should start searching from the end rather than the beginning after StartIndex ( [int](https://wiki.resonite.com/Type:Int "Type:Int")).

### ComparisonType ( [StringComparison](https://wiki.resonite.com/Type:StringComparison "Type:StringComparison"))

The string comparison to use.

## Outputs

### \\* ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The index where Part ( [String](https://wiki.resonite.com/Type:String "Type:String")) first occurs after StartIndex ( [int](https://wiki.resonite.com/Type:Int "Type:Int")) in Str ( [String](https://wiki.resonite.com/Type:String "Type:String")). The number returned is at where the occurrence starts.

## Examples

- [An example of Index Of String being used to splice a string for parsing.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Index_Of_String.webp "File:Protoflux example Index Of String.webp")

An example of Index Of String being used to splice a string for parsing.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:IndexOfString&oldid=110055](https://wiki.resonite.com/index.php?title=ProtoFlux:IndexOfString&oldid=110055)"

Contents