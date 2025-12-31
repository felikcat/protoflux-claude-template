# ProtoFlux:ClosestPointOnConeSurface

> Source: https://wiki.resonite.com/ProtoFlux:ClosestPointOnConeSurface

Closest Point On Cone Surface

ConeCenter

ClosestPoint

ConeOrientation

IsPointInside

ConeHeight

ConeBaseRadius

Point

Geometry 3D

The **Closest Point On Cone Surface** node takes in the cone parameters (size and rotation) and a provided point to check. Then it returns the closest point on that cone's surface and if that point is within that cone's defined parameters.

## Inputs

### ConeCenter ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The center of the cone (located at the center of the base of the cone).

### ConeOrientation ( [floatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ"))

The rotation of the cone.

### ConeHeight ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The height of the cone.

### ConeBaseRadius ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The size of the cone base's circle radius.

### Point ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The point we are checking.

## Outputs

### ClosestPoint ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

Returns the point in the cone's surface compared with the point given.

### IsPointInside ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Returns if the point is within this cone.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ClosestPointOnConeSurface&oldid=109373](https://wiki.resonite.com/index.php?title=ProtoFlux:ClosestPointOnConeSurface&oldid=109373)"

Contents