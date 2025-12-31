# ProtoFlux:OnStart

> Source: https://wiki.resonite.com/ProtoFlux:OnStart

On Start

OnlyHost

Trigger

Events

The On Start ProtoFlux node triggers on the start of that instance of the node's existence for the local user.

To check if a user joined, use [User Joined](https://wiki.resonite.com/ProtoFlux:User_Joined "ProtoFlux:User Joined") instead of this node.

## Inputs

### OnlyHost ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

If enabled, Trigger will only fire for the host.

## Outputs

### Trigger ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Sends a pulse when the node starts, this can be triggered from the node being duplicated, the node being spawned, or a user joining the session.

## Examples

- [On Start being used to play a welcome message to the host when starting a world.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_On_Start.webp "File:Protoflux example On Start.webp")

On Start being used to play a welcome message to the host when starting a world.

- [On Start being used to play a generic welcome message to every new user of a world. This would be better done with a User Joined node.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_On_Start_2.webp "File:Protoflux example On Start 2.webp")

On Start being used to play a generic welcome message to every new user of a world. This would be better done with a [User Joined](https://wiki.resonite.com/ProtoFlux:User_Joined "ProtoFlux:User Joined") node.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:OnStart&oldid=110377](https://wiki.resonite.com/index.php?title=ProtoFlux:OnStart&oldid=110377)"

Contents