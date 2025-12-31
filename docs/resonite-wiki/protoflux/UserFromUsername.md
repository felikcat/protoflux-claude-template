# ProtoFlux:UserFromUsername

> Source: https://wiki.resonite.com/ProtoFlux:UserFromUsername

User From Username

Username

\*

IgnoreCase

AllowPartialMatch

Users

This node returns a [user](https://wiki.resonite.com/Type:User "Type:User") object from a username.

This will only work for [users](https://wiki.resonite.com/Type:User "Type:User") present in the session.

## Inputs

### Username ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The username of the user you need.

### IgnoreCase ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Ignore case. For instance, using `FrOoXiUs` would still match `Frooxius`.

### AllowPartialMatch ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Allow for partial matches. For instance, using `Froox` as an input would still match `Frooxius`.

## Outputs

### \\* ( [User](https://wiki.resonite.com/Type:User "Type:User"))

A [user](https://wiki.resonite.com/Type:User "Type:User") object that satisfies this node's input requirements.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:UserFromUsername&oldid=110975](https://wiki.resonite.com/index.php?title=ProtoFlux:UserFromUsername&oldid=110975)"

Contents