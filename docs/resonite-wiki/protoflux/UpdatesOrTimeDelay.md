# ProtoFlux:UpdatesOrTimeDelay

> Source: https://wiki.resonite.com/ProtoFlux:UpdatesOrTimeDelay

Updates or Time Delay

\*

Next

Updates

OnTriggered

Duration

Async

Updates or Time Delay is a ProtoFlux node that will send an impulse out of Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses")) after a delay. It will use Updates ( [int](https://wiki.resonite.com/Type:Int "Type:Int")) updates or Duration (Pseudo-generic) time, whichever comes first. It will start the delay after \* ( [Async Call](https://wiki.resonite.com/Impulses#Async "Impulses")) is impulsed.

## Inputs

### \\* ( [Async Call](https://wiki.resonite.com/Impulses\#Async "Impulses"))

Call to start the delay.

### Updates ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

How many updates to delay for.

### Duration (Pseudo-generic)

How long to delay for as a time.

If a value other than a [TimeSpan](https://wiki.resonite.com/Type:TimeSpan "Type:TimeSpan") is provided, this value will delay it in seconds.

Examples: [Float](https://wiki.resonite.com/Type:Float "Type:Float"), [Double](https://wiki.resonite.com/Type:Double "Type:Double"), [Int](https://wiki.resonite.com/Type:Int "Type:Int"), [TimeSpan](https://wiki.resonite.com/Type:TimeSpan "Type:TimeSpan").

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires after Updates ( [int](https://wiki.resonite.com/Type:Int "Type:Int")) updates or Duration (Pseudo-generic) time has passed after an impulse has been sent to \* ( [Async Call](https://wiki.resonite.com/Impulses#Async "Impulses")).

### OnTriggered ( [Async Call](https://wiki.resonite.com/Impulses\#Async "Impulses"))

fires immediately after \* ( [Async Call](https://wiki.resonite.com/Impulses#Async "Impulses")) is called.

## Examples

- [Updates Or Time Delay being used in a code to reset a value for a visual after a button being pressed and x time passing.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Updates_Or_Time_Delay.webp "File:Protoflux example Updates Or Time Delay.webp")

Updates Or Time Delay being used in a code to reset a value for a visual after a button being pressed and x time passing.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:UpdatesOrTimeDelay&oldid=113140](https://wiki.resonite.com/index.php?title=ProtoFlux:UpdatesOrTimeDelay&oldid=113140)"

Contents