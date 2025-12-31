# ProtoFlux:RectFromPositionSize

> Source: https://wiki.resonite.com/ProtoFlux:RectFromPositionSize

Rect From Position Size

Position

Rect

Size

Rects

The **Rect From Position Size** node takes in 2 specific [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2") values, a position of the rect's `X` and `Y` position, and the size of the rect with the literal `Width` and `Height`, then returns a [rect](https://wiki.resonite.com/Type:Rect "Type:Rect") [value](https://wiki.resonite.com/Value_Type "Value Type"). In contrast to the [Rect From Min Max](https://wiki.resonite.com/ProtoFlux:Rect_From_Min_Max "ProtoFlux:Rect From Min Max") node where it adds the position and size to get a rect's bounding data.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you need to get a rect's position and size, use the [Rect To Position Size](https://wiki.resonite.com/ProtoFlux:Rect_To_Position_Size "ProtoFlux:Rect To Position Size") node instead.

If you want to make a rect using specific and separated inputs, use the [Rect From XYWH](https://wiki.resonite.com/ProtoFlux:Rect_From_XY_WH "ProtoFlux:Rect From XY WH") node instead.

## Inputs

### Position ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

The `X` and `Y` position for this rect.

### Size ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

The literal `Width` and `Height` size for this rect.

## Outputs

### Rect ( [Rect](https://wiki.resonite.com/Type:Rect "Type:Rect"))

Returns the rect value.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:RectFromPositionSize&oldid=110563](https://wiki.resonite.com/index.php?title=ProtoFlux:RectFromPositionSize&oldid=110563)"

Contents