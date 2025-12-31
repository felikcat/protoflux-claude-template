# ProtoFlux:IsSeparator

> Source: https://wiki.resonite.com/ProtoFlux:IsSeparator

Is Separator

Character

\*

Characters

The **Is Separator** node takes in a character literal and returns if that character is a separator character.

## Inputs

### Character ( [char](https://wiki.resonite.com/Type:Char "Type:Char"))

The character literal to check.

## Outputs

### \\* ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Returns `true` if `Character` is a separator, `false` otherwise. Separator characters recognized by this node are given the Unicode delegation [`Zl`](https://www.compart.com/en/unicode/category/Zl), [`Zp`](https://www.compart.com/en/unicode/category/Zp), or [`Zs`](https://www.compart.com/en/unicode/category/Zs).

## See Also

- [Microsoft Documentation about the `Char.IsSeparator(Char)` method](https://learn.microsoft.com/en-us/dotnet/api/system.char.isseparator#system-char-isseparator(system-char)).

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:IsSeparator&oldid=110155](https://wiki.resonite.com/index.php?title=ProtoFlux:IsSeparator&oldid=110155)"

Contents