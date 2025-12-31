# ProtoFlux:BakeReflectionProbes

> Source: https://wiki.resonite.com/ProtoFlux:BakeReflectionProbes

Bake Reflection Probes

\*

OnBakeBatchStart

Root

OnBeforeProbeBake

BakeInactive

OnProbeBaked

FilterWithTag

OnBakeBatchFinished

DelayBeforeBake

Probe

ProbeIndex

ProbeCount

Rendering

The `Bake Reflection Probes` node takes in the root slot holding all your reflection probes, whether or not to bake the inactive reflection probes, the matching tag to bake only those reflection probes, and a delay before starting the baking process. This node will then attempt to bake them all, then returns the focused reflection probe, the index of that reflection probe, and the count of all reflection probes.

## Inputs

### \\* ( [AsyncCall](https://wiki.resonite.com/Impulses "Impulses"))

Calls an impulse to bake all reflection probes with matching parameters.

### Root ( [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot"))

The slot hierarchy that holds the reflection probes.

### BakeInactive ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Should be able to bake reflection probs that are not enabled.

### FilterWithTag ( [string](https://wiki.resonite.com/Type:String "Type:String"))

Bakes the reflection probes that match this tag.

### DelayBeforeBake ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

Should wait a certain amount of time before actually beginning the bake.

## Outputs

### OnBakeBatchStart ( [AsyncCall](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the bake has started.

### OnBeforeProbeBake ( [AsyncCall](https://wiki.resonite.com/Impulses "Impulses"))

Fires before the probe is being baked.

### OnProbeBaked ( [AsyncCall](https://wiki.resonite.com/Impulses "Impulses"))

Fires after the probe has been baked.

### OnBakeBatchFinished ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the batch of probes have finished baking.

### Probe ( [ReflectionProbe](https://wiki.resonite.com/index.php?title=Type:ReflectionProbe&action=edit&redlink=1 "Type:ReflectionProbe (page does not exist)"))

The current probe being baked.

### ProbeIndex ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The index number showing which probe is being baked.

### ProbeCount ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The number of probes in this batch.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:BakeReflectionProbes&oldid=109313](https://wiki.resonite.com/index.php?title=ProtoFlux:BakeReflectionProbes&oldid=109313)"

Contents