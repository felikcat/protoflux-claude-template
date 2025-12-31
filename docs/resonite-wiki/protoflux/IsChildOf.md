# ProtoFlux:IsChildOf

> Source: https://wiki.resonite.com/ProtoFlux:IsChildOf

Is Child Of

Instance

\*

Other

IncludingSelf

Slots

The **Is Child Of** node determines if the `Instance` slot is a descendant of the `Other` slot. This check is recursive.

## Inputs

### Instance ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot to test.

### Other ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The potential parent slot of `Instance`.

### IncludingSelf ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

If `True`, the node will return `True` if `Instance` is the same slot as `Other`. Otherwise, the node will return `False` in this case.

## Outputs

### \\* ( [bool](https://wiki.resonite.com/Types:Bool "Types:Bool"))

Returns `True` if `Instance` is a descendant of the `Other` slot. Otherwise, returns `False`

## Examples

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:IsChildOf&oldid=110101](https://wiki.resonite.com/index.php?title=ProtoFlux:IsChildOf&oldid=110101)"

Contents