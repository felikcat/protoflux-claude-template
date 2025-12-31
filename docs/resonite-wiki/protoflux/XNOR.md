# ProtoFlux:XNOR

> Source: https://wiki.resonite.com/ProtoFlux:XNOR

XNOR

A

\*

B

Boolean

The **XNOR** node takes in two value inputs (either a [bool](https://wiki.resonite.com/Type:Bool "Type:Bool") or a [number](https://wiki.resonite.com/Value_Type "Value Type") value), and functions as both a [logical XNOR](https://en.wikipedia.org/wiki/Logical_biconditional) or bitwise XNOR depending on the type used.

```
- If both inputs are the same value, then the result will be true.
- If both inputs are different values, then the result is false.
```

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

The above ruleset breaks when using the [MultiXNOR](https://wiki.resonite.com/ProtoFlux:MultiXNOR "ProtoFlux:MultiXNOR") node, where the resulting output actually alternates when adding more input values. This may be due to how these nodes/code stacks it's operation when calculating the output.


## Inputs

### A (Pseudo-generic)

The first input value.

### B (Pseudo-generic)

The second input value.

## Outputs

### \\* (Pseudo-generic)

Returns the result of a logical XNOR of `A` and `B` if the node is a [bool](https://wiki.resonite.com/Type:Bool "Type:Bool") type, bitwise XNOR otherwise.

## See Also

- Wikipedia's definition of [logical XNOR](https://en.wikipedia.org/wiki/Logical_biconditional) & [xnor gate](https://en.wikipedia.org/wiki/XNOR_gate).

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:XNOR&oldid=87607](https://wiki.resonite.com/index.php?title=ProtoFlux:XNOR&oldid=87607)"

Contents