# ProtoFlux:SampleValueAnimationTrack

> Source: https://wiki.resonite.com/ProtoFlux:SampleValueAnimationTrack

Sample Value Animation Track<T>

Animation

\*

TrackIndex

Time

Assets

This node when provided an [Animation Asset](https://wiki.resonite.com/Type:Animation "Type:Animation") sample the given track index for a [primitive](https://wiki.resonite.com/Value_Type "Value Type") value at the specified time.

## Inputs

### Animation ( [Animation Asset](https://wiki.resonite.com/Type:Animation "Type:Animation"))

The [Animation Asset](https://wiki.resonite.com/Type:Animation "Type:Animation") provided by an [IAssetProvider<Animation>](https://wiki.resonite.com/Type:IAssetProvider%601 "Type:IAssetProvider`1").

### TrackIndex ( [int](https://wiki.resonite.com/Types:Int "Types:Int"))

The track index of the given Animation ( [Animation Asset](https://wiki.resonite.com/Type:Animation "Type:Animation")) to sample from

### Time ( [Float](https://wiki.resonite.com/Types:Float "Types:Float"))

The time in seconds at which to sample the animation. If between keyframes it will sample based on the [AnimJ's](https://wiki.resonite.com/AnimJ "AnimJ") interpolation for those frames on the track.

## Outputs

### \\* (Dummy Pseudo-generic)

This gives the [Primitive](https://wiki.resonite.com/Value_Type "Value Type") for the track index given to TrackIndex ( [int](https://wiki.resonite.com/Types:Int "Types:Int")) at the time given to Time ( [Float](https://wiki.resonite.com/Types:Float "Types:Float")). If between keyframes it will sample based on the [AnimJ's](https://wiki.resonite.com/AnimJ "AnimJ") interpolation for those frames on the track.

## Examples

- [![Example of a find track index being used with a sample track index.](https://wiki.resonite.com/images/thumb/9/93/Animation_Track_Index_Example1.png/480px-Animation_Track_Index_Example1.png)](https://wiki.resonite.com/File:Animation_Track_Index_Example1.png "Example of a find track index being used with a sample track index.")

Example of a find track index being used with a sample track index.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:SampleValueAnimationTrack&oldid=110643](https://wiki.resonite.com/index.php?title=ProtoFlux:SampleValueAnimationTrack&oldid=110643)"

Contents