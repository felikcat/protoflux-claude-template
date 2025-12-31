# ProtoFlux:RandomLerpColor

> Source: https://wiki.resonite.com/ProtoFlux:RandomLerpColor

Random Lerp Color

Min

\*

Max

Random

The **Random Lerp Color** node takes in a min and max value and returns a random [color](https://wiki.resonite.com/Type:Color "Type:Color") value.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This node constantly changes its value every frame, if you want to use this value, make sure to either [Write](https://wiki.resonite.com/ProtoFlux:Write "ProtoFlux:Write") to a [Variable](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store") or use it within that frame.


![](https://wiki.resonite.com/images/b/b7/DangerIcon.svg)

This node has quick flashing effects, which may cause seizures to light-sensitive and color-sensitive users! Please use caution when using this node or pulling out its display node!


## Inputs

### Min ( [color](https://wiki.resonite.com/Type:Color "Type:Color"))

The minimum this random value can be (inclusive). The default is `0, 0, 0, 0`.

### Max ( [color](https://wiki.resonite.com/Type:Color "Type:Color"))

The maximum this random value can be (exclusive). The default is `0, 0, 0, 0`.

## Outputs

### \\* ( [color](https://wiki.resonite.com/Type:Color "Type:Color"))

The random result.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:RandomLerpColor&oldid=110497](https://wiki.resonite.com/index.php?title=ProtoFlux:RandomLerpColor&oldid=110497)"

Contents