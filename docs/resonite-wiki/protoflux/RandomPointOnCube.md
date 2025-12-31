# ProtoFlux:RandomPointOnCube

> Source: https://wiki.resonite.com/ProtoFlux:RandomPointOnCube

Random Point On Cube

\*

Point

The **Random Point On Cube** node returns a random [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") value of a point on the shell of a [unit cube](https://en.wikipedia.org/wiki/Unit_cube) centered at `[0; 0; 0]`.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This node is a random node. Random nodes generate a new output every time they are accessed during an [impulse](https://wiki.resonite.com/Impulse "Impulse") chain, even if during the same frame. To reuse the same value for multiple impulse nodes, you _must_ [write](https://wiki.resonite.com/ProtoFlux:Write "ProtoFlux:Write") the value to a [Local](https://wiki.resonite.com/ProtoFlux:Local "ProtoFlux:Local"), [Store](https://wiki.resonite.com/ProtoFlux:Store "ProtoFlux:Store"), or [Data Model Store](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store") before operating on it.


## Outputs

### \\* ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

A random point on the shell of a unit cube. This will be a float3 where one value is `-0.5` or `0.5` and the other two values are between `-0.5` and `0.5`.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:RandomPointOnCube&oldid=110521](https://wiki.resonite.com/index.php?title=ProtoFlux:RandomPointOnCube&oldid=110521)"

Contents