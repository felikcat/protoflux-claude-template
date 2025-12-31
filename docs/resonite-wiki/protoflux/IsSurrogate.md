# ProtoFlux:IsSurrogate

> Source: https://wiki.resonite.com/ProtoFlux:IsSurrogate

Is Surrogate

Character

\*

Characters

The **Is Surrogate** node takes in a [char](https://wiki.resonite.com/Type:Char "Type:Char") and returns whether that character is a surrogate.

Surrogates are special values in [UTF-16](https://wiki.resonite.com/UTF-16 "UTF-16") that, in pairs, allows representing characters outside the [Basic Multilingual Plane](https://en.wikipedia.org/wiki/Plane_(Unicode)#Basic_Multilingual_Plane).

## Inputs

### Character ( [char](https://wiki.resonite.com/Type:Char "Type:Char"))

The character to check.

## Outputs

### \\* ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Returns `true` if `Character` is a surrogate, `false` otherwise. Surrogate characters recognized by this node are all characters between `U+D800` and `U+DFFF`.

## See Also

- [Microsoft Documentation about the `Char.IsSurrogate(Char)` method](https://learn.microsoft.com/en-us/dotnet/api/system.char.issurrogate#system-char-issurrogate(system-char)).

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:IsSurrogate&oldid=110159](https://wiki.resonite.com/index.php?title=ProtoFlux:IsSurrogate&oldid=110159)"

Contents