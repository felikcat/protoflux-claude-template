# ProtoFlux:BlackBodyColorX

> Source: https://wiki.resonite.com/ProtoFlux:BlackBodyColorX

Black Body Color X

Temperature

\*

Colors

Black Body Color X returns a color value of the light emitted by an ideal [black body radiator](https://en.wikipedia.org/wiki/Black-body_radiation). This can be used to calculate appropriate values for various [color temperatures](https://en.wikipedia.org/wiki/Color_temperature).

This node can convert color values in the range 1000 - 40000 Kelvin. Values outside this range are clamped.

The implementation in Resonite appears to use [this table](http://www.vendian.org/mncharity/dir3/blackbody/UnstableURLs/bbr_color.html) as a source of values. For values more granular than 100 Kelvin, the node interpolates linearly between the closest two values.

## Inputs

### Temperature ( [Float](https://wiki.resonite.com/Type:Float "Type:Float"))

The temperature, in Kelvin, to calculate the resulting color for.

## Outputs

### \\* ( [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The color value of the given color temperature.

- [![How to use Black Body Color to specify the color temperature of a light source.](https://wiki.resonite.com/images/thumb/3/32/Protoflux_Black_Body_Color_Light_Example.webp/480px-Protoflux_Black_Body_Color_Light_Example.webp.png)](https://wiki.resonite.com/File:Protoflux_Black_Body_Color_Light_Example.webp "How to use Black Body Color to specify the color temperature of a light source.")

How to use Black Body Color to specify the color temperature of a light source.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:BlackBodyColorX&oldid=109323](https://wiki.resonite.com/index.php?title=ProtoFlux:BlackBodyColorX&oldid=109323)"

Contents