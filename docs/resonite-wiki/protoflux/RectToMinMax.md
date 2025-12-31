# ProtoFlux:RectToMinMax

> Source: https://wiki.resonite.com/ProtoFlux:RectToMinMax

Rect To Min Max

Rect

Min

Max

Rects

The **Rect To Min Max** node takes in a [rect](https://wiki.resonite.com/Type:Rect "Type:Rect") [value](https://wiki.resonite.com/Value_Type "Value Type") and returns 2 specific [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2") values, showing the minimum size of the rect, usually just at the `X` and `Y` position, and also returning the max size of this rect, which is usually `X` \+ `Width` and `Y` \+ `Height`. In contrast to the [Rect To Position Size](https://wiki.resonite.com/ProtoFlux:Rect_To_Position_Size "ProtoFlux:Rect To Position Size") node where it takes the literal position and size to get a rect's bounding data.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you need to make a rect from a min and max size, use the [Rect From Min Max](https://wiki.resonite.com/ProtoFlux:Rect_From_Min_Max "ProtoFlux:Rect From Min Max") node instead.

If you need to split a rect into specific and separated outputs, use the [Rect To XYWH](https://wiki.resonite.com/ProtoFlux:Rect_To_XY_WH "ProtoFlux:Rect To XY WH") node instead.

## Inputs

### Rect ( [Rect](https://wiki.resonite.com/Type:Rect "Type:Rect"))

The rect value.

## Outputs

### Min ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

Returns the minimum size of this rect (usually returning the `X` and `Y` position of this rect).

### Max ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

Returns the maximum size of this rect (usually returning the `X` \+ `Width` and `Y` \+ `Height` of this rect).

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:RectToMinMax&oldid=110567](https://wiki.resonite.com/index.php?title=ProtoFlux:RectToMinMax&oldid=110567)"

Contents