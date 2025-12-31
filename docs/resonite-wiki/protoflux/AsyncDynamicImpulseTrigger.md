# ProtoFlux:AsyncDynamicImpulseTrigger

> Source: https://wiki.resonite.com/ProtoFlux:AsyncDynamicImpulseTrigger

Async Dynamic Impulse Trigger

\*

Next

Tag

TriggeredCount

TargetHierarchy

ExcludeDisabled

Async

The **Async Dynamic Impulse Trigger** node sends an [async](https://wiki.resonite.com/Async "Async") [dynamic impulse](https://wiki.resonite.com/Dynamic_impulse "Dynamic impulse") to all [Async Dynamic Impulse Receivers](https://wiki.resonite.com/ProtoFlux:Async_Dynamic_Impulse_Receiver "ProtoFlux:Async Dynamic Impulse Receiver") matching the provided `Tag` under the `TargetHierarchy`.

## Inputs

### \\* ( [AsyncCall](https://wiki.resonite.com/Impulses "Impulses"))

Trigger an async dynamic impulse with the tag `Tag` under `TargetHierarchy`.

### Tag ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The tag of the dynamic impulse.

### TargetHierarchy ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot under which to search for dynamic impulse receivers.

### ExcludeDisabled ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

If `True`, the dynamic impulse will not search for receivers under disabled slots.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Triggered once the context of every receiver is completed.

### TriggeredCount ( [Int](https://wiki.resonite.com/Types:Int "Types:Int"))

Number of receivers that were triggered. Only exists for the current [context](https://wiki.resonite.com/Context "Context").

## See Also

- [ProtoFlux:Async Dynamic Impulse Trigger With Data](https://wiki.resonite.com/ProtoFlux:Async_Dynamic_Impulse_Trigger_With_Data "ProtoFlux:Async Dynamic Impulse Trigger With Data") to send data with the impulse.
- [ProtoFlux:Dynamic Impulse Trigger](https://wiki.resonite.com/ProtoFlux:Dynamic_Impulse_Trigger "ProtoFlux:Dynamic Impulse Trigger") for the sync analogue.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:AsyncDynamicImpulseTrigger&oldid=109285](https://wiki.resonite.com/index.php?title=ProtoFlux:AsyncDynamicImpulseTrigger&oldid=109285)"

Contents