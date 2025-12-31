# ProtoFlux:IsPunctuation

> Source: https://wiki.resonite.com/ProtoFlux:IsPunctuation

Is Punctuation

Character

\*

Characters

The **Is Punctuation** node takes in a character literal and returns if that character is a punctuation character.

## Inputs

### Character ( [char](https://wiki.resonite.com/Type:Char "Type:Char"))

The character literal to check.

## Outputs

### \\* ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Returns `true` if `Character` is a punctuation character, `false` otherwise. Punctuation characters recognized by this node are given the Unicode delegation [`Pc`](https://www.compart.com/en/unicode/category/Pc), [`Pd`](https://www.compart.com/en/unicode/category/Pd), [`Ps`](https://www.compart.com/en/unicode/category/Ps), [`Pe`](https://www.compart.com/en/unicode/category/Pe), [`Pi`](https://www.compart.com/en/unicode/category/Pi), [`Pf`](https://www.compart.com/en/unicode/category/Pf), or [`Po`](https://www.compart.com/en/unicode/category/Po).

## See Also

- [Microsoft documentation of the `Char.IsPunctuation(Char)` method](https://learn.microsoft.com/en-us/dotnet/api/system.char.ispunctuation#system-char-ispunctuation(system-char)).

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:IsPunctuation&oldid=110151](https://wiki.resonite.com/index.php?title=ProtoFlux:IsPunctuation&oldid=110151)"

Contents