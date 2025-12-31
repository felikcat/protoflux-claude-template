# ProtoFlux:SampleColorX

> Source: https://wiki.resonite.com/ProtoFlux:SampleColorX

Sample ColorX

\*

OnSampleStart

Point

OnSampled

Direction

SampledColor

Reference

NearClip

FarClip

Rendering

The `Sample ColorX` node takes in the point and direction, along with the bounds of the a near and far clip to sample a color. This node will attempt to return a color that was found and sampled.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Calls an impulse to begin sampling the color with the provided parameters.

### Point ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

Where should this node start in 3D space when sampling the color.

### Direction ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

Which direction should this node look when sampling the color.

### Reference ( [Slot](https://wiki.resonite.com/Slot "Slot"))

...

### NearClip ( [float](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

How close this node should check for sampling the color.

### FarClip ( [float](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

How far this node should check for sampling the color.

## Outputs

### OnSampleStart ( [AsyncCall](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the sampling has started.

### OnSampled ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the color has been sampled.

### SampledColor ( [colorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))

Returns the sampled color.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:SampleColorX&oldid=110629](https://wiki.resonite.com/index.php?title=ProtoFlux:SampleColorX&oldid=110629)"

Contents