# ProtoFlux:ColorXAlphaBlend

> Source: https://wiki.resonite.com/ProtoFlux:ColorXAlphaBlend

Color XAlpha Blend

Source

\*

Destination

Colors

ColorX Alpha Blend does an [alpha blend](https://en.wikipedia.org/wiki/Alpha_compositing) of its two input colors. The source is blended "onto" the destination, and the higher the source alpha, the more of the "source" color and less of the "destination" color comes through.

Alpha values are summed and clamped to a maximum of 1.

This node is currently bugged and does not properly handle color profile information, simply acting like [Color Alpha Blend](https://wiki.resonite.com/ProtoFlux:Color_Alpha_Blend "ProtoFlux:Color Alpha Blend") and always returning an [sRGB color profile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")[\[1\]](https://wiki.resonite.com/ProtoFlux:ColorXAlphaBlend#cite_note-1).

## Inputs

### Source ( [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The color that is blended "onto" the destination.

### Destination ( [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The destination color that the source is blended "onto".

## Outputs

### \\* ( [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The blended color result.

## See Also

- [Color Alpha Blend](https://wiki.resonite.com/ProtoFlux:Color_Alpha_Blend "ProtoFlux:Color Alpha Blend"): for the [Color](https://wiki.resonite.com/Type:Color "Type:Color") type.

## References

1. [↑](https://wiki.resonite.com/ProtoFlux:ColorXAlphaBlend#cite_ref-1 "Jump up")[Resonite Issue #318: Some color manipulation nodes lose color profile information](https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/318)

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ColorXAlphaBlend&oldid=109403](https://wiki.resonite.com/index.php?title=ProtoFlux:ColorXAlphaBlend&oldid=109403)"

Contents