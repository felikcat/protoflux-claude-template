# ProtoFlux:XOR

> Source: https://wiki.resonite.com/ProtoFlux:XOR

XOR

A

\*

B

Boolean

The **XOR** node takes in two value inputs (either a [bool](https://wiki.resonite.com/Type:Bool "Type:Bool") or a [number](https://wiki.resonite.com/Value_Type "Value Type") value), and functions as both a [logical xor](https://en.wikipedia.org/wiki/Exclusive_or) or [bitwise XOR](https://en.wikipedia.org/wiki/Bitwise_operation#XOR) depending on the type used.

```
- If both inputs are different, then the result will be true.
- If both inputs are the same, then the result will be false.
```

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

The above ruleset breaks when using the [MultiXOR](https://wiki.resonite.com/ProtoFlux:MultiXOR "ProtoFlux:MultiXOR") node, where the resulting output actually alternates when adding more input values. This may be due to how these nodes/code stacks it's operation when calculating the output.


![](https://wiki.resonite.com/images/d/dd/InformationIcon.svg)

This node is similar to the [Xor Elements](https://wiki.resonite.com/ProtoFlux:Xor_Elements "ProtoFlux:Xor Elements") node.


## Inputs

### A (Pseudo-generic)

The first input value.

### B (Pseudo-generic)

The second input value.

## Outputs

### \\* (Pseudo-generic)

Returns the result of a logical XOR of `A` and `B` if the node is a [bool](https://wiki.resonite.com/Type:Bool "Type:Bool") type, bitwise XOR otherwise.

## Further Reading

### Videos

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## See Also

- Wikipedia's definition of [logical xor](https://en.wikipedia.org/wiki/Exclusive_or), [bitwise xor](https://en.wikipedia.org/wiki/Bitwise_operation#XOR), & [xor gate](https://en.wikipedia.org/wiki/XOR_gate).
- Microsoft's documentation on the [xor](https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/operators/boolean-logical-operators) operator.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:XOR&oldid=87634](https://wiki.resonite.com/index.php?title=ProtoFlux:XOR&oldid=87634)"

Contents