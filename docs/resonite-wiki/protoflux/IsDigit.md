# ProtoFlux:IsDigit

> Source: https://wiki.resonite.com/ProtoFlux:IsDigit

Is Digit

Character

\*

Characters

The **Is Digit** node takes in a character literal and returns if that character is a digit. Digit characters are numbers that have a numeric value to them and are not a symbol.

## Inputs

### Character ( [char](https://wiki.resonite.com/Type:Char "Type:Char"))

The character literal to check.

## Outputs

### \\* ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Returns `true` if `Character` is a digit, `false` otherwise. Digits recognized by this node are given [the delegation `Nd` in Unicode](https://www.compart.com/en/unicode/category/Nd)

An easy way to remember the difference between this node and the [Is Number](https://wiki.resonite.com/ProtoFlux:Is_Number "ProtoFlux:Is Number") node is: All digits are numbers, but not all numbers are digits.

- ½, ①, 1, 2, 3 all count as numbers.
- 1, 2, 3 also count as digits.

## Examples

## See Also

- [ProtoFlux:Is Number](https://wiki.resonite.com/ProtoFlux:Is_Number "ProtoFlux:Is Number")
- [Microsoft Documentation for the `Char.IsDigit(Char)` method.](https://learn.microsoft.com/en-us/dotnet/api/system.char.isdigit#system-char-isdigit(system-char))

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:IsDigit&oldid=110109](https://wiki.resonite.com/index.php?title=ProtoFlux:IsDigit&oldid=110109)"

Contents