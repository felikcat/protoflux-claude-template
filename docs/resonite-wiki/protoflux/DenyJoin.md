# ProtoFlux:DenyJoin

> Source: https://wiki.resonite.com/ProtoFlux:DenyJoin

Deny Join

\*

Next

Handle

DenyReason

Security

The **Deny Join** node takes in a [JoinRequestHandle](https://wiki.resonite.com/index.php?title=Type:JoinRequestHandle&action=edit&redlink=1 "Type:JoinRequestHandle (page does not exist)") and a deny reason, and if the [world](https://wiki.resonite.com/World "World") enabled a join verification system using the [Verify Join Request](https://wiki.resonite.com/ProtoFlux:Verify_Join_Request "ProtoFlux:Verify Join Request") node, this node will run and deny the [user](https://wiki.resonite.com/User "User") from joining and gives them a reason why.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Calls an impulse to deny the user from joining the world.

### Handle ( [JoinRequestHandle](https://wiki.resonite.com/index.php?title=Type:JoinRequestHandle&action=edit&redlink=1 "Type:JoinRequestHandle (page does not exist)"))

The handle for the join verification system.

### DenyReason ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The reason why a user is not allowed to join.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Continue the code from here.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:DenyJoin&oldid=109665](https://wiki.resonite.com/index.php?title=ProtoFlux:DenyJoin&oldid=109665)"

Contents