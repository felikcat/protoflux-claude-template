# ProtoFlux:DivDeltaTime

> Source: https://wiki.resonite.com/ProtoFlux:DivDeltaTime

÷dT

Value

\*

Math

DivDeltaTime is a [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") node which Divides a value by the amount of time passed since the last local update.

This is mostly used in conjunction with the [Delta](https://wiki.resonite.com/Delta_(ProtoFlux) "Delta (ProtoFlux)") node to resolve issues created by differing update rates as it scales deltas to be proportional to time instead of the update rate, which varies.

DivDeltaTime is a convenience node which is equivalent to dividing the input value by [Delta Time](https://wiki.resonite.com/ProtoFlux:Delta_Time "ProtoFlux:Delta Time"). This saves one additional node and some space.

## Inputs

### Value (Pseudo-Generic)

The value to be divided by the time that passed since the last local update.

## Outputs

### \\* (Pseudo-Generic)

The value divided by [Delta Time](https://wiki.resonite.com/ProtoFlux:Delta_Time "ProtoFlux:Delta Time").

## Examples

[![](https://wiki.resonite.com/images/7/72/ProtoFlux_Delta_Example_Direction.png)](https://wiki.resonite.com/File:ProtoFlux_Delta_Example_Direction.png)

Here, the delta position of the movable sphere is divided by delta time such that the resulting change vector is proportional to time (in units per second instead of units per update).

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:DivDeltaTime&oldid=109681](https://wiki.resonite.com/index.php?title=ProtoFlux:DivDeltaTime&oldid=109681)"

Contents