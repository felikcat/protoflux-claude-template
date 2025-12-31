# ProtoFlux:AnchorLocomotionData

> Source: https://wiki.resonite.com/ProtoFlux:AnchorLocomotionData

Anchor Locomotion Data

OnLocomotionUpdate

HasPrimary

HasSecondary

PrimaryAxis

SecondaryAxis

PrimaryAction

SecondaryAction

Anchor

null

∅

Anchors

Anchor Locomotion Data is a ProtoFlux node that checks the button presses for someone in an anchor and returns the values

The values for Anchor Locomotion Data outputs will all be default unless read during the OnLocomotionUpdate ( [Call](https://wiki.resonite.com/Impulses "Impulses")) impulse [context](https://wiki.resonite.com/Impulses#Contexts "Impulses").

## Outputs

### OnLocomotionUpdate ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

On locomotion update only fires if the user in the anchor is causing changes to any the outputs of this node compared to the previous value.

### HasPrimary ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Whether the user in the anchor has access to a joystick in their dominant hand

### HasSecondary ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Whether the user in the anchor has access to a joystick in their non dominant hand

### PrimaryAxis ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

The anchored user's joystick direction on the dominant hand.

### SecondaryAxis ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

The anchored user's joystick direction on the non dominant hand.

### PrimaryAction ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Whether the user in the anchor has pressed in their dominant hand joystick

### SecondaryAction ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Whether the user in the anchor has pressed in their non dominant hand joystick

## Globals

### Anchor ( [AvatarAnchor](https://wiki.resonite.com/Type:AvatarAnchor "Type:AvatarAnchor"))

The anchor to check for a user to check for events on.

## Examples

- [![Example of an Anchor Locomotion Data node having it's value read via multiple writes to Data Model Store](https://wiki.resonite.com/images/thumb/8/8f/Protoflux_example_Anchor_Locomotion_Data.png/455px-Protoflux_example_Anchor_Locomotion_Data.png)](https://wiki.resonite.com/File:Protoflux_example_Anchor_Locomotion_Data.png "Example of an Anchor Locomotion Data node having it's value read via multiple writes to Data Model Store")

Example of an Anchor Locomotion Data node having it's value read via multiple writes to [Data Model Store](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store")


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:AnchorLocomotionData&oldid=109253](https://wiki.resonite.com/index.php?title=ProtoFlux:AnchorLocomotionData&oldid=109253)"

Contents