# ProtoFlux:ShiftRight

> Source: https://wiki.resonite.com/ProtoFlux:ShiftRight

\> >

A

\*

Shift

Boolean

The **Shift Right** node shifts every bit of the input bool vector or integer to the right. Shifting is the act of moving each bit of the input to the right by the shift amount, where bits that fall off the end are lost.

## Inputs

### A (Pseudo-Generic)

The value to shift.

### Shift ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The amount to shift `A` to the right. If the type being shifted is [Long](https://wiki.resonite.com/Type:Long "Type:Long") or [Type:Ulong](https://wiki.resonite.com/Type:Ulong "Type:Ulong"), the shift amount is determined by the lowest six bits of `Shift`. Otherwise, it is determined by the lowest five bits of `Shift`.

## Outputs

### \\* (Pseudo-Generic)

The shifted value. If the type of `A` is a signed type, such as [Type:Int](https://wiki.resonite.com/Type:Int "Type:Int") or [Type:Long](https://wiki.resonite.com/Type:Long "Type:Long"), this node performs an [arithmetic shift](https://en.wikipedia.org/wiki/Arithmetic_shift) on `A`, which copies the most significant bit to each lower bit for the shift amount. Otherwise, it performs a [logical shift](https://en.wikipedia.org/wiki/Logical_shift) on `A`, where the highest-order bits are filled with `0` or `False` for the shift amount.

## Further Reading

### Videos

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## See Also

- [Microsoft documentation on the shifting operators](https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/operators/bitwise-and-shift-operators).

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ShiftRight&oldid=110745](https://wiki.resonite.com/index.php?title=ProtoFlux:ShiftRight&oldid=110745)"

Contents