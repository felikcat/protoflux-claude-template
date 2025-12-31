# ProtoFlux:UserLeft

> Source: https://wiki.resonite.com/ProtoFlux:UserLeft

User Left

OnlyHost

OnLeft

LeftUser

World

The `User Left` node is an event that fires when a user leaves the current world this node is in, as well as providing that user.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

Even though this will provide the user, it will only last for as long as this fired, only giving you enough time to check references, clean up anything, and using any of the data therein before the user fully leaves the world. After that point, that user, their references, and their data wont match to anything going forward past this point.


## Inputs

### OnlyHost ( [bool](https://wiki.resonite.com/Types:Bool "Types:Bool"))

Should this impulse only run on the host. (Default: true) Will run an impulse for all users when set to false.

## Outputs

### OnLeft ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Fires when a user leaves the world.

### LeftUser ( [User](https://wiki.resonite.com/User "User"))

The User that left the world.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:UserLeft&oldid=110981](https://wiki.resonite.com/index.php?title=ProtoFlux:UserLeft&oldid=110981)"

Contents