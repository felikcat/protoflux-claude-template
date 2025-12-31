# ProtoFlux:Construct Zita Parameters

> Source: https://wiki.resonite.com/ProtoFlux:Construct_Zita_Parameters

(Redirected from [ProtoFlux:Construct Zita Parameters](https://wiki.resonite.com/index.php?title=ProtoFlux:Construct_Zita_Parameters&redirect=no "ProtoFlux:Construct Zita Parameters"))

Construct Zita Parameters

InDelay

\*

Crossover

RT60Low

RT60Mid

HighFrequencyDamping

EQ1Frequency

EQ1Level

EQ2Frequency

EQ2Level

Mix

Level

Audio

The **Construct Zita Parameters** node creates [ZitaParameters](https://wiki.resonite.com/Type:ZitaParameters "Type:ZitaParameters") which are used make a reverberation sound effect parameter input object in the [Awwdio](https://wiki.resonite.com/Awwdio "Awwdio") system, for use in different reverberation sound effect methods like the one for [Static Audio Clips](https://wiki.resonite.com/Component:StaticAudioClip "Component:StaticAudioClip").

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you need a way to control reverb using [Components](https://wiki.resonite.com/Components "Components"), use [AudioZitaReverb](https://wiki.resonite.com/Component:AudioZitaReverb "Component:AudioZitaReverb") instead.


## Inputs

### InDelay ( [Float](https://wiki.resonite.com/Type:Float "Type:Float"))

The delay time before the reverb starts.

### Crossover ( [Float](https://wiki.resonite.com/Type:Float "Type:Float"))

How much the reverb "crosses over" or fades within itself.

### RT60Low ( [Float](https://wiki.resonite.com/Type:Float "Type:Float"))

RT60 refers to the Reverberation Time, which is the time it takes for the sound energy in a room to decay by 60 decibels after the sound source has stopped. (Low End)

### RT60Mid ( [Float](https://wiki.resonite.com/Type:Float "Type:Float"))

RT60 refers to the Reverberation Time, which is the time it takes for the sound energy in a room to decay by 60 decibels after the sound source has stopped. (Mid End)

### HighFrequencyDamping ( [Float](https://wiki.resonite.com/Type:Float "Type:Float"))

The high frequency dampening for the reverb.

### EQ1Frequency ( [Float](https://wiki.resonite.com/Type:Float "Type:Float"))

The equalizer frequency (1) of the reverb.

### EQ1Level ( [Float](https://wiki.resonite.com/Type:Float "Type:Float"))

The equalizer volume (1) of the reverb.

### EQ2Frequency ( [Float](https://wiki.resonite.com/Type:Float "Type:Float"))

The equalizer frequency (2) of the reverb.

### EQ2Level ( [Float](https://wiki.resonite.com/Type:Float "Type:Float"))

The equalizer volume (2) of the reverb.

### Mix ( [Float](https://wiki.resonite.com/Type:Float "Type:Float"))

The amount of audio to mix in the reverb.

### Level ( [Float](https://wiki.resonite.com/Type:Float "Type:Float"))

The overall level (or volume) of the reverb

## Outputs

### \\* ( [ZitaParameters](https://wiki.resonite.com/Type:ZitaParameters "Type:ZitaParameters"))

The constructed zita parameters.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ConstructZitaParameters&oldid=109565](https://wiki.resonite.com/index.php?title=ProtoFlux:ConstructZitaParameters&oldid=109565)"

Contents