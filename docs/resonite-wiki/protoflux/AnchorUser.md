# ProtoFlux:AnchorUser

> Source: https://wiki.resonite.com/ProtoFlux:AnchorUser

Anchor User

\*

OnAnchored

Anchor

OnFail

User

Anchors

Anchor User is a ProtoFlux node that attempts to anchor a user to any anchor, which is provided to the node via the [IAvatarAnchor](https://wiki.resonite.com/Type:IAvatarAnchor "Type:IAvatarAnchor") type.

If the anchor succeeds, it doesn't nessarily mean the user has stayed in the anchor, and requires checking [Anchored User Node](https://wiki.resonite.com/ProtoFlux:Anchored_User "ProtoFlux:Anchored User") A few updates later.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Anchors the User ( [User](https://wiki.resonite.com/Type:User "Type:User")) Upon impulse to the provided Anchor ( [IAvatarAnchor](https://wiki.resonite.com/Type:IAvatarAnchor "Type:IAvatarAnchor"))

### Anchor ( [IAvatarAnchor](https://wiki.resonite.com/Type:IAvatarAnchor "Type:IAvatarAnchor"))

The anchor to put the provided User ( [User](https://wiki.resonite.com/Type:User "Type:User")) into.

### User ( [User](https://wiki.resonite.com/Type:User "Type:User"))

The user to put into the provided Anchor ( [IAvatarAnchor](https://wiki.resonite.com/Type:IAvatarAnchor "Type:IAvatarAnchor")).

## Outputs

### OnAnchored ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Sends an impulse after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) is called and the user was sucessfully anchored.

### OnFail ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Sends an impulse after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) is called and the user was not anchored because the user currently is in another anchor, the provided anchor was null, or the provided anchor already had someone seated in it.

## Examples

- [![Example of how to anchor the user who pressed a button to a chair, which is seen behind the code.](https://wiki.resonite.com/images/thumb/1/14/Protoflux_example_anchor_user.jpg/480px-Protoflux_example_anchor_user.jpg)](https://wiki.resonite.com/File:Protoflux_example_anchor_user.jpg "Example of how to anchor the user who pressed a button to a chair, which is seen behind the code.")

Example of how to anchor the user who pressed a button to a chair, which is seen behind the code.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:AnchorUser&oldid=109255](https://wiki.resonite.com/index.php?title=ProtoFlux:AnchorUser&oldid=109255)"

Contents