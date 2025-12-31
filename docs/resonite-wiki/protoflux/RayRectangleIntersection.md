# ProtoFlux:RayRectangleIntersection

> Source: https://wiki.resonite.com/ProtoFlux:RayRectangleIntersection

Ray Rectangle Intersection

Origin

Intersection

Direction

Intersects

Rectangle

Geometry 2D

The **Ray Rectangle Intersection** node determines the first point at which a ray defined by an origin and direction intersects the bounds of the provided [Rect](https://wiki.resonite.com/Type:Rect "Type:Rect").

## Inputs

### Origin ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

Origin of the ray.

### Direction ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

Direction of the ray.

### Rectangle ( [Rect](https://wiki.resonite.com/Type:Rect "Type:Rect"))

Rectangle to detect intersections with.

## Outputs

### Intersection ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

The first point at which the defined ray intersects with the bounds of `Rectangle`. If the ray does not intersect, the value will be `[0; 0]`.

### Intersects ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

`True` if the ray intersects with `Rectangle`, `False` otherwise.

## Examples

- [![Inputs: Origin: [-0.6; 0.4], Direction: [3; 2], Rectangle: X=0, Y=0, W=1, H=2. Outputs: Intersection: [0; 0.8], Intersects: True](https://wiki.resonite.com/images/thumb/1/1c/ProtoFlux_Example_Ray_Rectangle_Intersection.webp/400px-ProtoFlux_Example_Ray_Rectangle_Intersection.webp.png)](https://wiki.resonite.com/File:ProtoFlux_Example_Ray_Rectangle_Intersection.webp "An example of the Ray Rectangle Intersection node, along with a graphical visual of the intersection.")

An example of the Ray Rectangle Intersection node, along with a graphical visual of the intersection.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:RayRectangleIntersection&oldid=110547](https://wiki.resonite.com/index.php?title=ProtoFlux:RayRectangleIntersection&oldid=110547)"

Contents