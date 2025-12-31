# ProtoFlux:OnGrabbableReceiverSurfaceReceived

> Source: https://wiki.resonite.com/ProtoFlux:OnGrabbableReceiverSurfaceReceived

On Grabbable Receiver Surface Received

OnRecieved

RecievedGrabbable

FromGrabber

Source

null

∅

Grabbable

On Grabbable Receiver Surface Received is a ProtoFlux node that monitors a Reciever for when a grabbable is let go of and is received by the Source ( [GrabbableReceiverSurface](https://wiki.resonite.com/Types:GrabbableReceiverSurface "Types:GrabbableReceiverSurface")). The node then sends an [Impulse](https://wiki.resonite.com/Impulses "Impulses").

## Outputs

### OnReceived ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Sends an impulse when Grabbable ( [IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable")) is let go of and is received by the Source ( [GrabbableReceiverSurface](https://wiki.resonite.com/Types:GrabbableReceiverSurface "Types:GrabbableReceiverSurface")).

### RecievedGrabbable ( [IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable"))

The grabbable that was recieved, only has a value during the OnReceived ( [Call](https://wiki.resonite.com/Impulses "Impulses")) impulse.

### FromGrabber ( [Grabber](https://wiki.resonite.com/Type:Grabber "Type:Grabber"))

The grabber that let go of the RecievedGrabbable ( [IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable")).

## Globals

### Source ( [GrabbableReceiverSurface](https://wiki.resonite.com/Types:GrabbableReceiverSurface "Types:GrabbableReceiverSurface"))

The [GrabbableReceiverSurface](https://wiki.resonite.com/Types:GrabbableReceiverSurface "Types:GrabbableReceiverSurface") to monitor for an [IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable") is recieved by it.

## Examples

- [An example of On Grabbable Receiver Surface Received being used to check if the object that was received by a shelf was a vase.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_On_Grabbable_Receiver_Surface_Received.webp "File:Protoflux example On Grabbable Receiver Surface Received.webp")

An example of On Grabbable Receiver Surface Received being used to check if the object that was received by a shelf was a vase.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:OnGrabbableReceiverSurfaceReceived&oldid=110355](https://wiki.resonite.com/index.php?title=ProtoFlux:OnGrabbableReceiverSurfaceReceived&oldid=110355)"

Contents