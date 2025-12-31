# ProtoFlux:ColorXMultiplicativeBlend

> Source: https://wiki.resonite.com/ProtoFlux:ColorXMultiplicativeBlend

Multiplicative Blend

Source

\*

Destination

Colors

ColorX Multiplicative Blend does a multiplicative blend of its two input colors. The result is the product of each component between the target and destination.

This is a symmetric operation, the result is the same with target and destination swapped. Regardless, the "target" and "destination" terminology is used for consistency with other blend nodes.

If the two input colors have a different [ColorProfile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile"), both are converted to Linear before operation. Otherwise the operation is done in the input color profile and returned as such.

## Inputs

### Source ( [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The color that is blended "onto" the destination.

### Destination ( [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The destination color that the source is blended "onto".

## Outputs

### \\* ( [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The blended color result.

## See Also

- [Color Multiplicative Blend](https://wiki.resonite.com/ProtoFlux:Color_Multiplicative_Blend "ProtoFlux:Color Multiplicative Blend"): for the [Type:Color](https://wiki.resonite.com/Type:Color "Type:Color") type.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ColorXMultiplicativeBlend&oldid=109427](https://wiki.resonite.com/index.php?title=ProtoFlux:ColorXMultiplicativeBlend&oldid=109427)"

Contents