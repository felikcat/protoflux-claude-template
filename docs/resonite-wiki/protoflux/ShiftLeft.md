# ProtoFlux:ShiftLeft

> Source: https://wiki.resonite.com/ProtoFlux:ShiftLeft

< <

A

\*

Shift

Boolean

The **Shift Left** node performs a [logical shift](https://en.wikipedia.org/wiki/Logical_shift) of every bit of the input bool vector or integer to the left. Shifting is the act of moving each bit of the input to the left by the shift amount, where bits that fall off the end are lost.

## Inputs

### A (Pseudo-Generic)

The value to shift.

### Shift ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The amount to shift `A` to the left. If the type being shifted is [Long](https://wiki.resonite.com/Type:Long "Type:Long") or [Type:Ulong](https://wiki.resonite.com/Type:Ulong "Type:Ulong"), the shift amount is determined by the lowest six bits of `Shift`. Otherwise, it is determined by the lowest five bits of `Shift`.

## Outputs

### \\* (Pseudo-Generic)

The shifted value.

## Further Reading

### Videos

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## See Also

- [Microsoft documentation on the shifting operators](https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/operators/bitwise-and-shift-operators).

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ShiftLeft&oldid=110741](https://wiki.resonite.com/index.php?title=ProtoFlux:ShiftLeft&oldid=110741)"

Contents