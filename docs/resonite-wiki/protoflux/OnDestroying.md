# ProtoFlux:OnDestroying

> Source: https://wiki.resonite.com/ProtoFlux:OnDestroying

On Destroying

Trigger

Events

The **On Destroying** node sends an impulse out of Trigger whenever the node is marked for destruction. This will not preserve [Async](https://wiki.resonite.com/Impulses#ASync "Impulses") tasks, as since those create delays they will be destroyed before execution of the task finishes.

## Outputs

### Trigger ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Sends an Impulse when the node is marked for destruction which may include all the rest of the code, but nothing is destroyed yet.

## Examples

- [On Destroying being used to activate a large bit of code without any async tasks that makes an effect.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_On_Destroying.webp "File:Protoflux example On Destroying.webp")

On Destroying being used to activate a large bit of code without any async tasks that makes an effect.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:OnDestroying&oldid=110349](https://wiki.resonite.com/index.php?title=ProtoFlux:OnDestroying&oldid=110349)"

Contents