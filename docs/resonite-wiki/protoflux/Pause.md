# ProtoFlux:Pause

> Source: https://wiki.resonite.com/ProtoFlux:Pause

Pause

\*

Next

Target

Media

Pause is a ProtoFlux node that pauses the provided Target ( [IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable")) when \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) is called.
Pause doesn't change the current [Position Output](https://wiki.resonite.com/ProtoFlux:Position "ProtoFlux:Position"), it essentially sets [Is Playing Output](https://wiki.resonite.com/ProtoFlux:Is_Playing "ProtoFlux:Is Playing") to false.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Impulse this to pause the provided Target ( [IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable"))

### Target ( [IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable"))

The [IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable") to pause.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Sends an impulse after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) was called and it was successfully paused.

## Examples

- [A simple setup that allows control of the playback of an audio clip utilizing this node along with some others.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ProtoFlux_example_simple_audio_playback.webp "File:ProtoFlux example simple audio playback.webp")

A simple setup that allows control of the playback of an audio clip utilizing this node along with some others.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:Pause&oldid=75107](https://wiki.resonite.com/index.php?title=ProtoFlux:Pause&oldid=75107)"

Contents