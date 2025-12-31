# ProtoFlux:OnLocomotionGripEnd

> Source: https://wiki.resonite.com/ProtoFlux:OnLocomotionGripEnd

On Locomotion Grip End

OnEvent

GrippedSlot

GrippedPoint

GrippingHand

Locomotion

null

∅

Events

The **On Locomotion Grip End** node takes in a global reference from a [user's](https://wiki.resonite.com/Type:User "Type:User") [PhysicalLocomotion](https://wiki.resonite.com/index.php?title=Type:PhysicalLocomotion&action=edit&redlink=1 "Type:PhysicalLocomotion (page does not exist)"). And fires when a grip ends that relates to that locomotion along with the data of the slot, position in 3D space, and what side of the user's grip it was.

## Outputs

### OnEvent ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Fires when a locomotion grip ends.

### GrippedSlot ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot that has been gripped.

### GrippedPoint ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The point in 3D space where the grip has ended.

### GrippingHand ( [Chirality](https://wiki.resonite.com/Type:Chirality "Type:Chirality"))

The side that has been gripped from a user.

## Globals

### Locomotion ( [PhysicalLocomotion](https://wiki.resonite.com/index.php?title=Type:PhysicalLocomotion&action=edit&redlink=1 "Type:PhysicalLocomotion (page does not exist)"))

The global reference to a physical locomotion from a user.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:OnLocomotionGripEnd&oldid=110369](https://wiki.resonite.com/index.php?title=ProtoFlux:OnLocomotionGripEnd&oldid=110369)"

Contents