# ProtoFlux:Repeat01

> Source: https://wiki.resonite.com/ProtoFlux:Repeat01

Repeat 01

Value

\*

Math

The **Repeat 01** node constrains a number between `0` and `1` by "wrapping around" its value at every integer.

## Inputs

### Value (Pseudo-generic)

The number to constrain.

## Outputs

### \\* (Pseudo-generic)

The value constrained between `0` and `1`. At every integer, the value wraps back to `0`, forming a [sawtooth wave](https://en.wikipedia.org/wiki/Sawtooth_wave) if graphed.

If `Value` is `Infinity`, `-Infinity`, or `NaN`, `NaN` is output.

For types with multiple values, each individual value is put through the function.

## Examples

- [![Float input: 3.7; float output: 0.7. ColorX input: 2, 1.2, -0.2, 0; ColorX output: 0, 0.2, 0.8, 0. Float3 input: NaN, Infinity, -0.3; float3 output: NaN, NaN, 0.7](https://wiki.resonite.com/images/thumb/9/96/Protoflux_example_repeat_01.webp/400px-Protoflux_example_repeat_01.webp.png)](https://wiki.resonite.com/File:Protoflux_example_repeat_01.webp "Three examples of the Repeat 01 node with different types")

Three examples of the Repeat 01 node with different types


## See Also

- [ProtoFlux:Value Repeat](https://wiki.resonite.com/ProtoFlux:Value_Repeat "ProtoFlux:Value Repeat")

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:Repeat01&oldid=110595](https://wiki.resonite.com/index.php?title=ProtoFlux:Repeat01&oldid=110595)"

Contents