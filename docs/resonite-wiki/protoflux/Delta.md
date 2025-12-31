# ProtoFlux:Delta

> Source: https://wiki.resonite.com/ProtoFlux:Delta

Delta

Value

\*

Math

Returns a change in [value](https://wiki.resonite.com/Value_Type "Value Type"). The [Greek letter Delta (Δ)](https://en.wikipedia.org/wiki/Delta_(letter)) is commonly being used as a variable or symbol related to change.

This node is dependent on your local update rate and its output may differ between users as it is not being synchronized.

This is best used in conjunction with the [DivDeltaTime](https://wiki.resonite.com/ProtoFlux:DivDeltaTime "ProtoFlux:DivDeltaTime") node such that changes are proportional to time instead of the local update rate.

## Inputs

### Value (Pseudo-Generic)

The value for which a delta should be kept track of.

## Outputs

### \\* (Pseudo-Generic)

This is the delta-value, which is the change compared to the last [Local Update](https://wiki.resonite.com/ProtoFlux:Local_Update "ProtoFlux:Local Update").

## Examples

[![](https://wiki.resonite.com/images/7/72/ProtoFlux_Delta_Example_Direction.png)](https://wiki.resonite.com/File:ProtoFlux_Delta_Example_Direction.png)

The delta global position can be used to get the direction and speed an object is moving by. In this example, a sphere can be grabbed and moved around. The direction vector, whose magnitude is its movement speed, is displayed as a debug vector.

[DivDeltaTime](https://wiki.resonite.com/ProtoFlux:DivDeltaTime "ProtoFlux:DivDeltaTime") is being used to normalize the length of the vector over time such that the magnitude corresponds to "distance per second" instead of "distance per update".

## Implementation Details

This node can be implemented using other ProtoFlux nodes:

[![](https://wiki.resonite.com/images/f/f6/ProtoFlux_Delta_Implementation.png)](https://wiki.resonite.com/File:ProtoFlux_Delta_Implementation.png)

In this case, the leftmost Input Node represents the node's input and the Display its output. This implementation of an int Delta Node is equivalent to the implementation in the game's code. How exactly the difference to the previous value is calculated depends on the value type.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:Delta&oldid=103711](https://wiki.resonite.com/index.php?title=ProtoFlux:Delta&oldid=103711)"

Contents