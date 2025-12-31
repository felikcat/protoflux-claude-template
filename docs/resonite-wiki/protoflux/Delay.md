# ProtoFlux:Delay

> Source: https://wiki.resonite.com/ProtoFlux:Delay

Delay

\*

Next

Duration

OnTriggered

Flow

Delay is a ProtoFlux node that allows for delaying an [Async](https://wiki.resonite.com/Impulses#Async "Impulses") execution for the provided Duration (Pseudo-generic) before continuing.

## Inputs

### \\* ( [AsyncCall](https://wiki.resonite.com/Impulses\#Async "Impulses"))

Start the delay.

### Duration (Pseudo-generic)

How long to delay for in seconds or timespan.

Examples: [Double](https://wiki.resonite.com/Type:Double "Type:Double"), [Float](https://wiki.resonite.com/Type:Float "Type:Float"), [Int](https://wiki.resonite.com/Type:Int "Type:Int") and [TimeSpan](https://wiki.resonite.com/Type:TimeSpan "Type:TimeSpan").

![](https://wiki.resonite.com/images/b/b7/DangerIcon.svg)

Delays of less than 0.5 milliseconds will be rounded to zero and may cause Resonite to hang if used inside of a loop.


## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires on the next game tick once the given duration has passed since the Delay was triggered **and** _OnTriggered_ has finished. If _OnTriggered_ takes longer than the delay duration to finish, _Next_ will be executed immediately after.

### OnTriggered ( [AsyncCall](https://wiki.resonite.com/Impulses\#Async "Impulses"))

Fires immediately after the Delay is triggered. This impulse chain will block _Next_, e.g. if it contains another Delay with a higher duration.

## Examples

- [![A "Useless Machine" that resets itself a second after pressing the Async Call Input. Note that every click will cause a delayed impulse that will reset the state. This may be unwanted if the goal is to reset a second after the last press.](https://wiki.resonite.com/images/thumb/5/51/Protoflux_example_Delay.webp/480px-Protoflux_example_Delay.webp.png)](https://wiki.resonite.com/File:Protoflux_example_Delay.webp "A \"Useless Machine\" that resets itself a second after pressing the Async Call Input. Note that every click will cause a delayed impulse that will reset the state. This may be unwanted if the goal is to reset a second after the last press.")

A ["Useless Machine"](https://en.wikipedia.org/wiki/Useless_machine "wikipedia:Useless machine") that resets itself a second after pressing the [Async Call Input](https://wiki.resonite.com/ProtoFlux:Async_Call_Input "ProtoFlux:Async Call Input"). Note that every click will cause a delayed impulse that will reset the state. This may be unwanted if the goal is to reset a second after the last press.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:Delay&oldid=92966](https://wiki.resonite.com/index.php?title=ProtoFlux:Delay&oldid=92966)"

Contents