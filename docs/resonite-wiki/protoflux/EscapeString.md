# ProtoFlux:EscapeString

> Source: https://wiki.resonite.com/ProtoFlux:EscapeString

Escape String

String

\*

Strings

The **Escape String** node escapes strings by adding `\` behind special characters. Its intention is for use in an environment with [.NET Regular Expressions](https://learn.microsoft.com/en-us/dotnet/standard/base-types/regular-expressions), but since Resonite does not currently implement any user-facing regex, its usefulness is limited.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you need [percent encoding](https://en.wikipedia.org/wiki/Percent-encoding) for network communication outside of Resonite, use the [Escape Uri Data String](https://wiki.resonite.com/ProtoFlux:Escape_Uri_Data_String "ProtoFlux:Escape Uri Data String") node instead.


### String ( [string](https://wiki.resonite.com/Type:String "Type:String"))

The string to escape.

### \\* ( [string](https://wiki.resonite.com/Type:String "Type:String"))

The escaped string with `\` added behind the following characters: `\`, `*`, `+`, `?`, `|`, `{`, `[`, `(`, `)`, `^`, `$`, `.`, `#`, and [whitespace characters](https://wiki.resonite.com/ProtoFlux:Is_White_Space "ProtoFlux:Is White Space").\
\
## Examples\
\
- [Escape String being used in some ProtoFlux code.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Escape_String.webp "File:Protoflux example Escape String.webp")\
\
Escape String being used in some ProtoFlux code.\
\
\
## See Also\
\
- [Microsoft documentation for its regular expression language](https://learn.microsoft.com/en-us/dotnet/standard/base-types/regular-expression-language-quick-reference).\
- [Microsoft documentation for the `Regex.Escape(String)` method](https://learn.microsoft.com/en-us/dotnet/api/system.text.regularexpressions.regex.escape?view=netframework-4.6).\
\
Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:EscapeString&oldid=109731](https://wiki.resonite.com/index.php?title=ProtoFlux:EscapeString&oldid=109731)"\
\
Contents