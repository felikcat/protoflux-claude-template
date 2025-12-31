# ProtoFlux:RandomPointOnSquare

> Source: https://wiki.resonite.com/ProtoFlux:RandomPointOnSquare

Random Point On Square

\*

Point

The **Random Point On Square** node returns a random [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2") value of a point on the edge of a [unit square](https://en.wikipedia.org/wiki/Unit_square) centered at `[0; 0]`.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This node is a random node. Random nodes generate a new output every time they are accessed during an [impulse](https://wiki.resonite.com/Impulse "Impulse") chain, even if during the same frame. To reuse the same value for multiple impulse nodes, you _must_ [write](https://wiki.resonite.com/ProtoFlux:Write "ProtoFlux:Write") the value to a [Local](https://wiki.resonite.com/ProtoFlux:Local "ProtoFlux:Local"), [Store](https://wiki.resonite.com/ProtoFlux:Store "ProtoFlux:Store"), or [Data Model Store](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store") before operating on it.


## Outputs

### \\* ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

A random point on the edge of a unit square. This will be a float2 where one value is `-0.5` or `0.5` and the other value is between `-0.5` and `0.5`.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:RandomPointOnSquare&oldid=110525](https://wiki.resonite.com/index.php?title=ProtoFlux:RandomPointOnSquare&oldid=110525)"

Contents