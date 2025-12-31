# ProtoFlux:RandomPointInCone

> Source: https://wiki.resonite.com/ProtoFlux:RandomPointInCone

Random Point In Cone

Height

\*

BaseRadius

Point

The **Random Point In Cone** node returns a random point within the bounds of a [cone](https://en.wikipedia.org/wiki/Cone) with the given `Height` and `BaseRadius` centered at `[0; 0; 0]`.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This node is a random node. Random nodes generate a new output every time they are accessed during an [impulse](https://wiki.resonite.com/Impulse "Impulse") chain, even if during the same frame. To reuse the same value for multiple impulse nodes, you _must_ [write](https://wiki.resonite.com/ProtoFlux:Write "ProtoFlux:Write") the value to a [Local](https://wiki.resonite.com/ProtoFlux:Local "ProtoFlux:Local"), [Store](https://wiki.resonite.com/ProtoFlux:Store "ProtoFlux:Store"), or [Data Model Store](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store") before operating on it.


## Inputs

### Height ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The height of the cone.

### BaseRadius ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The radius of the circle base of the cone.

## Outputs

### \\* ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

A random point inside the specified cone. The center of the cone is at `[0; 0; 0]`, making the `y` field anywhere between `-BaseHeight/2` and `+BaseHeight/2`, where the former is the circle side and the latter is the tip side.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:RandomPointInCone&oldid=110509](https://wiki.resonite.com/index.php?title=ProtoFlux:RandomPointInCone&oldid=110509)"

Contents