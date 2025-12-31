# ProtoFlux:PlayOneShot

> Source: https://wiki.resonite.com/ProtoFlux:PlayOneShot

Play One Shot

\*

OnStartedPlaying

Clip

Audio

Volume

Speed

Spatialize

SpatialBlend

Point

Root

ParentUnderRoot

Priority

Doppler

MinDistance

MaxDistance

Rolloff

DistanceSpace

MinScale

MaxScale

Group

LocalOnly

Audio

Play One Shot is a ProtoFlux node that creates a new audio source under the provided Root ( [Slot](https://wiki.resonite.com/Slot "Slot")) (except when ParentUnderRoot ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool")) is enabled) with the provided parameters. Play One Shot is under Audio in the Protoflux Node creation menu

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Play the audio clip with the provided parameters

### Clip ( [IAssetProvider\`1](https://wiki.resonite.com/Type:IAssetProvider%601 "Type:IAssetProvider`1") < [AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip") >)

The audio clip to play on the newly created sound object

### Volume ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The volume to play the audio at.

### Speed ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The speed to play the audio at.

### Spatialize ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Whether the audio played will have spatialization.

### SpatialBlend ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

How spatialized the audio played will be.

### Point ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The point to play the audio if Root ( [Slot](https://wiki.resonite.com/Slot "Slot")) is not provided.

### Root ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot to play the audio under. The audio will not be audible if the slot is part of a disabled hierarchy. If nothing is filled in for this input, the sound will come from the node itself.

### ParentUnderRoot ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Whether to put the audio under the root of the world or not.

### Priority ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

How much priority this audio clip has, which can override others when the buffer is too full. So this audio has more priority to be played in such cases.

### Doppler ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Whether the audio clip played should have Doppler. [What is Doppler?](https://en.wikipedia.org/wiki/Doppler_effect)

### MinDistance ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The distance the audio stops becoming louder when getting closer to the source.

### MaxDistance ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The max distance the audio can be heard from until it is inaudible

### Rolloff ( [AudioRolloffMode](https://wiki.resonite.com/Type:AudioRolloffMode "Type:AudioRolloffMode"))

The [AudioRolloffMode](https://wiki.resonite.com/Type:AudioRolloffMode "Type:AudioRolloffMode") the audio created should use.

### DistanceSpace ( [AudioDistanceSpace](https://wiki.resonite.com/Type:AudioDistanceSpace "Type:AudioDistanceSpace"))

The [AudioDistanceSpace](https://wiki.resonite.com/Type:AudioDistanceSpace "Type:AudioDistanceSpace") the audio created should use.

### MinScale ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

See [Min and Max Scale section on audio output component page.](https://wiki.resonite.com/Component:AudioOutput#Min_and_Max_Scale "Component:AudioOutput")

### MaxScale ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

See [Min and Max Scale section on audio output component page.](https://wiki.resonite.com/Component:AudioOutput#Min_and_Max_Scale "Component:AudioOutput")

### Group ( [AudioTypeGroup](https://wiki.resonite.com/Type:AudioTypeGroup "Type:AudioTypeGroup"))

What [AudioTypeGroup](https://wiki.resonite.com/Type:AudioTypeGroup "Type:AudioTypeGroup") this node is in.

### LocalOnly ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Whether this audio should only play locally for the user that fired the node.

## Outputs

### OnStartedPlaying ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

When the audio clip has successfully started playing

### Audio ( [AudioOutput](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput"))

The [Audio Output](https://wiki.resonite.com/Component:AudioOutput "Component:AudioOutput") component created to play the audio. The [Get Slot](https://wiki.resonite.com/ProtoFlux:Get_Slot "ProtoFlux:Get Slot") node can be used to get the created slot for the one shot. This will only have a value during the OnStartedPlaying ( [Continuation](https://wiki.resonite.com/Impulses "Impulses")) impulse.

## Examples

- [Example of a Play One Shot being used in a random funny meme item.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Play_One_Shot.webp "File:Protoflux example Play One Shot.webp")

Example of a Play One Shot being used in a random funny meme item.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:PlayOneShot&oldid=110451](https://wiki.resonite.com/index.php?title=ProtoFlux:PlayOneShot&oldid=110451)"

Contents