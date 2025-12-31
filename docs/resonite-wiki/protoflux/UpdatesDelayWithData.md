# ProtoFlux:UpdatesDelayWithData

> Source: https://wiki.resonite.com/ProtoFlux:UpdatesDelayWithData

Updates Delay With Data

\*

Next

Updates

OnTriggered

Value

DelayedValue

Async

Updates Delay With Data is a ProtoFlux node that will send an impulse out of Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses")) after Updates ( [int](https://wiki.resonite.com/Type:Int "Type:Int")) updates after \* ( [ASync Call](https://wiki.resonite.com/Impulses#ASync "Impulses")) is impulsed. It will carry a value and keep it during the duration of the delay and spit it out after the delay.

## Inputs

### \\* ( [ASync Call](https://wiki.resonite.com/Impulses\#ASync "Impulses"))

Call to start the delay.

### Updates ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

How many updates to delay for.

### Value (Generic)

The value to delay. Can be any type.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires after Updates ( [int](https://wiki.resonite.com/Type:Int "Type:Int")) updates has passed after an impulse has been sent to \* ( [ASync Call](https://wiki.resonite.com/Impulses#ASync "Impulses")).

### OnTriggered ( [ASync Call](https://wiki.resonite.com/Impulses\#ASync "Impulses"))

fires immediately after \* ( [ASync Call](https://wiki.resonite.com/Impulses#ASync "Impulses")) is called.

### DelayedValue (Generic)

Has a value during the Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses")) impulse and outputs the value that was provided to Value (Generic) when \* ( [ASync Call](https://wiki.resonite.com/Impulses#ASync "Impulses")) was impulsed.

## Examples

- [Updates Delay With Data being used in a code to keep a value from a Source till after the delay and using DelayedValue rather than using the Source directly after the delay.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Updates_Delay_With_Data.webp "File:Protoflux example Updates Delay With Data.webp")

Updates Delay With Data being used in a code to keep a value from a [Source](https://wiki.resonite.com/ProtoFlux:Source "ProtoFlux:Source") till after the delay and using DelayedValue rather than using the [Source](https://wiki.resonite.com/ProtoFlux:Source "ProtoFlux:Source") directly after the delay.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:UpdatesDelayWithData&oldid=110949](https://wiki.resonite.com/index.php?title=ProtoFlux:UpdatesDelayWithData&oldid=110949)"

Contents