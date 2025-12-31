# ProtoFlux:EncapsulatePoint

> Source: https://wiki.resonite.com/ProtoFlux:EncapsulatePoint

Encapsulate Point

Bounds

\*

Point

Bounds

The **Encapsulate Point** node extends the input Bounds such that the output fully encapsulates the input Point.

## Inputs

### Bounds ( [BoundingBox](https://wiki.resonite.com/Type:BoundingBox "Type:BoundingBox"))

The bounding box to be enlarged. Default value is a bounding box with center \[0;0;0\] and size \[0;0;0\].

### Point ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The point to be encapsulated. Default value is \[0;0;0\]

## Outputs

### \\* ( [BoundingBox](https://wiki.resonite.com/Type:BoundingBox "Type:BoundingBox"))

The Bounds bounding box enlarged to encapsulate the Point. May be identical to Bounds if the Point is already entirely inside Bounds.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:EncapsulatePoint&oldid=109717](https://wiki.resonite.com/index.php?title=ProtoFlux:EncapsulatePoint&oldid=109717)"

Contents