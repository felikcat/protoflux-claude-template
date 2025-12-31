# ProtoFlux:ReleaseAllGrabbed

> Source: https://wiki.resonite.com/ProtoFlux:ReleaseAllGrabbed

Release All Grabbed

\*

Next

Node

SuppressEvents

Grabbable

The `Release All Grabbed` node, when [impulsed](https://wiki.resonite.com/Impulses "Impulses"), makes all [slots](https://wiki.resonite.com/Slot "Slot") the provided [body node](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode") has, to become released. This also has the option to suppress events, useful if the slots were listening using the [On Grabbable Released](https://wiki.resonite.com/ProtoFlux:On_Grabbable_Released "ProtoFlux:On Grabbable Released") node, preventing a lot of pulses from firing.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Call this to make the provided Node ( [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"))'s grabber release everything it is holding.

### Node ( [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"))

The node to find a grabber for so this node can make it release all that it is holding.

### SuppressEvents ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Tells this node to suppress released events that other nodes or components may be listening to. Doesn't prevent code from running that is listening to the grabber of the released objects, however.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Sends an impulse when \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) is called and the provided Node ( [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode")) has had it's grabber release everything it was grabbing.

## Examples

- [An example of Release All Grabbed being used to make a user drop an item if they don't have the proper stats on their user.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Release_All_Grabbed.webp "File:Protoflux example Release All Grabbed.webp")

An example of Release All Grabbed being used to make a user drop an item if they don't have the proper stats on their user.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ReleaseAllGrabbed&oldid=110587](https://wiki.resonite.com/index.php?title=ProtoFlux:ReleaseAllGrabbed&oldid=110587)"

Contents