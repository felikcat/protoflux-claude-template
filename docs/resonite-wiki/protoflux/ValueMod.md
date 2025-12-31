# ProtoFlux:ValueMod

> Source: https://wiki.resonite.com/ProtoFlux:ValueMod

%

A

\*

B

Operators

The **ValueMod** node takes in 2 inputs and returns the remainder value of a division operation. This node goes by names such as "Modulus", "Modulo", and "Mod". (TODO: Does truncation/rounding come into play when using this as an int value compared to float values?)

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you just want the result of a division, use the [Div](https://wiki.resonite.com/ProtoFlux:Div "ProtoFlux:Div") node instead.


![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This node when using negative numbers (in the `A` input), will result in values that enter the excluded range of values (See image of the chart explaining the side effects). Using the [Value Repeat](https://wiki.resonite.com/ProtoFlux:Value_Repeat "ProtoFlux:Value Repeat") node will give different results.


## Inputs

### A (Pseudo-Generic)

Takes in the value for division, this is your current amount to check against.

### B (Pseudo-Generic)

Takes in a value for division, this is your range, or how much you can fill in with your value before it rolls over and starting from 0.

## Outputs

### \\* (Pseudo-Generic)

Returns the remainder value of a division operation.

## Examples

- [![A chart showing the difference between using Modulus and Repeat nodes (courtesy of GManAmby).](https://wiki.resonite.com/images/thumb/5/52/Modulus_VS_Repeat_Node_01.png/480px-Modulus_VS_Repeat_Node_01.png)](https://wiki.resonite.com/File:Modulus_VS_Repeat_Node_01.png "A chart showing the difference between using Modulus and Repeat nodes (courtesy of GManAmby).")

A chart showing the difference between using Modulus and Repeat nodes (courtesy of GManAmby).


## See Also

- Wikipedia's definition of the [Modulo Operator](https://en.wikipedia.org/wiki/Modulo) in Computer Science.
- Microsoft's Documentation on both the [Arithmetic Operators](https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/operators/arithmetic-operators) and the [Mod](https://learn.microsoft.com/en-us/office/vba/language/reference/user-interface-help/mod-operator) reserved keyword.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ValueMod&oldid=111069](https://wiki.resonite.com/index.php?title=ProtoFlux:ValueMod&oldid=111069)"

Contents