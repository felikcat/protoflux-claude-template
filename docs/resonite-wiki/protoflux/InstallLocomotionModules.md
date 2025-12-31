# ProtoFlux:InstallLocomotionModules

> Source: https://wiki.resonite.com/ProtoFlux:InstallLocomotionModules

Install Locomotion Modules

\*

Next

ModulesRoot

TargetUser

ClearExisting

Locomotion

Install Locomotion Modules is a ProtoFlux node that takes a slot with a type from the [ILocomotionModule](https://wiki.resonite.com/Type:ILocomotionModule "Type:ILocomotionModule") interface on it. The locomotion will also need a character controller and a few other components, which should be auto generated when a type from the [ILocomotionModule](https://wiki.resonite.com/Type:ILocomotionModule "Type:ILocomotionModule") interface component is added.

When called, this node will add the locomotion to the user in question.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Call this to install the locomotion(s) to the target user.

### ModulesRoot ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The module slot itself, or a slot with multiple locomotions under it to install to the target user. each slot to install needs a type from the [ILocomotionModule](https://wiki.resonite.com/Type:ILocomotionModule "Type:ILocomotionModule") interface on it.

### TargetUser ( [User](https://wiki.resonite.com/Type:User "Type:User"))

The user to install the provided ModulesRoot ( [Slot](https://wiki.resonite.com/Slot "Slot")) to.

### ClearExisting ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Removes all the existing locomotions from the user and replace with the provided ModulesRoot ( [Slot](https://wiki.resonite.com/Slot "Slot")) locomotion module(s).

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Sends an impulse after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) was called and the locomotion(s) are installed to the provided user.

## Examples

- [Using install locomotion modules to add a climb avatar to the local user.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Install_Locomotion_Modules.webp "File:Protoflux example Install Locomotion Modules.webp")

Using install locomotion modules to add a climb avatar to the local user.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:InstallLocomotionModules&oldid=110065](https://wiki.resonite.com/index.php?title=ProtoFlux:InstallLocomotionModules&oldid=110065)"

Contents