# ProtoFlux:UserSpawn

> Source: https://wiki.resonite.com/ProtoFlux:UserSpawn

User Spawn

OnlyHost

OnSpawn

SpawnedUser

World

The `User Spawn` node is an event that fires when a user spawns/respawns in the current world this node is in, as well as providing that user.

Spawn events can happen when a user either gets removed or deleted from the hierarchy, using the respawn button in the session menu, or using a gadget to respawn a user.

![](https://wiki.resonite.com/images/d/dd/InformationIcon.svg)

When a user joins, this node will also fire due to them spawning in the world for the first time.


## Inputs

### OnlyHost ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Fires events for user spawns only for the host of the session.

## Outputs

### OnSpawn ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Fires when a user spawned in the world.

### SpawnedUser ( [User](https://wiki.resonite.com/User "User"))

The User that spawned in this world.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:UserSpawn&oldid=111005](https://wiki.resonite.com/index.php?title=ProtoFlux:UserSpawn&oldid=111005)"

Contents