# ProtoFlux:ApplyHDRGammaColorX

> Source: https://wiki.resonite.com/ProtoFlux:ApplyHDRGammaColorX

Apply HDRGamma Color X

Color

\*

Gamma

Colors

The **Apply HDR Gamma Color X** node takes in a color and the amount of gamma to adjust it by, then returns the corrected color. Gamma is used for lightness (called "luminance") color correction, and is standard in many other game titles, films, and photography.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you want the gamma to lower with a higher number, use the [Apply HDR Inverse Gamma ColorX](https://wiki.resonite.com/ProtoFlux:Apply_HDR_Inverse_Gamma_ColorX "ProtoFlux:Apply HDR Inverse Gamma ColorX") node instead.


## Inputs

### Color ( [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The color to adjust.

### Gamma ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The adjustment to the lightness for the input color. Defaults to `2.2`.

## Outputs

### \\* ( [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The gamma corrected colorX.

## See Also

- Wikipedia's definition on [Gamma Correction](https://en.wikipedia.org/wiki/Gamma_correction).

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ApplyHDRGammaColorX&oldid=109265](https://wiki.resonite.com/index.php?title=ProtoFlux:ApplyHDRGammaColorX&oldid=109265)"

Contents