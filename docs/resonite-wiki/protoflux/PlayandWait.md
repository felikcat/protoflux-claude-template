# ProtoFlux:PlayandWait

> Source: https://wiki.resonite.com/ProtoFlux:PlayandWait

Play And Wait

\*

OnStarted

Target

OnPlaybackFinished

Media

PlayAndWait is a ProtoFlux node that plays the provided Target ( [IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable")) when \* ( [IAsyncOperation](https://wiki.resonite.com/Impulses "Impulses")) is called, and then can continue with an [Continuation](https://wiki.resonite.com/Impulses "Impulses").

## Inputs

### \\* ( [IAsyncOperation](https://wiki.resonite.com/Impulses "Impulses"))

Impulse this to play the provided Target ( [IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable"))

### Target ( [IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable"))

The [IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable") to play.

## Outputs

### OnStarted ( [AsyncCall](https://wiki.resonite.com/Impulses "Impulses"))

An async impulse that impulses when the target starts playing.

### OnPlaybackFinished ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Sends an impulse after the target finishes playback.

## Examples

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:PlayandWait&oldid=110455](https://wiki.resonite.com/index.php?title=ProtoFlux:PlayandWait&oldid=110455)"

Contents