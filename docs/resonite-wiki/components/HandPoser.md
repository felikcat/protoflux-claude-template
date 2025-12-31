# Component:HandPoser

> Source: https://wiki.resonite.com/Component:HandPoser

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/7/7b/HandPoser.png/510px-HandPoser.png)](https://wiki.resonite.com/File:HandPoser.png) **Hand Poser** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

This component modifies the rotation of the fingers of an avatar's hand based on a pose source.
The HandPoser works with whatever data is avilable, either precise finger tracking like a LeapMotion, or course grained like a vive wand, where grip and trigger affect the main finger positions.

The HandPoser is made of five duplicate finger objects, each of which contains four duplicate bone objects. Each bone object contains a Coordinate Compensation, Root, OrigionalRotation, and RotationDrive.
The below chart is difficult to read for this reason, but read it as: the same four fields, duplicated four times (one for each bone), duplicated five times (one for each finger).

Due to this pattern, the intermediate bone of the thumb should never be bound as a human thumb does not have an intermediate bone.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `PoseSource` | **[IFingerPoseSourceComponent](https://wiki.resonite.com/Type:IFingerPoseSourceComponent "Type:IFingerPoseSourceComponent")** | What the finger transform data is derived from. |
| `Side` | **[Chirality](https://wiki.resonite.com/Type:Chirality "Type:Chirality")** | Which hand this poser is representing |
| `PoseMetacarpals` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | If metacarpals should be posed (this should normally be left as True) |
| `HandRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of the hand (if null the slot the component is attached to is used) |
| `HandForward` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | A unit vector pointing forward from the wrist to the fingers. |
| `HandUp` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | A unit vector pointing from the back of the hand outwards (alternatively phrased, this is pointing into the palm) |
| `HandRight` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | A unit vector pointing to the right of the hand, if the hand is facing down. This is roughly the direction of the thumb on the left hand, and the other side of the hand from the thumb on the right hand. |
| `Thumb` | _direct_ **[HandPoser.Finger](https://wiki.resonite.com/Component:HandPoser#Finger)** | The Thumb on an anthro hand. |
| `Index` | _direct_ **[HandPoser.Finger](https://wiki.resonite.com/Component:HandPoser#Finger)** | The Index on an anthro hand. |
| `Middle` | _direct_ **[HandPoser.Finger](https://wiki.resonite.com/Component:HandPoser#Finger)** | The Middle on an anthro hand. |
| `Ring` | _direct_ **[HandPoser.Finger](https://wiki.resonite.com/Component:HandPoser#Finger)** | The Ring on an anthro hand. |
| `Pinky` | _direct_ **[HandPoser.Finger](https://wiki.resonite.com/Component:HandPoser#Finger)** | The Pinky on an anthro hand. |
| `DebugFingers` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to show visuals for debugging the fingers. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnAssignFromRig:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Assigns the hand bones based on a parent [Rig](https://wiki.resonite.com/Component:Rig "Component:Rig") component. |
| `OnInitializeHand:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Sets up the default rotations and coordinate compensations for the fingers currently in this component from its current pose. |

Triggers
Collapse

## Finger

| Name | Type | Description |
| --- | --- | --- |
| `Metacarpal` | _direct_ **[FingerSegment](https://wiki.resonite.com/Component:HandPoser#FingerSegment)** | Usually inside of the palm and not actually inside the finger itself. |
| `Proximal` | _direct_ **[FingerSegment](https://wiki.resonite.com/Component:HandPoser#FingerSegment)** | The first finger segment of 3. |
| `Intermediate` | _direct_ **[FingerSegment](https://wiki.resonite.com/Component:HandPoser#FingerSegment)** | The second finger segment of 3. |
| `Distal` | _direct_ **[FingerSegment](https://wiki.resonite.com/Component:HandPoser#FingerSegment)** | The third finger segment of 3. |

Fields

## FingerSegment

| Name | Type | Description |
| --- | --- | --- |
| `CoordinateCompensation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The amount the bone is offset from the expected finger rotation by Resonite. |
| `Root` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot representing this bone. Note that a hand has no thumb intermediate bone. This is filled when the hand does have this finger segment. |
| `OriginalRotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The resting rotation of the finger bone. |
| `RotationDrive` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The Rotation field of the slot `Slot` of this finger segement. Used to move the finger. |

Fields

## Usage

This component forcibly assigns the rotation of each bound finger to a particular bone relative to the palm.
As an example of this, if you only assign a Distal bone, that bone will spin 270 degrees starting pointing forwards, curling to point out the direction of the palm, back towards the wrist, then pointing out the back of the hand.

It is often easiest to make changes to this component following this procedure:

1. Have the avatar be unequipped
2. Clear every RotationDrive field
3. Assign the Root field of each bone in the hand to be driven, this list will not be complete and some roots will be null.
4. Press InitializeHand at the bottom of the component (Note: This button only works once, to reset the button select another slot, then select the slot with the component again).
5. Re-Equip the avatar and see if the hands initialized successfully.
6. If a bone did not bind correctly, repeat.

## Interaction with grabbable items

### Precision grabbing

The HandPoser component is used as a source for determining how to grab items when using the "Precision" grabbing mode.

Precision grabbing selects the object which is closest to the midpoint between your index and your thumb. For this to work, your HandPoser needs to define at least one segment for these two fingers, otherwise grabbing simply will not work in this mode.

### Tools

The HandPoser component is also used as a source for determining the position of equipped [tools](https://wiki.resonite.com/Tools "Tools").

When grabbing or equipping a tool which defines a [GripPoseReference](https://wiki.resonite.com/Component:GripPoseReference "Component:GripPoseReference") without a set TipReference, the initial location from which the grip pose is applied is interpolated based on the location of the fingers and the HandRoot configured in the HandPoser.

For avatars with commonly-shaped hands with at least three fingers, this interpolated pose is usually close enough to allow using the majority of community-made tools without having to adjust the tool’s grip pose by too much.

## Examples

A few common problems can occur with an avatar's hands, here are common solutions.

### Fingertips Through the Palm

Some avatars have very long fingertips (distal bones), but the human hand is structured to have very short fingertips. For these avatars if the hand is fully closed the fingertips (or clawtips) may poke through the back of the avatars hands. To resolve this

One known fix for this is to follow the steps outlined in Behavior, but assign every Distal bone to the Intermediate slot (leaving the Indermediate unbound). This will result in the distal bones curling down to lay flat against the palm, instead of curling all theway through the hand.

### Hook Index Finger

This is where the rest of the hand bones accept the index finger bend at the base of the palm, instead of the knuckle. The index finger metacarpal doesn't bend at all though, leading to a 'hooked' appearance when the hand is closed.

[![](https://wiki.resonite.com/images/thumb/8/89/Hook_Index_Finger_Example_1.png/300px-Hook_Index_Finger_Example_1.png)](https://wiki.resonite.com/File:Hook_Index_Finger_Example_1.png)

There are two main fixes here, if the avatar isn't fully imported then re-import with the thumb parented to the palm bone instead of the index metacarpal.
Otherwise do the following:

1. Reparent the thumb metacarpal to the palm in the inspector (This may not be needed, investigation is needed).
2. Reassign the root fields for the entire hand following the procedure outlined in Behavior, the bindings will be incorrect.

### Extra Finger Spread

Some avatars may end up with much more splayed fingers when inhabited by a user, the current proposed solution is to not bind the metacarpal bones (More investigation is needed into this solution).

### Hand curls to look like cat claws

The first digit of the finger isn't curling when the hand is closed, making the hand look like a cat claw.

[![](https://wiki.resonite.com/images/3/3a/HandPoserComponent-CatClawHandCurl.jpg)](https://wiki.resonite.com/File:HandPoserComponent-CatClawHandCurl.jpg)

This is caused by the avatar's hand having more bones than Resonite expects, and the first bone in the hand is bound to the metacarpal, it needs to be bound to proximal instead, moving each corresponding bone one position down the finger.
The thumb is likely not affected by this.

### Most grabbable tools have bad positioning

Depending on the configuration of your HandPoser, it may be possible that most default and community-made tools have GripPoseReferences that cause the tool to be positioned at an awkward location in or around your hand. This can especially be the case if your avatar has no fingers, or only one "nub" in guise of an index or middle finger.

If that is the case, you can define empty slots to serve as a false HandRoot and false fingers. By assigning them in the HandPoser and placing them in appropriate locations around your hand, you can influence the default interpolated position of grabbed tools and fix this issue for most tools.

## See Also

- [Component:AvatarHandDataAssigner](https://wiki.resonite.com/Component:AvatarHandDataAssigner "Component:AvatarHandDataAssigner")
- [Finger Posing System](https://wiki.resonite.com/Finger_Posing_System "Finger Posing System")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:HandPoser&oldid=112334](https://wiki.resonite.com/index.php?title=Component:HandPoser&oldid=112334)"

Contents