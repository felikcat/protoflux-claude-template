# ProtoFlux:IsNumber

> Source: https://wiki.resonite.com/ProtoFlux:IsNumber

Is Number

Character

\*

Characters

The **Is Number** node takes in a character literal and returns if that character is a number.

## Inputs

### Character ( [char](https://wiki.resonite.com/Type:Char "Type:Char"))

The character literal to check.

## Outputs

### \\* ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Returns `true` if `Character` is a number, `false` otherwise. Numbers recognized by this node are given the Unicode delegation [`Nd`](https://www.compart.com/en/unicode/category/Nd), [`Nl`](https://www.compart.com/en/unicode/category/Nl), or [`No`](https://www.compart.com/en/unicode/category/No).

## Examples

An easy way to remember the difference between this node and the [Is Digit](https://wiki.resonite.com/ProtoFlux:Is_Digit "ProtoFlux:Is Digit") node is: All digits are numbers, but not all numbers are digits.

- ½, ①, 1, 2, 3 all count as numbers.
- 1, 2, 3 also count as digits.

## See Also

- [ProtoFlux:Is Digit](https://wiki.resonite.com/ProtoFlux:Is_Digit "ProtoFlux:Is Digit")
- [Microsoft documentation for the `Char.IsNumber(Char)` function](https://learn.microsoft.com/en-us/dotnet/api/system.char.isnumber#system-char-isnumber(system-char)).

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:IsNumber&oldid=110145](https://wiki.resonite.com/index.php?title=ProtoFlux:IsNumber&oldid=110145)"

Contents