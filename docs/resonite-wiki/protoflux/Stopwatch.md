# ProtoFlux:Stopwatch

> Source: https://wiki.resonite.com/ProtoFlux:Stopwatch

Stopwatch

Start

OnStart

Stop

OnStop

Reset

OnReset

Time

IsRunning

Actions

The **Stopwatch** node keeps track of time when running. Akin to a [real stopwatch](https://en.wikipedia.org/wiki/Stopwatch), it allows one to start time, stop time, and reset time.

## Inputs

### Start ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Starts the stopwatch, putting it in the running state.

### Stop ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Stops the stopwatch, putting it in the stopped state.

### Reset ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Resets the stopwatch time. Does not affect the state of the stopwatch.

## Outputs

### OnStarted ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Sends an impulse when `Start` is impulsed. Is not affected by the state of the stopwatch.

### OnStopped ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Sends an impulse when `Stop` is impulsed. Is not affected by the state of the stopwatch.

### OnReset ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Sends an impulse when `Reset` is impulsed. Is not affected by the state of the stopwatch.

### Time ( [Float](https://wiki.resonite.com/Type:Float "Type:Float"))

The time in seconds stored by the stopwatch. This value increments when in the running state and freezes when in the stopped state. If `Reset` is pulsed, this output is set to `0`, but continues the same behavior of the state the watch is in.

Sometimes, it may be desirable to obtain a [TimeSpan](https://wiki.resonite.com/Type:TimeSpan "Type:TimeSpan") type from this value. To do so, use a [TimeSpan From Seconds](https://wiki.resonite.com/ProtoFlux:TimeSpan_From_Seconds "ProtoFlux:TimeSpan From Seconds") node.

### IsRunning ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

`True` if the stopwatch is in a running state, `False` otherwise.

## Examples

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:Stopwatch&oldid=103546](https://wiki.resonite.com/index.php?title=ProtoFlux:Stopwatch&oldid=103546)"

Contents