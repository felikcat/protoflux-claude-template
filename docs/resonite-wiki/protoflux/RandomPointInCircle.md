# ProtoFlux:RandomPointInCircle

> Source: https://wiki.resonite.com/ProtoFlux:RandomPointInCircle

Random Point In Circle

\*

Point

The **Random Point In Circle** node returns a random [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2") value of a point within the bounds of a [unit circle](https://en.wikipedia.org/wiki/Unit_circle).

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This node is a random node. Random nodes generate a new output every time they are accessed during an [impulse](https://wiki.resonite.com/Impulse "Impulse") chain, even if during the same frame. To reuse the same value for multiple impulse nodes, you _must_ [write](https://wiki.resonite.com/ProtoFlux:Write "ProtoFlux:Write") the value to a [Local](https://wiki.resonite.com/ProtoFlux:Local "ProtoFlux:Local"), [Store](https://wiki.resonite.com/ProtoFlux:Store "ProtoFlux:Store"), or [Data Model Store](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store") before operating on it.


## Outputs

### \\* ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

A random point within the unit circle.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:RandomPointInCircle&oldid=110507](https://wiki.resonite.com/index.php?title=ProtoFlux:RandomPointInCircle&oldid=110507)"

Contents