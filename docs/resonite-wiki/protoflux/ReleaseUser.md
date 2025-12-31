# ProtoFlux:ReleaseUser

> Source: https://wiki.resonite.com/ProtoFlux:ReleaseUser

Release User

\*

OnReleased

Anchor

OnFailure

Anchors

Release User Is a ProtoFlux node that releases the user currently occupying an anchor.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Call this to release the [user](https://wiki.resonite.com/Type:User "Type:User") in the provided Anchor ( [IAvatarAnchor](https://wiki.resonite.com/Type:IAvatarAnchor "Type:IAvatarAnchor")).

### Anchor ( [IAvatarAnchor](https://wiki.resonite.com/Type:IAvatarAnchor "Type:IAvatarAnchor"))

The anchor to check for if a user is sitting in it.

## Outputs

### OnReleased ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

When the [user](https://wiki.resonite.com/Type:User "Type:User") in the provided anchor is released.

### OnFailure ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

When the provided Anchor ( [IAvatarAnchor](https://wiki.resonite.com/Type:IAvatarAnchor "Type:IAvatarAnchor")) doesn't have a [user](https://wiki.resonite.com/Type:User "Type:User") and the \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) is fired, this will send an impulse.

## Examples

- [Example of an Release User node being used in some code.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Release_User.webp "File:Protoflux example Release User.webp")

Example of an Release User node being used in some code.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ReleaseUser&oldid=110589](https://wiki.resonite.com/index.php?title=ProtoFlux:ReleaseUser&oldid=110589)"

Contents