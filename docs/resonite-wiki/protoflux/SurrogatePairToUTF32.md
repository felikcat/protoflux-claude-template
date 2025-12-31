# ProtoFlux:SurrogatePairToUTF32

> Source: https://wiki.resonite.com/ProtoFlux:SurrogatePairToUTF32

Surrogate Pair To UTF32

HighSurrogate

\*

LowSurrogate

Characters

The **Surrogate Pair To UTF32** node returns the codepoint ( [UTF-32](https://wiki.resonite.com/UTF-32 "UTF-32") value) generated from the two surrogate characters.

## Inputs

### HighSurrogate ( [char](https://wiki.resonite.com/Type:Char "Type:Char"))

The high surrogate of the surrogate pair.

### LowSurrogate ( [char](https://wiki.resonite.com/Type:Char "Type:Char"))

The low surrogate of the surrogate pair.

## Outputs

### \\* ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The codepoint generated from the two surrogate characters.

The value `0` is returned instead if either `HighSurrogate` is not a high surrogate or `LowSurrogate` is not a low surrogate.

## See Also

- [The Wikipedia article on UTF-16](https://en.wikipedia.org/wiki/UTF-16#U+D800_to_U+DFFF_(surrogates)), which goes into more depth about how exactly one encodes and decodes a UTF-32 codepoint to and from a surrogate pair.
- [Microsoft documentation for the `Char.ConvertToUtf32(Char, Char)` method.](https://learn.microsoft.com/en-us/dotnet/api/system.char.converttoutf32#system-char-converttoutf32(system-char-system-char))

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:SurrogatePairToUTF32&oldid=110787](https://wiki.resonite.com/index.php?title=ProtoFlux:SurrogatePairToUTF32&oldid=110787)"

Contents