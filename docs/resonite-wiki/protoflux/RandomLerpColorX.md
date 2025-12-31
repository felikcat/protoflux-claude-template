# ProtoFlux:RandomLerpColorX

> Source: https://wiki.resonite.com/ProtoFlux:RandomLerpColorX

Random Lerp Color X

Min

\*

Max

Random

The **Random Lerp ColorX** node takes in a min and max value and returns a random [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX") value.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This node constantly changes its value every frame, if you want to use this value, make sure to either [Write](https://wiki.resonite.com/ProtoFlux:Write "ProtoFlux:Write") to a [Variable](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store") or use it within that frame.


![](https://wiki.resonite.com/images/b/b7/DangerIcon.svg)

This node has quick flashing effects, which may cause seizures to light-sensitive and color-sensitive users! Please use caution when using this node or pulling out its display node!


## Inputs

### Min ( [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The minimum this random value can be (inclusive). The default is `0, 0, 0, 0`.

### Max ( [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The maximum this random value can be (exclusive). The default is `0, 0, 0, 0`.

## Outputs

### \\* ( [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

The random result.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:RandomLerpColorX&oldid=110499](https://wiki.resonite.com/index.php?title=ProtoFlux:RandomLerpColorX&oldid=110499)"

Contents