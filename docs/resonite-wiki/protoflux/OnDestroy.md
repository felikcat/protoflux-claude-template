# ProtoFlux:OnDestroy

> Source: https://wiki.resonite.com/ProtoFlux:OnDestroy

On Destroy

OnlyHost

Trigger

Events

The **On Destroy** node sends an impulse out of Trigger whenever the node is destroyed.
This can sometimes not fire code the way you want, since the code after the node may have already been destroyed. It is better practice to use [On Destroying](https://wiki.resonite.com/ProtoFlux:On_Destroying "ProtoFlux:On Destroying").

## Inputs

### OnlyHost ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Checks the event on the host rather than on everyone.

## Outputs

### Trigger ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Sends an Impulse when the node is destroyed.

## Examples

- [On Destroy being used to activate just one node after it like a dynamic impulse.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_On_Destroy.webp "File:Protoflux example On Destroy.webp")

On Destroy being used to activate just one node after it like a [dynamic impulse](https://wiki.resonite.com/Dynamic_Impulses "Dynamic Impulses").


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:OnDestroy&oldid=110347](https://wiki.resonite.com/index.php?title=ProtoFlux:OnDestroy&oldid=110347)"

Contents