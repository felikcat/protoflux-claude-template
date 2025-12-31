# ProtoFlux:ValueRepeat

> Source: https://wiki.resonite.com/ProtoFlux:ValueRepeat

Repeat

N

\*

Length

Math

The `Value Repeat` node takes in the number value and the expected length range, then returns a value of the expected placement of that number. This is similar to the [Value Mod](https://wiki.resonite.com/ProtoFlux:Value_Mod "ProtoFlux:Value Mod") node.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This node will always return the result of the number from the expected length provided (See image of the chart explaining the side effects). Using the [Value Mod](https://wiki.resonite.com/ProtoFlux:Value_Mod "ProtoFlux:Value Mod") node will give different results.


## Inputs

### N (Pseudo-Generic)

The number value we are checking.

### Length (Pseudo-Generic)

The expected range for our number to be in. If the number we gave rolls over, it will wrap around this length.

## Outputs

### \\* (Pseudo-Generic)

The result of the repeated value.

## Examples

- [![A chart showing the difference between using Modulus and Repeat nodes (courtesy of GManAmby).](https://wiki.resonite.com/images/thumb/5/52/Modulus_VS_Repeat_Node_01.png/480px-Modulus_VS_Repeat_Node_01.png)](https://wiki.resonite.com/File:Modulus_VS_Repeat_Node_01.png "A chart showing the difference between using Modulus and Repeat nodes (courtesy of GManAmby).")

A chart showing the difference between using Modulus and Repeat nodes (courtesy of GManAmby).


## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ValueRepeat&oldid=111081](https://wiki.resonite.com/index.php?title=ProtoFlux:ValueRepeat&oldid=111081)"

Contents