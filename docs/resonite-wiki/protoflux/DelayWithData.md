# ProtoFlux:DelayWithData

> Source: https://wiki.resonite.com/ProtoFlux:DelayWithData

Time Delay with Data

\*

Next

Value

OnTriggered

Duration

DelayedValue

Flow

Delay With Data is a ProtoFlux node that allows for delaying an [Async](https://wiki.resonite.com/Impulses#Async "Impulses") execution for the provided Duration (Pseudo-generic) before continuing. It will also carry over a Value (Generic) during the delay and output it to DelayedValue (Generic) when Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses")) fires.

## Inputs

### \\* ( [AsyncCall](https://wiki.resonite.com/Impulses\#Async "Impulses"))

Start the delay.

### Value (Generic)

The value to delay for Duration (Pseudo-generic) time.

### Duration (Pseudo-generic)

How long to delay for in seconds or timespan.

Examples: [Double](https://wiki.resonite.com/Type:Double "Type:Double"), [Float](https://wiki.resonite.com/Type:Float "Type:Float"), [Int](https://wiki.resonite.com/Type:Int "Type:Int") and [TimeSpan](https://wiki.resonite.com/Type:TimeSpan "Type:TimeSpan").

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires after Duration (Pseudo-generic) time has passed after \* ( [AsyncCall](https://wiki.resonite.com/Impulses#Async "Impulses")) was called. DelayedValue (Generic) during this impulse will have the value of what was put into Value (Generic) when \* ( [AsyncCall](https://wiki.resonite.com/Impulses#Async "Impulses")) was called.

### OnTriggered ( [SyncResumption](https://wiki.resonite.com/Impulses\#Async "Impulses"))

Fires instantly after \* ( [AsyncCall](https://wiki.resonite.com/Impulses#Async "Impulses")) is called.

### DelayedValue (Generic)

this will have the value of what was put into Value (Generic) when \* ( [AsyncCall](https://wiki.resonite.com/Impulses#Async "Impulses")) was called during the Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses")) impulse.

## Examples

- [![Delay With Data being used as a way to display where the user was 5 seconds ago](https://wiki.resonite.com/images/thumb/2/25/Protoflux_example_Delay_With_Data.webp/480px-Protoflux_example_Delay_With_Data.webp.png)](https://wiki.resonite.com/File:Protoflux_example_Delay_With_Data.webp "Delay With Data being used as a way to display where the user was 5 seconds ago")

Delay With Data being used as a way to display where the user was 5 seconds ago


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:DelayWithData&oldid=109655](https://wiki.resonite.com/index.php?title=ProtoFlux:DelayWithData&oldid=109655)"

Contents