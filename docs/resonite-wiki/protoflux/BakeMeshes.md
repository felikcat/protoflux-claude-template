# ProtoFlux:BakeMeshes

> Source: https://wiki.resonite.com/ProtoFlux:BakeMeshes

Bake Meshes

\*

OnBakeStarted

Root

OnBaked

SkinnedMeshMode

BakedRoot

IncludeInactive

DestroyOriginal

AssetsSlot

GrabbableHandling

ColliderHandling

Undoable

Assets

Bake Meshes is a ProtoFlux node that takes a slot and combines it's meshes and slots into one slot. Allowing for the optimization of content and allowing for packing together objects. For example, many avatar statue makers use this to create statues out of people's avatars with no functionalities. It's a way to make a statue of your favorite contact on your shelf withouut having to have their 10000 ProtoFlux nodes still on it.

[Avatar Protections](https://wiki.resonite.com/Component:SimpleAvatarProtection "Component:SimpleAvatarProtection") in the hierarchy of any slot you try to bake using this node will cause the bake to fail unless the Local User of the \* ( [AsyncCall](https://wiki.resonite.com/Impulses#ASync "Impulses")) Async call is coming from the user that the avatar protections is assigned to. In the case of avatar protections assigned to different users under the entire hiearchy, the bake will fail regardless. Because if one user tries to bake their protections, the other user's protections will prevent the node from working.

## Inputs

### \\* ( [AsyncCall](https://wiki.resonite.com/Impulses\#ASync "Impulses"))

Call this to start the bake.

### Root ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot to bake all of it's content for.

### SkinnedMeshMode ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

### IncludeInactive ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Include meshes and objects that currently aren't visible in the final product.

### DestroyOriginal ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Whether to destroy the Root ( [Slot](https://wiki.resonite.com/Slot "Slot")) when baked. Bad idea with baking statues for players.

### AssetsSlot ( [Slot](https://wiki.resonite.com/Slot "Slot"))

Where to put the assets?

### GrabbableHandling ( [ComponentHandling](https://wiki.resonite.com/Type:ComponentHandling "Type:ComponentHandling"))

What to do with [grabbable](https://wiki.resonite.com/Component:Grabbable "Component:Grabbable") components under what you're baking.

### ColliderHandling ( [ComponentHandling](https://wiki.resonite.com/Type:ComponentHandling "Type:ComponentHandling"))

What to do with [Colliders](https://wiki.resonite.com/Collider "Collider") under what you're baking.

### Undoable ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Weither the action can be undone via the undo keybind of the user that triggered the node.

## Outputs

### OnBakeStarted ( [AsyncCall](https://wiki.resonite.com/Impulses "Impulses"))

Called immediately after \* ( [AsyncCall](https://wiki.resonite.com/Impulses "Impulses")) is called and the bake successfully started.

### OnBaked ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires some time after \* ( [AsyncCall](https://wiki.resonite.com/Impulses "Impulses")) is called and the bake successfully finished.

### BakedRoot ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The result of the bake and all of it's contents will be under this slot minus assets. This will only have a value during the OnBaked ( [Continuation](https://wiki.resonite.com/Impulses "Impulses")) impulse.

## Examples

- [Using Bake Meshes to bake someone's avatar but not delete them.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ProtoFlux_examples_Bake_Meshes.webp "File:ProtoFlux examples Bake Meshes.webp")

Using Bake Meshes to bake someone's avatar but not delete them.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:BakeMeshes&oldid=109309](https://wiki.resonite.com/index.php?title=ProtoFlux:BakeMeshes&oldid=109309)"

Contents