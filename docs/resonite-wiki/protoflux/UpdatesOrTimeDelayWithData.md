# ProtoFlux:UpdatesOrTimeDelayWithData

> Source: https://wiki.resonite.com/ProtoFlux:UpdatesOrTimeDelayWithData

Updates Or Time Delay With Data

\*

Next

Updates

OnTriggered

Value

DelayedValue

Duration

Async

Updates Or Time Delay With Data is a ProtoFlux node that will send an impulse out of Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses")) after a delay. It will use Updates ( [int](https://wiki.resonite.com/Type:Int "Type:Int")) updates if provided or Duration (Pseudo-generic) time if provided. It will start the delay after \* ( [ASync Call](https://wiki.resonite.com/Impulses#ASync "Impulses")) is impulsed. It will carry a value and keep it during the duration of the delay and spit it out after the delay.

TODO: Which time takes priority?

## Inputs

### \\* ( [ASync Call](https://wiki.resonite.com/Impulses\#ASync "Impulses"))

Call to start the delay.

### Updates ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

How many updates to delay for if provided.

### Value (Generic)

The value to delay. Can be any type.

### Duration (Pseudo-generic)

How long to delay for as a time rather than updates if provided.

If a value other than a [TimeSpan](https://wiki.resonite.com/Type:TimeSpan "Type:TimeSpan") is provided, this value will delay it in seconds.

Examples: [Float](https://wiki.resonite.com/Type:Float "Type:Float"), [Double](https://wiki.resonite.com/Type:Double "Type:Double"), [Int](https://wiki.resonite.com/Type:Int "Type:Int"), [TimeSpan](https://wiki.resonite.com/Type:TimeSpan "Type:TimeSpan").

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires after Updates ( [int](https://wiki.resonite.com/Type:Int "Type:Int")) updates has passed or Duration (Pseudo-generic) time after an impulse has been sent to \* ( [ASync Call](https://wiki.resonite.com/Impulses#ASync "Impulses")).

### OnTriggered ( [ASync Call](https://wiki.resonite.com/Impulses\#ASync "Impulses"))

fires immediately after \* ( [ASync Call](https://wiki.resonite.com/Impulses#ASync "Impulses")) is called.

### DelayedValue (Generic)

Has a value during the Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses")) impulse and outputs the value that was provided to Value (Generic) when \* ( [ASync Call](https://wiki.resonite.com/Impulses#ASync "Impulses")) was impulsed.

## Examples

- [Updates Delay With Data being used in a code to keep a value from a Source till after the delay and using DelayedValue rather than using the Source directly after the delay.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Updates_Delay_With_Data.webp "File:Protoflux example Updates Delay With Data.webp")

Updates Delay With Data being used in a code to keep a value from a [Source](https://wiki.resonite.com/ProtoFlux:Source "ProtoFlux:Source") till after the delay and using DelayedValue rather than using the [Source](https://wiki.resonite.com/ProtoFlux:Source "ProtoFlux:Source") directly after the delay.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:UpdatesOrTimeDelayWithData&oldid=110953](https://wiki.resonite.com/index.php?title=ProtoFlux:UpdatesOrTimeDelayWithData&oldid=110953)"

Contents