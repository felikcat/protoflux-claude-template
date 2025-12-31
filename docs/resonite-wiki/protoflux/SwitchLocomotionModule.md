# ProtoFlux:SwitchLocomotionModule

> Source: https://wiki.resonite.com/ProtoFlux:SwitchLocomotionModule

Switch Locomotion Module

\*

OnSwitched

TargetUser

OnNotFound

ModuleName

ExactMatch

Locomotion

Switch Locomotion Module is a ProtoFlux node that switches a user to a locomotion by name.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Call this to switch the locomotion for the TargetUser ( [User](https://wiki.resonite.com/Type:User "Type:User")).

### TargetUser ( [User](https://wiki.resonite.com/Type:User "Type:User"))

The user to switch the locomotion they are using to walk when this node is triggered.

### ModuleName ( [String](https://wiki.resonite.com/Type:String "Type:String"))

the name of the locomotion slot that the user should switch to.

Ex: "Walk/Run (with climbing)", "Fly", "Noclip", "Teleport", (etc.)

### ExactMatch ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Whether to switch the lomotion if it is a partial match (false) or switch only if the name exactly matches (true).

## Outputs

### OnSwitched ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Sends an impulse after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) was called and a locomotion was successfully found and switched to.

### OnNotFound ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Sends an impulse after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) was called and the specified locomotion was not found.

## Examples

- [Using Switch Locomotion Module to add a climb avatar to the local user.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Switch_Locomotion_Module.webp "File:Protoflux example Switch Locomotion Module.webp")

Using Switch Locomotion Module to add a climb avatar to the local user.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:SwitchLocomotionModule&oldid=110789](https://wiki.resonite.com/index.php?title=ProtoFlux:SwitchLocomotionModule&oldid=110789)"

Contents