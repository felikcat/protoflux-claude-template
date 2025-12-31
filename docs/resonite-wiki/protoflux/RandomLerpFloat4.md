# ProtoFlux:RandomLerpFloat4

> Source: https://wiki.resonite.com/ProtoFlux:RandomLerpFloat4

Random Lerp Float4

Min

\*

Max

Random

The **Random Lerp Float4** node takes in a min and max value and returns a random [float4](https://wiki.resonite.com/Type:Float4 "Type:Float4") value.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This node constantly changes its value every frame, if you want to use this value, make sure to either [Write](https://wiki.resonite.com/ProtoFlux:Write "ProtoFlux:Write") to a [Variable](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store") or use it within that frame.


![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

This is a lerp node, meaning that this picks a point between two points randomly, inherently linking them in a sense. If you wanted a random float4, use the [Random Float4](https://wiki.resonite.com/ProtoFlux:Random_Float4 "ProtoFlux:Random Float4") node instead.


## Inputs

### Min ( [float4](https://wiki.resonite.com/Type:Float4 "Type:Float4"))

The minimum this random value can be (exclusive). The default is `0, 0, 0, 0`.

### Max ( [float4](https://wiki.resonite.com/Type:Float4 "Type:Float4"))

The maximum this random value can be (exclusive). The default is `1, 1, 1, 1`.

## Outputs

### \\* ( [float4](https://wiki.resonite.com/Type:Float4 "Type:Float4"))

The random result.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:RandomLerpFloat4&oldid=110505](https://wiki.resonite.com/index.php?title=ProtoFlux:RandomLerpFloat4&oldid=110505)"

Contents