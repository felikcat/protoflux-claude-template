# ProtoFlux:RandomPointInCube

> Source: https://wiki.resonite.com/ProtoFlux:RandomPointInCube

Random Point In Cube

\*

Point

The **Random Point In Cube** node returns a random [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") value of a point within the bounds of a [unit cube](https://en.wikipedia.org/wiki/Unit_cube) centered at `[0; 0; 0]`.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This node is a random node. Random nodes generate a new output every time they are accessed during an [impulse](https://wiki.resonite.com/Impulse "Impulse") chain, even if during the same frame. To reuse the same value for multiple impulse nodes, you _must_ [write](https://wiki.resonite.com/ProtoFlux:Write "ProtoFlux:Write") the value to a [Local](https://wiki.resonite.com/ProtoFlux:Local "ProtoFlux:Local"), [Store](https://wiki.resonite.com/ProtoFlux:Store "ProtoFlux:Store"), or [Data Model Store](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store") before operating on it.


## Outputs

### \\* ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

A random point within the unit cube centered at `[0; 0; 0]`.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:RandomPointInCube&oldid=110511](https://wiki.resonite.com/index.php?title=ProtoFlux:RandomPointInCube&oldid=110511)"

Contents