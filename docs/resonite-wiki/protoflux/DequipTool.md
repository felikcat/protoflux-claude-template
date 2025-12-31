# ProtoFlux:DequipTool

> Source: https://wiki.resonite.com/ProtoFlux:DequipTool

Dequip Tool

\*

OnDequipped

User

OnDequipFail

Side

PopOff

Tools

The `Dequip Tool` node makes a user take off a [tool](https://wiki.resonite.com/Tools "Tools") from their hand of a specific side of that user.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Calls an impulse to dequip the tool on one side of the user.

### User ( [User](https://wiki.resonite.com/User "User"))

The user to dequip the tool from.

### Side ( [Chirality](https://wiki.resonite.com/Type:Chirality "Type:Chirality"))

The side to dequip from.

### PopOff ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Should the tool pop off a certain distance from your hand.

## Outputs

### OnDequipped ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the tool is dequipped.

### OnDequipFail ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the tool failed to dequip in any way.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:DequipTool&oldid=109667](https://wiki.resonite.com/index.php?title=ProtoFlux:DequipTool&oldid=109667)"

Contents