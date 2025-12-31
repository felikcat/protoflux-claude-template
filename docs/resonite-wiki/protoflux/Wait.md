# ProtoFlux:Wait

> Source: https://wiki.resonite.com/ProtoFlux:Wait

Wait

\*

OnWaitBegin

Target

OnPlaybackFinished

Media

Wait is a ProtoFlux node that waits for the provided Target ( [IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable")) to complete playback, and then provides a continuation.

## Inputs

### \\* ( [IAsyncOperation](https://wiki.resonite.com/Impulses "Impulses"))

### Target ( [IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable"))

The [IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable") to wait for.

## Outputs

### OnWaitBegin ( [AsyncCall](https://wiki.resonite.com/Impulses "Impulses"))

An async impulse that impulses when the node starts waiting.

### OnPlaybackFinished ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Sends an impulse after the target finishes playback.

## Examples

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:Wait&oldid=82790](https://wiki.resonite.com/index.php?title=ProtoFlux:Wait&oldid=82790)"

Contents