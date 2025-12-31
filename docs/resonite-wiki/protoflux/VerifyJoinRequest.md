# ProtoFlux:VerifyJoinRequest

> Source: https://wiki.resonite.com/ProtoFlux:VerifyJoinRequest

Verify Join Request

Verify

UserID

UserSessionID

MachineID

Username

HeadOutputDevice

Platform

IsInvited

IsContact

IsInKioskMode

IsSpectatorBanned

IsMuteBanned

Handle

Security

The **Verify Join Request** node listens for join requests when [users](https://wiki.resonite.com/User "User") join a [world](https://wiki.resonite.com/World "World") with an enabled join verification system, firing an event when it happens. This node returns a set of information that contains info of the joining user. This node can be combined with the [Allow Join](https://wiki.resonite.com/ProtoFlux:Allow_Join "ProtoFlux:Allow Join"), [Deny Join](https://wiki.resonite.com/ProtoFlux:Deny_Join "ProtoFlux:Deny Join"), and [Assign Role](https://wiki.resonite.com/ProtoFlux:Assign_Role "ProtoFlux:Assign Role") nodes.

To activate a join verification system, a user needs to open the node in a [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector") and go to the [VerifyJoinRequest](https://wiki.resonite.com/index.php?title=Component:VerifyJoinRequest&action=edit&redlink=1 "Component:VerifyJoinRequest (page does not exist)") component. The bottom of the component has a button labeled "Set as custom join request verifier" and a warning letting users know that this feature does not prevent tampering of worlds that use this feature.

The following is the exact warning inside this node:

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

WARNING: At the moment, there is no mechanism to prevent tampering with the verifier once enabled. If tampering with the ProtoFlux setup for verification is a concern, DO NOT USE this feature and DO NOT ENABLE it in your worlds.


## Outputs

### Verify ( [AsyncCall](https://wiki.resonite.com/Impulses "Impulses"))

Fires when a user is wanting to join the world.

### UserID ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The user ID that is wanting to join the world.

### UserSessionID ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The user session ID that the user is coming from.

### MachineID ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The user machine ID that is wanting to join the world.

### Username ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The username that is wanting to join the world.

### HeadOutputDevice ( [HeadOutputDevice](https://wiki.resonite.com/Type:HeadOutputDevice "Type:HeadOutputDevice"))

The joining user's head output device.

### Platform ( [Platform](https://wiki.resonite.com/Type:Platform "Type:Platform"))

The joining user's platform.

### IsInvited ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Returns if this joining user was invited.

### IsContact ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Returns if this joining user is in the host's contacts list.

### IsInKioskMode ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Returns if this joining user is in kiosk mode.

### IsSpectatorBanned ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Returns if this joining user was banned as a spectator.

### IsMuteBanned ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Returns if this joining user was banned and muted.

### Handle ( [JoinRequestHandle](https://wiki.resonite.com/index.php?title=Type:JoinRequestHandle&action=edit&redlink=1 "Type:JoinRequestHandle (page does not exist)"))

Returns this join request as a type.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:VerifyJoinRequest&oldid=111089](https://wiki.resonite.com/index.php?title=ProtoFlux:VerifyJoinRequest&oldid=111089)"

Contents