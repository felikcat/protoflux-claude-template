# ProtoFlux:RectToPositionSize

> Source: https://wiki.resonite.com/ProtoFlux:RectToPositionSize

Rect To Position Size

Rect

Position

Size

Rects

The **Rect To Position Size** node takes in a [rect](https://wiki.resonite.com/Type:Rect "Type:Rect") [value](https://wiki.resonite.com/Value_Type "Value Type") and returns 2 specific [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2") values giving a position of the rect's `X` and `Y` position, and giving the size of the rect with the literal `Width` and `Height`. In contrast to the [Rect To Min Max](https://wiki.resonite.com/ProtoFlux:Rect_To_Min_Max "ProtoFlux:Rect To Min Max") node where it adds the position and size to get a rect's bounding data.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you need to make a rect from a position and size, use the [Rect From Position Size](https://wiki.resonite.com/ProtoFlux:Rect_From_Position_Size "ProtoFlux:Rect From Position Size") node instead.

If you need to split a rect into specific and separated outputs, use the [Rect To XYWH](https://wiki.resonite.com/ProtoFlux:Rect_To_XY_WH "ProtoFlux:Rect To XY WH") node instead.

## Inputs

### Rect ( [Rect](https://wiki.resonite.com/Type:Rect "Type:Rect"))

The rect value.

## Outputs

### Position ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

Returns the `X` and `Y` position of this rect.

### Size ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

Returns the literal `Width` and `Height` size of this rect.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:RectToPositionSize&oldid=110569](https://wiki.resonite.com/index.php?title=ProtoFlux:RectToPositionSize&oldid=110569)"

Contents