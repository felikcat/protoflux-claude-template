# ProtoFlux:ClosestPointOnSphericalSectorSurface

> Source: https://wiki.resonite.com/ProtoFlux:ClosestPointOnSphericalSectorSurface

Closest Point On Spherical Sector Surface

Center

ClosestPoint

Direction

IsPointInside

Radius

Angle

Point

Geometry 3D

The **Closest Point On Spherical Sector Surface** node takes a point in 3D space and computes the closest point on the surface of a spherical sector defined by its center, direction, radius, and angle. Then it returns the closest point on that sphere's surface and if that point is within that sphere's defined parameters.

## Inputs

### Center ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The center of the sphere.

### Direction ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The facing direction of the sphere.

### Radius ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The radius of the sphere.

### Angle ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The angle this point and sphere is going to be using for calculations.

### Point ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The point we are checking.

## Outputs

### ClosestPoint ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

Returns the point in the sphere's surface compared with the point given.

### IsPointInside ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Returns if the point is within this sphere.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ClosestPointOnSphericalSectorSurface&oldid=109377](https://wiki.resonite.com/index.php?title=ProtoFlux:ClosestPointOnSphericalSectorSurface&oldid=109377)"

Contents