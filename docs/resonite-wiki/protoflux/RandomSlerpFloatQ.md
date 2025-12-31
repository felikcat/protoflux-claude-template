# ProtoFlux:RandomSlerpFloatQ

> Source: https://wiki.resonite.com/ProtoFlux:RandomSlerpFloatQ

Random Slerp FloatQ

Min

\*

Max

Random

The **Random Slerp FloatQ** node takes in a min and max value and returns a random [floatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ") value.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This node constantly changes its value every frame, if you want to use this value, make sure to either [Write](https://wiki.resonite.com/ProtoFlux:Write "ProtoFlux:Write") to a [Variable](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store") or use it within that frame.


![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

This is a slerp node, meaning that this picks a point between two spherical rotations randomly, inherently linking them in a sense. If you wanted a random floatQ, use the [Random Rotation](https://wiki.resonite.com/ProtoFlux:Random_Rotation "ProtoFlux:Random Rotation") node instead.


## Inputs

### Min ( [floatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ"))

The minimum this random value can be (exclusive). The default is `0, 0, 0`.

### Max ( [floatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ"))

The maximum this random value can be (exclusive). The default is `0, 0, 0`.

## Outputs

### \\* ( [floatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ"))

The random result.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:RandomSlerpFloatQ&oldid=110537](https://wiki.resonite.com/index.php?title=ProtoFlux:RandomSlerpFloatQ&oldid=110537)"

Contents