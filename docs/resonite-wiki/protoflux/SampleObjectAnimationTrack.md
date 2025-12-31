# ProtoFlux:SampleObjectAnimationTrack

> Source: https://wiki.resonite.com/ProtoFlux:SampleObjectAnimationTrack

Sample Object Animation Track< T>

Animation

\*

TrackIndex

Time

Assets

This node when provided an [Animation Asset](https://wiki.resonite.com/Type:Animation "Type:Animation") sample the given track index for a [Reference Type](https://wiki.resonite.com/Category:Type "Category:Type") Reference at the specified time.

It is currently only possible to make use of this node to read [Strings](https://wiki.resonite.com/Type:String "Type:String") from [AnimJs](https://wiki.resonite.com/AnimJ "AnimJ"). This can be useful to store large amounts or string data, like translations or subtitles driven via animations.

## Inputs

### Animation ( [Animation Asset](https://wiki.resonite.com/Type:Animation "Type:Animation"))

The [Animation Asset](https://wiki.resonite.com/Type:Animation "Type:Animation") provided by an [IAssetProvider<Animation>](https://wiki.resonite.com/Type:IAssetProvider%601 "Type:IAssetProvider`1").

### TrackIndex ( [int](https://wiki.resonite.com/Types:Int "Types:Int"))

The track index of the given Animation ( [Animation Asset](https://wiki.resonite.com/Type:Animation "Type:Animation")) to sample from

### Time ( [Float](https://wiki.resonite.com/Types:Float "Types:Float"))

The time in seconds at which to sample the animation.

## Outputs

### \\* (Dummy Pseudo-generic)

This gives the [Reference Type](https://wiki.resonite.com/Category:Type "Category:Type") for the track index given to TrackIndex ( [int](https://wiki.resonite.com/Types:Int "Types:Int")) at the time given to Time ( [Float](https://wiki.resonite.com/Types:Float "Types:Float")).

This does not have interpolation\[Citation needed\]

## Examples

- [Example of a Sample Object Animation Track<Slot> being used to change the parent of a slot](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_sample_object_animation_track.webp "File:Protoflux sample object animation track.webp")

Example of a Sample Object Animation Track<Slot> being used to change the parent of a slot


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:SampleObjectAnimationTrack&oldid=110635](https://wiki.resonite.com/index.php?title=ProtoFlux:SampleObjectAnimationTrack&oldid=110635)"

Contents