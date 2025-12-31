# ProtoFlux:RayToLineIntersectionDistance

> Source: https://wiki.resonite.com/ProtoFlux:RayToLineIntersectionDistance

Ray To Line Intersection Distance

Origin

Distance

Direction

Intersects

LinePoint0

LinePoint1

Geometry 2D

The **Ray To Line Intersection Distance** node determines the distance from a ray origin to the point at which the ray intersects a line _segment_ defined by two points. This node is functionally equivalent to using the [ProtoFlux:Ray To Line Intersection](https://wiki.resonite.com/ProtoFlux:Ray_To_Line_Intersection "ProtoFlux:Ray To Line Intersection") node, then plugging the value used for `Origin` and the `Intersection` output into a [Distance](https://wiki.resonite.com/ProtoFlux:Distance "ProtoFlux:Distance") <float2> node.

## Inputs

### Origin ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

Origin of the ray.

### Direction ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

Direction of the ray.

### LinePoint0 ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

First point of the line segment.

### LinePoint1 ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

Second point of the line segment.

## Outputs

### Distance ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The [Euclidean distance](https://en.wikipedia.org/wiki/Euclidean_distance) between `Origin` and the point at which the defined ray intersects with the line segment with endpoints `LinePoint0` and `LinePoint1`. If the ray does not intersect, the value will be `0`.

### Intersects ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

`True` if the ray intersects with the line segment, `False` otherwise. See [ProtoFlux:Ray To Line Intersection](https://wiki.resonite.com/ProtoFlux:Ray_To_Line_Intersection "ProtoFlux:Ray To Line Intersection") for what counts as intersection.

## See Also

- [ProtoFlux:Ray To Line Intersection](https://wiki.resonite.com/ProtoFlux:Ray_To_Line_Intersection "ProtoFlux:Ray To Line Intersection")

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:RayToLineIntersectionDistance&oldid=110553](https://wiki.resonite.com/index.php?title=ProtoFlux:RayToLineIntersectionDistance&oldid=110553)"

Contents