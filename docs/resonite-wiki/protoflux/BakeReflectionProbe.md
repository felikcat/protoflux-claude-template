# ProtoFlux:BakeReflectionProbe

> Source: https://wiki.resonite.com/ProtoFlux:BakeReflectionProbe

Bake Reflection Probe

\*

OnBackStart

Probe

OnBakeFail

OnBakeComplete

BakedCubemapURL

Rendering

The `Bake Reflection Probe` node takes in a [Reflection Probe](https://wiki.resonite.com/index.php?title=Type:ReflectionProbe&action=edit&redlink=1 "Type:ReflectionProbe (page does not exist)") and begins the baking process, then returns the [Uri](https://wiki.resonite.com/Type:Uri "Type:Uri") asset that can be used for the world when completed.

## Inputs

### \\* ( [AysncCall](https://wiki.resonite.com/Impulses "Impulses"))

Calls an impulse to bake the reflection probe.

### Probe ( [ReflectionProbe](https://wiki.resonite.com/index.php?title=Type:ReflectionProbe&action=edit&redlink=1 "Type:ReflectionProbe (page does not exist)"))

The reflection probe to bake.

## Outputs

### OnBakeStart ( [AysncCall](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the bake has started.

### OnBakeFail ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the bake has failed.

### OnBakeComplete ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the bake has completed.

### BakedCubemapURL ( [Uri](https://wiki.resonite.com/Type:Uri "Type:Uri"))

Returns the baked asset URL.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:BakeReflectionProbe&oldid=109311](https://wiki.resonite.com/index.php?title=ProtoFlux:BakeReflectionProbe&oldid=109311)"

Contents