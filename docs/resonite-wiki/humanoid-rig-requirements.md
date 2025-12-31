# Humanoid Rig Requirements for IK

When you import a rigged model to turn it into an avatar, this guide helps you understand the requirements.

## Supported Formats

If you have a rigged model compatible with other VR Platforms (VRChat, etc.), it should work out of the box.

**We do NOT support importing:**
- `.unitypackage`
- `.vrm`
- `.asset`
- `.mesh`
- `.prefab`

**Supported Humanoid Avatar formats:**
- FBX
- GLTF
- Blender

## Overall Rig/Model Requirements

### Definitions

- **Segment** - A single bone within a Rig (e.g., a finger with 3 bones has 3 segments)
- **IK** - Inverse Kinematics, the system used to pose your Rig in Resonite

### General Guidance

- Model should be in **A-pose or T-Pose**
- Orientation (forward facing) should be along **positive Z axis**
- Flipped Z axis can be detected but might contain bugs

**Quick validation:** Check "Force T-pose" in advanced import settings:
- Hands crossed → rotate 180° along Z axis
- One hand front/one back → rotate 90° along Z axis

### Ignoring Bones

Add `<NoIK>` (case insensitive) anywhere in bone name to exclude from IK:

| Bone Name | Used in IK? |
|-----------|-------------|
| Right Hand | ✅ |
| `<NoIK>` Right Hand | ❌ |
| Right Hand `<NoIK>` | ❌ |
| Right Hand `<noik>` | ❌ |

Useful for twist bones or clothing/hair bones detected as skeletal bones.

## Bone Requirements

Resonite uses pattern matching and heuristics for bone detection. Names are:
- Case insensitive ("hips", "Hips", "HIPS" all work)
- Forgiving of spaces ("upper arm" = "upperarm")
- Can have additional data ("cheese_hips" detected as hips)

### Central Spine/Hips

Root of armature should be a single hips bone facing upwards.

| Order | Part | Alternative Names | Invalid Names ❌ |
|-------|------|-------------------|------------------|
| 1st | Hips | hips, pelvis, root | hip |
| 2nd | Spine | spine, chest | |
| 3rd | Chest | chest, upper chest, ribcage, spine1, spine2 | |
| 4th | Neck | neck | |
| 5th | Head | head | skull |

**Upper Chests:** Extra bone segments (Spine2/Upper Chest) are supported but not required.

### Shoulders and Arms

Two arms attached to "Chest" bone. Use "L" and "R" for sides (case insensitive).

| Order | Part | Alternative Names | Invalid Names ❌ |
|-------|------|-------------------|------------------|
| 1st | Shoulder | shoulder, clavicle, collar, collarbone | |
| 2nd | Upper Arm | upperarm, upper arm, arm, bicep | forearm |
| 3rd | Lower Arm | fore arm, forearm, lower arm, lowerarm, elbow | |
| 4th | Hand | hand, wrist, palm | |

### Hands

**Finger requirements:**
- Each finger **must have** at least 2 segments
- Support up to 4 segments: Metacarpal, Proximal, Intermediate, Distal
- Need **at least 3 fingers** to identify a hand
- Need an identifiable **thumb**

With 5 fingers, geometric detection figures out bone names automatically.

**Finger naming pattern:** `<fingername>1 -> <fingername>2 -> <fingername>3 -> <fingername>4`

| Finger # | Name | Alternative Names |
|----------|------|-------------------|
| 1 | Thumb | |
| 2 | Index | point |
| 3 | Middle | |
| 4 | Ring | |
| 5 | Pinky | little |

### Legs

Each leg connected to Hip bone. Use "L" and "R" for sides.

| Order | Part | Alternative Names |
|-------|------|-------------------|
| 1st | Upper Leg | upper leg, upleg, thigh, upperleg, hipL, hipR |
| 2nd | Lower Leg | leg, calf, knee, shin |
| 3rd | Foot | foot, ankle |
| 4th | Toes | toe, toes, ball, toebase |

**Digitigrade Legs:** Not natively supported. Community workaround: Use `CopyGlobalTransform` component to copy dummy plantigrade leg movements onto digitigrade legs.

### Heads

#### Eyes

For automatic eye movements and eye tracking:

| Part | Compatible Names |
|------|------------------|
| Left Eye | LeftEye, Left Eye, Eye.L, Eye_L |
| Right Eye | RightEye, Right Eye, Eye.R, Eye_R |

#### Jaws

Name jaw bone "Jaw" (case insensitive) for jaw-based animations.

## Supported Tools

- **Mixamo** generated rigs work without changes
- **Ready Player Me** avatars work without changes

Source: https://wiki.resonite.com/Humanoid_rig_requirements_for_IK
