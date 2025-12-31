# ProtoFlux:Div

> Source: https://wiki.resonite.com/ProtoFlux:Div

÷

A

\*

B

Operators

The **Div** node takes in 2 inputs and returns the calculated result. The second input (`B`) will divide the first input (`A`) into sub sections (mathematically speaking), and the result will show how many of our first value will fit into the second value.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you want the remainder of a division, use the [Value Mod](https://wiki.resonite.com/ProtoFlux:Value_Mod "ProtoFlux:Value Mod") node instead. If you want to divide over a set repeated range from a value, use the [Value Repeat](https://wiki.resonite.com/ProtoFlux:Value_Repeat "ProtoFlux:Value Repeat") node instead.


![](https://wiki.resonite.com/images/b/b7/DangerIcon.svg)

It is typically recommended to avoid dividing anything by `0`, it is undefined and returns `Infinity` in the [FrooxEngine](https://wiki.resonite.com/FrooxEngine "FrooxEngine"). Conversely, dividing anything by `Infinity` will return `0`.


Division is non-commutative (known as [Anticommutative](https://en.wikipedia.org/wiki/Anticommutative_property)), which means where you put your inputs matters.

## Inputs

### A (Pseudo-Generic)

The value we have.

### B (Pseudo-Generic)

The value we want to divide from (basically, how many times to cut our first value into to fit these many sub sections).

## Outputs

### \\* (Pseudo-Generic)

The new result from this operation.

## Further Reading

### Magic Numbers For Division

At a low level, computers use a special number to do multiplication for their division operations, known as a [magic number](https://en.wikipedia.org/wiki/Magic_number_(programming)). Each processor is different and may have a different number for calculations, but the video below should explain this concept a bit better.

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## See Also

- Wikipedia's definition of [division](https://en.wikipedia.org/wiki/Division_(mathematics)).
- Microsoft's documentation on the [division](https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/operators/arithmetic-operators) operator.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:Div&oldid=87516](https://wiki.resonite.com/index.php?title=ProtoFlux:Div&oldid=87516)"

Contents