# ProtoFlux:AsyncDynamicImpulseTriggerWithData

> Source: https://wiki.resonite.com/ProtoFlux:AsyncDynamicImpulseTriggerWithData

Async Dynamic Impulse Trigger With Data

\*

Next

Tag

TriggeredCount

TargetHierarchy

ExcludeDisabled

Value

Async

The **Async Dynamic Impulse Trigger With Data** node sends an [async](https://wiki.resonite.com/Async "Async") [dynamic impulse](https://wiki.resonite.com/Dynamic_impulse "Dynamic impulse") to all [Async Dynamic Impulse Receiver With Data](https://wiki.resonite.com/ProtoFlux:Async_Dynamic_Impulse_Receiver_With_Data "ProtoFlux:Async Dynamic Impulse Receiver With Data") nodes with a matching type and tag under the provided `TargetHierarchy`.

## Inputs

### \\* ( [AsyncCall](https://wiki.resonite.com/Impulses "Impulses"))

Trigger an async dynamic impulse with the tag `Tag` and data `Value` under `TargetHierarchy`.

### Tag ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The tag of the dynamic impulse.

### TargetHierarchy ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot under which to search for dynamic impulse receivers.

### ExcludeDisabled ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

If `True`, the dynamic impulse will not search for receivers under disabled slots.

### Value (Generic)

The data to send with the dynamic impulse. Receivers must have a matching type as this value.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Triggered once the [context](https://wiki.resonite.com/Context "Context") of every receiver is completed.

### TriggeredCount ( [Int](https://wiki.resonite.com/Types:Int "Types:Int"))

Number of receivers that were triggered. Only exists for the current ProtoFlux context.

## See Also

- [ProtoFlux:Async Dynamic Impulse Trigger](https://wiki.resonite.com/ProtoFlux:Async_Dynamic_Impulse_Trigger "ProtoFlux:Async Dynamic Impulse Trigger") if data does not need to be sent.
- [ProtoFlux:Dynamic Impulse Trigger With Data](https://wiki.resonite.com/ProtoFlux:Dynamic_Impulse_Trigger_With_Data "ProtoFlux:Dynamic Impulse Trigger With Data") for the sync context analogue.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:AsyncDynamicImpulseTriggerWithData&oldid=109287](https://wiki.resonite.com/index.php?title=ProtoFlux:AsyncDynamicImpulseTriggerWithData&oldid=109287)"

Contents