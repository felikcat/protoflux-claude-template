# ProtoFlux:IsSymbol

> Source: https://wiki.resonite.com/ProtoFlux:IsSymbol

Is Symbol

Character

\*

Characters

The **Is Symbol** node takes in a character literal and returns if that character is a symbol as defined by Unicode.

## Inputs

### Character ( [char](https://wiki.resonite.com/Type:Char "Type:Char"))

The character literal to check.

## Outputs

### \\* ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Returns `true` if `Character` is a symbol, `false` otherwise. Symbol characters recognized by this node are given the unicode delegation [`Sm`](https://www.compart.com/en/unicode/category/Sm), [`Sc`](https://www.compart.com/en/unicode/category/Sc), [`Sk`](https://www.compart.com/en/unicode/category/Sk), or [`So`](https://www.compart.com/en/unicode/category/So).

## See Also

- [Microsoft Documentation about the `Char.IsSymbol(Char)` method](https://learn.microsoft.com/en-us/dotnet/api/system.char.issymbol#system-char-issymbol(system-char)).

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:IsSymbol&oldid=110161](https://wiki.resonite.com/index.php?title=ProtoFlux:IsSymbol&oldid=110161)"

Contents