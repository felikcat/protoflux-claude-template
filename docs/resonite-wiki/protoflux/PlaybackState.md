# ProtoFlux:PlaybackState

> Source: https://wiki.resonite.com/ProtoFlux:PlaybackState

Playback State

Target

IsPlaying

Loop

Position

NormalizedPosition

ClipLength

Speed

Media

PlayBack State is a ProtoFlux node that provides information of a ( [IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable")). This can be used to get information of if the a source is playing, the current time position, and the length of the audio source.

## Inputs

### Source ( [IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable"))

The [IPlayable](https://wiki.resonite.com/Type:IPlayable "Type:IPlayable") to provide information from.

## Outputs

### IsPlaying ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Tells if the source is playing.

### Loop ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Tells if the source is set to loop.

### Position ( [Float](https://wiki.resonite.com/Type:Float "Type:Float"))

The playing position of the current target in seconds as a float.

### NormalizedPosition ( [Float](https://wiki.resonite.com/Type:Float "Type:Float"))

The playing position of the current target remapped to a float minimum of 0 and maximum of 1.
This essentially [remaps](https://wiki.resonite.com/ProtoFlux:Remap "ProtoFlux:Remap") the song length to 0 being the start and 1 being the end.

### ClipLength ( [Float](https://wiki.resonite.com/Type:Float "Type:Float"))

The target length in seconds, as a float.

### Speed ( [Float](https://wiki.resonite.com/Type:Float "Type:Float"))

The target current playing speed. 1 is equivalent to x1.0.

## Examples

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:PlaybackState&oldid=110459](https://wiki.resonite.com/index.php?title=ProtoFlux:PlaybackState&oldid=110459)"

Contents