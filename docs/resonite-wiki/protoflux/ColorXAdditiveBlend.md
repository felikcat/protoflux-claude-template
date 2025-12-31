# ProtoFlux:ColorXAdditiveBlend

> Source: https://wiki.resonite.com/ProtoFlux:ColorXAdditiveBlend

Color XAdditive Blend

Source

\*

Destination

Colors

Color Additive Blend does an additive blend of its two input colors. The result is the sum of each component between the target and destination.

This is a symmetric operation, the result is the same with target and destination swapped. Regardless, the "target" and "destination" terminology is used for consistency with other blend nodes.

Alpha values are clamped to a maximum of 1.

This node is currently bugged and does not properly handle color profile information, simply acting like [Color Additive Blend](https://wiki.resonite.com/ProtoFlux:Color_Additive_Blend "ProtoFlux:Color Additive Blend") and always returning an [sRGB color profile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")[\[1\]](https://wiki.resonite.com/ProtoFlux:ColorXAdditiveBlend#cite_note-1).

## Inputs

### Source ( [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The color that is blended "onto" the destination.

### Destination ( [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The destination color that the source is blended "onto".

## Outputs

### \\* ( [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The blended color result.

## References

1. [↑](https://wiki.resonite.com/ProtoFlux:ColorXAdditiveBlend#cite_ref-1 "Jump up")[Resonite Issue #318: Some color manipulation nodes lose color profile information](https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/318)

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ColorXAdditiveBlend&oldid=109401](https://wiki.resonite.com/index.php?title=ProtoFlux:ColorXAdditiveBlend&oldid=109401)"

Contents