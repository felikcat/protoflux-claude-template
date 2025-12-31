# ProtoFlux:PlaybackDrive

> Source: https://wiki.resonite.com/ProtoFlux:PlaybackDrive

Playback Drive

StartDrive

OnStartDrive

StopDrive

OnStopDrive

ForceResync

OnResync

Target

IsDriving

NormalizedPosition

MaximumPositionError

Speed

Play

Loop

Media

Playback Drive is a node that will take a [SyncPlayback](https://wiki.resonite.com/Type:SyncPlayback "Type:SyncPlayback") and allow you to start or stop driving it to a set of provided playback settings and values. The driving of the SyncPlayback is non networked.

## Inputs

### StartDrive ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Starts driving the Target ( [SyncPlayback](https://wiki.resonite.com/Type:SyncPlayback "Type:SyncPlayback")) in a non networked fashion, which essentially makes the provided Target ( [SyncPlayback](https://wiki.resonite.com/Type:SyncPlayback "Type:SyncPlayback")) no longer synced until StopDrive ( [Call](https://wiki.resonite.com/Impulses "Impulses")) is called.

### StopDrive ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Stop driving the Target ( [SyncPlayback](https://wiki.resonite.com/Type:SyncPlayback "Type:SyncPlayback")), making it networked again.

### ForceResync ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

When this is impulsed, The node will try to sync the current Target ( [SyncPlayback](https://wiki.resonite.com/Type:SyncPlayback "Type:SyncPlayback")) position that the local user sees with everyone else in a session. (See [Impulses](https://wiki.resonite.com/Impulses "Impulses") for what a local user on an Impulse means) If this is called and NormalizedPosition ( [float](https://wiki.resonite.com/Type:Float "Type:Float")) does not have an input, it will do nothing.

### Target ( [SyncPlayback](https://wiki.resonite.com/Type:SyncPlayback "Type:SyncPlayback"))

The Network Synced Playable that will become un-networked via being driven by this node.

### NormalizedPosition ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The position to drive Target ( [SyncPlayback](https://wiki.resonite.com/Type:SyncPlayback "Type:SyncPlayback")) to from 0 to 1.

### Maximum Position Error ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The the max amount the position on Target ( [SyncPlayback](https://wiki.resonite.com/Type:SyncPlayback "Type:SyncPlayback")) can vary from NormalizedPosition ( [float](https://wiki.resonite.com/Type:Float "Type:Float")).

### Speed ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The a multiplier for the playback speed of Target ( [SyncPlayback](https://wiki.resonite.com/Type:SyncPlayback "Type:SyncPlayback")).

### Play ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

If the Target ( [SyncPlayback](https://wiki.resonite.com/Type:SyncPlayback "Type:SyncPlayback")) should be playing. (default true if normalized position is given and moving)

### Loop ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

If the Target ( [SyncPlayback](https://wiki.resonite.com/Type:SyncPlayback "Type:SyncPlayback")) should loop. May clash when providing NormalizedPosition ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

## Outputs

### OnStartDrive ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

When StartDrive ( [Call](https://wiki.resonite.com/Impulses "Impulses")) is impulsed and it can drive Target ( [SyncPlayback](https://wiki.resonite.com/Type:SyncPlayback "Type:SyncPlayback"))

### OnStopDrive ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

When StopDrive ( [Call](https://wiki.resonite.com/Impulses "Impulses")) is impulsed and this node was driving Target ( [SyncPlayback](https://wiki.resonite.com/Type:SyncPlayback "Type:SyncPlayback"))

### OnResync ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

sends an impulse when ForceResync ( [Call](https://wiki.resonite.com/Impulses "Impulses")) succeeds.

### IsDriving ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

If the Target ( [SyncPlayback](https://wiki.resonite.com/Type:SyncPlayback "Type:SyncPlayback")) is currently driving. (Aka StartDrive ( [Call](https://wiki.resonite.com/Impulses "Impulses")) was called but not StopDrive ( [Call](https://wiki.resonite.com/Impulses "Impulses")) yet.)

## Examples

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:PlaybackDrive&oldid=110457](https://wiki.resonite.com/index.php?title=ProtoFlux:PlaybackDrive&oldid=110457)"

Contents