# ProtoFlux:RangeLoopInt

> Source: https://wiki.resonite.com/ProtoFlux:RangeLoopInt

Range Loop

\*

LoopStart

Start

LoopIteration

End

LoopEnd

StepSize

Current

Flow

The **Range Loop Int** node is used to perform looping operations by allowing one to define a range of values and step size for iterations to follow. It is a more flexible version of the [For](https://wiki.resonite.com/ProtoFlux:For "ProtoFlux:For") node.

## Inputs

### \\* ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

Begin the range loop.

### Start ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The number for `Current` to start at during execution.

### End ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The number for `Current` to iterate towards and compare to during execution. This input is inclusive.

### StepSize ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The value that is added or subtracted to `Current` per iteration for the current `LoopIteration`. The loop will either add or subtract this value depending on whether `Start` is less than or greater than `End`. There will be no iterations if this value is less than `1`.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

As of the time of writing, [this node does not account for overflow or underflow when evaluating the loop range](https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/3350). To avoid this issue, make sure that `2147483647 - End >= StepSize` when going forwards or `2147483648 + End >= StepSize` when going backwards.


## Outputs

### LoopStart ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Fires after `*` is pulsed and before any iterations are done. Will be pulsed even if `StepSize < 1`.

### LoopIteration ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Fires for each iteration of the loop. This impulse is triggered until `Current` exceeds `End` in the direction of the loop, at which point the iterations will stop.

### LoopEnd ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires once the loop has finished.

### Current ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

This value will start at `Start` for the first iteration, then at each iteration, this value will either increase or decrease by `StepSize` depending on whether `End` is greater than or less than `Start`. This value lasts for said iteration's entire [context](https://wiki.resonite.com/Context "Context").

## Examples

## See Also

- [ProtoFlux:Async Range Loop Int](https://wiki.resonite.com/ProtoFlux:Async_Range_Loop_Int "ProtoFlux:Async Range Loop Int") for the [async](https://wiki.resonite.com/Async "Async") variant of this node.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:RangeLoopInt&oldid=110541](https://wiki.resonite.com/index.php?title=ProtoFlux:RangeLoopInt&oldid=110541)"

Contents