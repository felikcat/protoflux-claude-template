# ProtoFlux:EscapeUriDataString

> Source: https://wiki.resonite.com/ProtoFlux:EscapeUriDataString

Escape Uri Data String

String

\*

Network

The `Escape Uri Data String` node takes in a string literal and converts that string into another string that uses [Percent Encoding](https://en.wikipedia.org/wiki/Percent-encoding). This is used mostly for applications that can only read the ASCII representation of characters.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

This node should not be confused with the [Escape String](https://wiki.resonite.com/ProtoFlux:Escape_String "ProtoFlux:Escape String") node, which has the output of `\` as the escaped string. If you need separator characters for file paths, use that node instead.


## Inputs

### \\* ( [string](https://wiki.resonite.com/Type:String "Type:String"))

The string literal that we want to encode.

## Outputs

### \\* ( [string](https://wiki.resonite.com/Type:String "Type:String"))

The encoded string literal.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:EscapeUriDataString&oldid=109733](https://wiki.resonite.com/index.php?title=ProtoFlux:EscapeUriDataString&oldid=109733)"

Contents