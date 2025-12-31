# ProtoFlux:RayToLineIntersection

> Source: https://wiki.resonite.com/ProtoFlux:RayToLineIntersection

Ray To Line Intersection

Origin

Intersection

Direction

Intersects

LinePoint0

LinePoint1

Geometry 2D

The **Ray To Line Intersection** node determines the point at which a ray defined by an origin and direction intersects a line _segment_ defined by two points.

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

### Intersection ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

The point at which the defined ray intersects with the line segment defined by `LinePoint0` and `LinePoint1`. If the ray does not intersect, the value will be `[0; 0]`.

### Intersects ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

`True` if the ray intersects with the line segment, `False` otherwise. If the defined ray has both the same slope and lies on the line segment, it will _not_ count as intersection. If the ray starts on the line segment and has a distinct slope from the line segment, it will count as intersection, and the intersection point will be `Origin`.

## Examples

- [![Inputs: Origin: [2; -1], Direction: [-1; 3], LinePoint0: [-5; 2], LinePoint1: [4; 2]. Outputs: Intersection: [1.3871; 0.3837], Intersects: True](https://wiki.resonite.com/images/thumb/5/51/ProtoFlux_Example_Ray_To_Line_Intersection.webp/400px-ProtoFlux_Example_Ray_To_Line_Intersection.webp.png)](https://wiki.resonite.com/File:ProtoFlux_Example_Ray_To_Line_Intersection.webp "An example of the Ray To Line Intersection node, along with a graphical visual of the intersection.")

An example of the Ray To Line Intersection node, along with a graphical visual of the intersection.

- [![Edge cases of the node. From top left to bottom right: Origin lying on the line segment, but the slope differs; The ray lying on the line segment; and the ray intersecting outside of the two defined points.](https://wiki.resonite.com/images/thumb/f/fa/ProtoFlux_Example_Ray_To_Line_Intersection_Edge_Cases.webp/400px-ProtoFlux_Example_Ray_To_Line_Intersection_Edge_Cases.webp.png)](https://wiki.resonite.com/File:ProtoFlux_Example_Ray_To_Line_Intersection_Edge_Cases.webp "Edge cases of the node. From top left to bottom right: Origin lying on the line segment, but the slope differs; The ray lying on the line segment; and the ray intersecting outside of the two defined points.")

Edge cases of the node. From top left to bottom right: `Origin` lying on the line segment, but the slope differs; The ray lying on the line segment; and the ray intersecting outside of the two defined points.


## See Also

- [ProtoFlux:Ray To Line Intersection Distance](https://wiki.resonite.com/ProtoFlux:Ray_To_Line_Intersection_Distance "ProtoFlux:Ray To Line Intersection Distance")

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:RayToLineIntersection&oldid=110551](https://wiki.resonite.com/index.php?title=ProtoFlux:RayToLineIntersection&oldid=110551)"

Contents