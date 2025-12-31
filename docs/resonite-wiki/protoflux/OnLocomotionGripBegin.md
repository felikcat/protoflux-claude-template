# ProtoFlux:OnLocomotionGripBegin

> Source: https://wiki.resonite.com/ProtoFlux:OnLocomotionGripBegin

On Locomotion Grip Begin

OnEvent

GrippedSlot

GrippedPoint

GrippingHand

Locomotion

null

∅

Events

The **On Locomotion Grip Begin** node takes in a global reference from a [user's](https://wiki.resonite.com/Type:User "Type:User") [PhysicalLocomotion](https://wiki.resonite.com/index.php?title=Type:PhysicalLocomotion&action=edit&redlink=1 "Type:PhysicalLocomotion (page does not exist)"). And fires when a grip happens that relates to that locomotion along with the data of the slot, position in 3D space, and what side of the user's grip it was.

## Outputs

### OnEvent ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Fires when a locomotion grip happens.

### GrippedSlot ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot that is being gripped.

### GrippedPoint ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The point in 3D space where the grip is happening.

### GrippingHand ( [Chirality](https://wiki.resonite.com/Type:Chirality "Type:Chirality"))

The side that is being gripped from a user.

## Globals

### Locomotion ( [PhysicalLocomotion](https://wiki.resonite.com/index.php?title=Type:PhysicalLocomotion&action=edit&redlink=1 "Type:PhysicalLocomotion (page does not exist)"))

The global reference to a physical locomotion from a user.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:OnLocomotionGripBegin&oldid=110367](https://wiki.resonite.com/index.php?title=ProtoFlux:OnLocomotionGripBegin&oldid=110367)"

Contents