# ProtoFlux:DynamicImpulseTrigger

> Source: https://wiki.resonite.com/ProtoFlux:DynamicImpulseTrigger

Dynamic Impulse Trigger

\*

Next

Tag

TriggeredCount

TargetHierarchy

ExcludeDisabled

Flow

The **Dynamic Impulse Trigger** node sends a [dynamic impulse](https://wiki.resonite.com/Dynamic_impulse "Dynamic impulse") to all [Dynamic Impulse Receivers](https://wiki.resonite.com/ProtoFlux:Dynamic_Impulse_Receiver "ProtoFlux:Dynamic Impulse Receiver") matching the provided `Tag` under the `TargetHierarchy`.

This node can be used in an [async flow](https://wiki.resonite.com/Async_flow "Async flow") node chain as well, though the node chain for the receiver will not be async.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Trigger a dynamic impulse with the tag `Tag` under `TargetHierarchy`.

### Tag ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The tag of the dynamic impulse.

### TargetHierarchy ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot under which to search for dynamic impulse receivers.

### ExcludeDisabled ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

If `True`, the dynamic impulse will not search for receivers under disabled slots.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Triggered once the [context](https://wiki.resonite.com/Context "Context") of every receiver is completed.

### TriggeredCount ( [Int](https://wiki.resonite.com/Types:Int "Types:Int"))

Number of receivers that were triggered. Only exists for the current [context](https://wiki.resonite.com/Context "Context").

## See Also

- [ProtoFlux:Dynamic Impulse Trigger With Data](https://wiki.resonite.com/ProtoFlux:Dynamic_Impulse_Trigger_With_Data "ProtoFlux:Dynamic Impulse Trigger With Data") to send data with the impulse.
- [ProtoFlux:Async Dynamic Impulse Trigger](https://wiki.resonite.com/ProtoFlux:Async_Dynamic_Impulse_Trigger "ProtoFlux:Async Dynamic Impulse Trigger") for the async analogue.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:DynamicImpulseTrigger&oldid=109691](https://wiki.resonite.com/index.php?title=ProtoFlux:DynamicImpulseTrigger&oldid=109691)"

Contents