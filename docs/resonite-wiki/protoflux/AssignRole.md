# ProtoFlux:AssignRole

> Source: https://wiki.resonite.com/ProtoFlux:AssignRole

Assign Role

\*

Next

Handle

RoleName

Security

The **Assign Role** node takes in a [JoinRequestHandle](https://wiki.resonite.com/index.php?title=Type:JoinRequestHandle&action=edit&redlink=1 "Type:JoinRequestHandle (page does not exist)") and a role name, and if the [world](https://wiki.resonite.com/World "World") enabled a join verification system using the [Verify Join Request](https://wiki.resonite.com/ProtoFlux:Verify_Join_Request "ProtoFlux:Verify Join Request") node, this node will run and set the [user's](https://wiki.resonite.com/User "User") role in this world.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Calls an impulse to set the user's role in the world.

### Handle ( [JoinRequestHandle](https://wiki.resonite.com/index.php?title=Type:JoinRequestHandle&action=edit&redlink=1 "Type:JoinRequestHandle (page does not exist)"))

The handle for the join verification system.

### RoleName ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The role to set this user.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Continue the code from here.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:AssignRole&oldid=109277](https://wiki.resonite.com/index.php?title=ProtoFlux:AssignRole&oldid=109277)"

Contents