# ProtoFlux:EncapsulateBounds

> Source: https://wiki.resonite.com/ProtoFlux:EncapsulateBounds

Encapsulate Bounds

Bounds

\*

OtherBounds

Bounds

The **Encapsulate Bounds** node extends the input Bounds such that the output fully encapsulates the OtherBounds.

## Inputs

### Bounds ( [BoundingBox](https://wiki.resonite.com/Type:BoundingBox "Type:BoundingBox"))

The bounding box to be enlarged. Default value is a bounding box with center \[0;0;0\] and size \[0;0;0\].

### OtherBounds ( [BoundingBox](https://wiki.resonite.com/Type:BoundingBox "Type:BoundingBox"))

The bounding box to be encapsulated. Default value is a bounding box with center \[0;0;0\] and size \[0;0;0\].

## Outputs

### \\* ( [BoundingBox](https://wiki.resonite.com/Type:BoundingBox "Type:BoundingBox"))

The Bounds bounding box enlarged to fully encapsulate the OtherBounds. May be identical to Bounds if the OtherBounds is already entirely inside Bounds.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:EncapsulateBounds&oldid=109715](https://wiki.resonite.com/index.php?title=ProtoFlux:EncapsulateBounds&oldid=109715)"

Contents