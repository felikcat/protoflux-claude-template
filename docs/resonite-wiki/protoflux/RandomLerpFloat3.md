# ProtoFlux:RandomLerpFloat3

> Source: https://wiki.resonite.com/ProtoFlux:RandomLerpFloat3

Random Lerp Float3

Min

\*

Max

Random

The **Random Lerp Float3** node takes in a min and max value and returns a random [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") value.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This node constantly changes its value every frame, if you want to use this value, make sure to either [Write](https://wiki.resonite.com/ProtoFlux:Write "ProtoFlux:Write") to a [Variable](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store") or use it within that frame.


![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

This is a lerp node, meaning that this picks a point between two points randomly, inherently linking them in a sense. If you wanted a random float3, use the [Random Float3](https://wiki.resonite.com/ProtoFlux:Random_Float3 "ProtoFlux:Random Float3") node instead.


## Inputs

### Min ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The minimum this random value can be (exclusive). The default is `0, 0, 0`.

### Max ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The maximum this random value can be (exclusive). The default is `1, 1, 1`.

## Outputs

### \\* ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The random result.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:RandomLerpFloat3&oldid=110503](https://wiki.resonite.com/index.php?title=ProtoFlux:RandomLerpFloat3&oldid=110503)"

Contents