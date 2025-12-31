# ProtoFlux:OnDuplicate

> Source: https://wiki.resonite.com/ProtoFlux:OnDuplicate

On Duplicate

Trigger

Events

On Duplicate is a ProtoFlux node that sends an impulse out of Trigger whenever the node is duplicated. This will fire on the duplicate of the code, and not the original copy.

Since this node may send an impulse before the rest of the protoflux is loaded, certain functions such as [Smooth Lerp](https://wiki.resonite.com/ProtoFlux:Value_Smooth_Lerp "ProtoFlux:Value Smooth Lerp") may not work as intended. If you have a use case relying on interpolation, consired adding a small [Delay](https://wiki.resonite.com/ProtoFlux:Delay "ProtoFlux:Delay"), or using the [On Start](https://wiki.resonite.com/ProtoFlux:On_Start "ProtoFlux:On Start") node instead.

## Outputs

### Trigger ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Sends an Impulse when the node is duplicated.

## Examples

- [On Duplicate being used to create a particle effect when an item is duplicated.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_On_Duplicate.webp "File:Protoflux example On Duplicate.webp")

On Duplicate being used to create a particle effect when an item is duplicated.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:OnDuplicate&oldid=110351](https://wiki.resonite.com/index.php?title=ProtoFlux:OnDuplicate&oldid=110351)"

Contents