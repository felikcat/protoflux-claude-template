# ProtoFlux:DelayUpdates

> Source: https://wiki.resonite.com/ProtoFlux:DelayUpdates

Delay Updates

\*

Next

Updates

OnTriggered

Async

Delay Updates is a ProtoFlux node that will send an impulse out of Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses")) after Updates ( [int](https://wiki.resonite.com/Type:Int "Type:Int")) updates after \* ( [ASync Call](https://wiki.resonite.com/Impulses#ASync "Impulses")) is impulsed.

## Inputs

### \\* ( [ASync Call](https://wiki.resonite.com/Impulses\#ASync "Impulses"))

Call to start the delay.

### Updates ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

How many updates to delay for.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires after Updates ( [int](https://wiki.resonite.com/Type:Int "Type:Int")) updates has passed after an impulse has been sent to \* ( [ASync Call](https://wiki.resonite.com/Impulses#ASync "Impulses")).

### OnTriggered ( [ASync Call](https://wiki.resonite.com/Impulses\#ASync "Impulses"))

fires immediately after \* ( [ASync Call](https://wiki.resonite.com/Impulses#ASync "Impulses")) is called.

## Examples

- [Delay Updates being used in a code to reset a value for a visual after a button being pressed and x time passing.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Delay_Updates.webp "File:Protoflux example Delay Updates.webp")

Delay Updates being used in a code to reset a value for a visual after a button being pressed and x time passing.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:DelayUpdates&oldid=109651](https://wiki.resonite.com/index.php?title=ProtoFlux:DelayUpdates&oldid=109651)"

Contents