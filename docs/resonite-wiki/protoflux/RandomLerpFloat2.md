# ProtoFlux:RandomLerpFloat2

> Source: https://wiki.resonite.com/ProtoFlux:RandomLerpFloat2

Random Lerp Float2

Min

\*

Max

Random

The **Random Lerp Float2** node takes in a min and max value and returns a random [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2") value.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This node constantly changes its value every frame, if you want to use this value, make sure to either [Write](https://wiki.resonite.com/ProtoFlux:Write "ProtoFlux:Write") to a [Variable](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store") or use it within that frame.


![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

This is a lerp node, meaning that this picks a point between two points randomly, inherently linking them in a sense. If you wanted a random float2, use the [Random Float2](https://wiki.resonite.com/ProtoFlux:Random_Float2 "ProtoFlux:Random Float2") node instead.


## Inputs

### Min ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

The minimum this random value can be (exclusive). The default is `0, 0`.

### Max ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

The maximum this random value can be (exclusive). The default is `1, 1`.

## Outputs

### \\* ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

The random result.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:RandomLerpFloat2&oldid=110501](https://wiki.resonite.com/index.php?title=ProtoFlux:RandomLerpFloat2&oldid=110501)"

Contents