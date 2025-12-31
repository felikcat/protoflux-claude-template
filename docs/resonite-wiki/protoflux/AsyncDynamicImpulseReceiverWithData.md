# ProtoFlux:AsyncDynamicImpulseReceiverWithData

> Source: https://wiki.resonite.com/ProtoFlux:AsyncDynamicImpulseReceiverWithData

Async Dynamic Impulse Receiver With Data

OnTriggered

Value

Tag

null

∅

Async

The **Async Dynamic Impulse Receiver With Data** node is the recipient of a [dynamic impulse](https://wiki.resonite.com/Dynamic_impulse "Dynamic impulse") with an associated [value](https://wiki.resonite.com/Value_Type "Value Type") or [object](https://wiki.resonite.com/Type:Object "Type:Object") for [async flow](https://wiki.resonite.com/Async_flow "Async flow"). Its trigger analogue is the [Async Dynamic Impulse Trigger With Data](https://wiki.resonite.com/ProtoFlux:Async_Dynamic_Impulse_Trigger_With_Data "ProtoFlux:Async Dynamic Impulse Trigger With Data") node.

## Outputs

### OnTriggered ( [AsyncCall](https://wiki.resonite.com/Impulses "Impulses"))

Sends an [async impulse](https://wiki.resonite.com/Async_impulse "Async impulse") when the node has received a dynamic impulse with the specified `Tag` that has data of the same type as `Value`.

### Value (Generic)

Contains the data sent with the dynamic impulse. Only available during the [context](https://wiki.resonite.com/Context "Context") of the `OnTriggered` impulse.

## Globals

### Tag ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The tag to listen for impulses on.

## See Also

- [ProtoFlux:Dynamic Impulse Receiver With Data](https://wiki.resonite.com/ProtoFlux:Dynamic_Impulse_Receiver_With_Data "ProtoFlux:Dynamic Impulse Receiver With Data") for the sync analogue.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:AsyncDynamicImpulseReceiverWithData&oldid=109283](https://wiki.resonite.com/index.php?title=ProtoFlux:AsyncDynamicImpulseReceiverWithData&oldid=109283)"

Contents