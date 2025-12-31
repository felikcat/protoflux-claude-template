# ProtoFlux:SlotChildrenEvents

> Source: https://wiki.resonite.com/ProtoFlux:SlotChildrenEvents

Slot Children Events

OnUser

OnChildAdded

OnChildRemoved

Child

Instance

null

∅

Slots

Slot Children events is a ProtoFlux node that monitors a given Instance ( [Slot](https://wiki.resonite.com/Slot "Slot")). It then sends impulses for OnChildAdded ( [Call](https://wiki.resonite.com/Impulses "Impulses")) and OnChildRemoved ( [Call](https://wiki.resonite.com/Impulses "Impulses")) when children are added or removed. When an event trigger happens, Child ( [Slot](https://wiki.resonite.com/Slot "Slot")) is available for reading during the impulse.

## Inputs

### OnUser ( [User](https://wiki.resonite.com/Type:User "Type:User"))

The user that should monitor the given Instance ( [Slot](https://wiki.resonite.com/Slot "Slot")) for slot events. Only if this user sees a slot change will a call be triggered from this node.

When this node is used the user who fires the impulse is determined using the following steps:

1: If null fire the impulse for the user who added/removed the slot.

2: If set to a user, only that user will fire the event.

3: If is connected to a localuser node fire for all users.

Note: unlike fire on true/false/change it does not care if it is under a users avatar, the two above steps are the only ones that exist.

## Outputs

### OnChildAdded ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Sends an impulse when a child is added to Instance ( [Slot](https://wiki.resonite.com/Slot "Slot")) according to what the user provided to OnUser ( [User](https://wiki.resonite.com/Type:User "Type:User")) sees on their client.

### OnChildRemoved ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Sends an impulse when a child is removed from Instance ( [Slot](https://wiki.resonite.com/Slot "Slot")) according to what the user provided to OnUser ( [User](https://wiki.resonite.com/Type:User "Type:User")) sees on their client.

### Child ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The child object that was added or removed from Instance ( [Slot](https://wiki.resonite.com/Slot "Slot")). This will only have a value during an impulse from OnChildAdded ( [Call](https://wiki.resonite.com/Impulses "Impulses")) and OnChildRemoved ( [Call](https://wiki.resonite.com/Impulses "Impulses")).

## Globals

### Instance ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot to monitor for slot events using OnUser ( [User](https://wiki.resonite.com/Type:User "Type:User"))'s client.

## Examples

- [Example of how to use a Slot Children Events to check when a box is put on a shelf.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Slot_Children_Events.webp "File:Protoflux example Slot Children Events.webp")

Example of how to use a Slot Children Events to check when a box is put on a shelf.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:SlotChildrenEvents&oldid=110751](https://wiki.resonite.com/index.php?title=ProtoFlux:SlotChildrenEvents&oldid=110751)"

Contents