# ProtoFlux:RectFromMinMax

> Source: https://wiki.resonite.com/ProtoFlux:RectFromMinMax

Rect From Min Max

Min

Rect

Max

Rects

The **Rect From Min Max** node takes in 2 specific [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2") values, giving the minimum size of the rect, usually just at the `X` and `Y` position, and also needing the max size of this rect, which is usually `X` \+ `Width` and `Y` \+ `Height`. Then this node returns a [rect](https://wiki.resonite.com/Type:Rect "Type:Rect") [value](https://wiki.resonite.com/Value_Type "Value Type") that has the min and max provided. In contrast to the [Rect From Position Size](https://wiki.resonite.com/ProtoFlux:Rect_From_Position_Size "ProtoFlux:Rect From Position Size") node where it takes the literal position and size to get a rect's bounding data.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you need the min and max values from a rect, use the [Rect To Min Max](https://wiki.resonite.com/ProtoFlux:Rect_To_Min_Max "ProtoFlux:Rect To Min Max") node instead.

If you want to make a rect using specific and separated inputs, use the [Rect From XYWH](https://wiki.resonite.com/ProtoFlux:Rect_From_XY_WH "ProtoFlux:Rect From XY WH") node instead.

## Inputs

### Min ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

The minimum size of this rect (usually returning the `X` and `Y` position of this rect).

### Max ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

The maximum size of this rect (usually returning the `X` \+ `Width` and `Y` \+ `Height` of this rect).

## Outputs

### Rect ( [Rect](https://wiki.resonite.com/Type:Rect "Type:Rect"))

Returns the rect value.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:RectFromMinMax&oldid=110561](https://wiki.resonite.com/index.php?title=ProtoFlux:RectFromMinMax&oldid=110561)"

Contents