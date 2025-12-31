# ProtoFlux:ColorXSoftAdditiveBlend

> Source: https://wiki.resonite.com/ProtoFlux:ColorXSoftAdditiveBlend

Color XSoft Additive Blend

Source

\*

Destination

Colors

Color X Additive Blend does a "soft additive" blend of its two input colors. The result of the color components is destination color + (source color \* (1 - destination color)). The alpha component is simply added together and clamped to a maximum of 1.

This node is currently bugged and does not properly handle color profile information, simply acting like [Color Soft Additive Blend](https://wiki.resonite.com/ProtoFlux:Color_Soft_Additive_Blend "ProtoFlux:Color Soft Additive Blend") and always returning an [sRGB color profile](https://wiki.resonite.com/Type:ColorProfile "Type:ColorProfile")[\[1\]](https://wiki.resonite.com/ProtoFlux:ColorXSoftAdditiveBlend#cite_note-1).

## Inputs

### Source ( [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The color that is blended "onto" the destination.

### Destination ( [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The destination color that the source is blended "onto".

## Outputs

### \\* ( [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The blended color result.

## See Also

- [Color Soft Additive Blend](https://wiki.resonite.com/ProtoFlux:Color_Soft_Additive_Blend "ProtoFlux:Color Soft Additive Blend"): for the [Color](https://wiki.resonite.com/Type:Color "Type:Color") type.

## References

1. [↑](https://wiki.resonite.com/ProtoFlux:ColorXSoftAdditiveBlend#cite_ref-1 "Jump up")[Resonite Issue #318: Some color manipulation nodes lose color profile information](https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/318)

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ColorXSoftAdditiveBlend&oldid=109443](https://wiki.resonite.com/index.php?title=ProtoFlux:ColorXSoftAdditiveBlend&oldid=109443)"

Contents