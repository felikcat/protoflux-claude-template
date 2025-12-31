# ProtoFlux:ClipRect

> Source: https://wiki.resonite.com/ProtoFlux:ClipRect

Clip Rect

Rect

\*

Mask

Rects

The **Clip Rect** node takes in 2 [rect](https://wiki.resonite.com/Type:Rect "Type:Rect") [values](https://wiki.resonite.com/Value_Type "Value Type"), and returns a rect that is inside both of them into one rect.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you need to check for the entire bounds of 2 rects, use the [Encapsulate Rect](https://wiki.resonite.com/ProtoFlux:Encapsulate_Rect "ProtoFlux:Encapsulate Rect") node instead.


## Inputs

### Rect ( [Rect](https://wiki.resonite.com/Type:Rect "Type:Rect"))

The first rect.

### Mask ( [Rect](https://wiki.resonite.com/Type:Rect "Type:Rect"))

The second rect, the one that overlaps the first rect.

## Outputs

### \\* ( [Rect](https://wiki.resonite.com/Type:Rect "Type:Rect"))

Returns the rect that is inside the 2 provided rects.

## Examples

- [![An example of the Clip Rect node in action, drawn out using Debug Line nodes, Rect 1 = Red, Rect 2 = Green, Rect 3 = Blue.](https://wiki.resonite.com/images/thumb/2/28/ClipRectExample01.png/386px-ClipRectExample01.png)](https://wiki.resonite.com/File:ClipRectExample01.png "An example of the Clip Rect node in action, drawn out using Debug Line nodes, Rect 1 = Red, Rect 2 = Green, Rect 3 = Blue.")

An example of the Clip Rect node in action, drawn out using [Debug Line](https://wiki.resonite.com/ProtoFlux:Debug_Line "ProtoFlux:Debug Line") nodes, Rect 1 = Red, Rect 2 = Green, Rect 3 = Blue.

- [![Some code that draws 3 rects (using Debug Line nodes), Rect 1 = Red, Rect 2 = Green, Rect 3 = Blue.](https://wiki.resonite.com/images/thumb/7/76/ExampleCode_DebugRect01.png/478px-ExampleCode_DebugRect01.png)](https://wiki.resonite.com/File:ExampleCode_DebugRect01.png "Some code that draws 3 rects (using Debug Line nodes), Rect 1 = Red, Rect 2 = Green, Rect 3 = Blue.")

Some code that draws 3 [rects](https://wiki.resonite.com/Type:Rect "Type:Rect") (using [Debug Line](https://wiki.resonite.com/ProtoFlux:Debug_Line "ProtoFlux:Debug Line") nodes), Rect 1 = Red, Rect 2 = Green, Rect 3 = Blue.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ClipRect&oldid=109367](https://wiki.resonite.com/index.php?title=ProtoFlux:ClipRect&oldid=109367)"

Contents