# ProtoFlux:ContinuouslyChangingRelay

> Source: https://wiki.resonite.com/ProtoFlux:ContinuouslyChangingRelay

Continuous Relay

Input

\*

Utility

The **Continuously Changing Relay** node is a utility node marked with the [ContinuouslyChanging](https://wiki.resonite.com/ContinuouslyChanging "ContinuouslyChanging") attribute. This causes the entire node group that the node is connected to be evaluated every [engine update](https://wiki.resonite.com/Engine_update "Engine update") when paired with a [listener](https://wiki.resonite.com/Type:IExecutionChangeListener "Type:IExecutionChangeListener") node, such as a [drive](https://wiki.resonite.com/Drive "Drive") or [display](https://wiki.resonite.com/ProtoFlux:Display "ProtoFlux:Display").

This node is unnecessary for most use cases, but it can still find usefulness when working with [stores](https://wiki.resonite.com/ProtoFlux:Store "ProtoFlux:Store"), which do not propagate change signals due to existing outside the [FrooxEngine](https://wiki.resonite.com/FrooxEngine "FrooxEngine") [data model](https://wiki.resonite.com/Data_model "Data model"). Additionally, non-ContinuouslyChanging nodes that can have their outputs change without any change in inputs (such as a [Find Child By Name](https://wiki.resonite.com/ProtoFlux:Find_Child_By_Name "ProtoFlux:Find Child By Name") node) can benefit from this relay if the output is needed to drive something that otherwise isn't part of a ContinuousChanges node group.

## Inputs

### Input (Generic)

The output of a previous node that should be continuously polled every engine update.

## Outputs

### \\* (Generic)

The same output, yet continuously changing for future listeners to utilize.

## Examples

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ContinuouslyChangingRelay&oldid=109569](https://wiki.resonite.com/index.php?title=ProtoFlux:ContinuouslyChangingRelay&oldid=109569)"

Contents