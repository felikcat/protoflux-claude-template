# Resonite Components Overview

> Source: https://wiki.resonite.com/Category:Components

Components give slots functionality in Resonite. This is the complete category reference.

## Main Component Categories

| Category | Summary |
|----------|---------|
| **Assets** | Materials, Procedural Components, Meshes |
| **Audio** | Audio Output, Reverb Zones |
| **Cloud** | Cloud User Information, Server Status |
| **Common UI** | UIX/touchable button events, UI Drivers |
| **Data** | Dynamic Variables, item Metadata, value fields |
| **Debug** | Component Debugging |
| **Generators** | Procedural Generators |
| **Input** | Controls for Desktop, VR inputs, haptic interactions |
| **Interaction** | Grip Pose Reference |
| **Localization** | Translations |
| **Locomotion** | User Locomotions, Locomotion modifiers, Character Controller |
| **Media** | Audio clip player variations, Media Drivers |
| **Metadata** | Metadata about the object |
| **Network** | Twitch Interface, Websockets |
| **Misc** | Miscellaneous Components |
| **Permissions** | World Permissions |
| **Physics** | Colliders, Dynamic Bones |
| **ProtoFlux** | ProtoFlux related components |
| **Radiant UI** | Context Menus, Facets, General UI Elements |
| **Relations** | Multi-Drivers |
| **Rendering** | Render Providers, Animators, Text Rendering, Particles |
| **Tools** | Tools & brushes |
| **Transform** | Field drivers, Object Tagging, button interactions |
| **UI** | Mostly Legacy UI |
| **UIX** | Components for UIX, Resonite's UI System |
| **Users** | Basic Avatar & User systems |
| **Userspace** | Virtual Keyboard inputs |
| **Utility** | Value/Reference Multiplexer, Hyperlinks |
| **Wizards** | Asset/World optimization Wizards |
| **World** | World Based Components (WorldOrb, Thumbnail Source) |

## Hidden Components

These components are used internally by FrooxEngine and cannot be created normally.

## Custom Components

Can be added with plugins. GitHub Issue #3769 tracks ProtoFlux-based custom components.

---

## Essential Components Reference

### MeshRenderer

Renders static 3D meshes and applies materials.

| Field | Type | Description |
|-------|------|-------------|
| `Mesh` | Mesh | The mesh to render (StaticMesh or Procedural) |
| `Materials` | list of Material | Materials to apply to mesh |
| `ShadowCastMode` | ShadowCastMode | How object casts shadows |
| `SortingOrder` | Int | Render order relative to other renderers |

### BoxCollider

Simple box-shaped collider (second most performant after Sphere).

| Field | Type | Description |
|-------|------|-------------|
| `Offset` | Float3 | Offset from slot's position |
| `Type` | ColliderType | Collider behavior type |
| `Size` | Float3 | Local size in x, y, z |
| `CharacterCollider` | Bool | Prevents avatar from entering |
| `IgnoreRaycasts` | Bool | Prevents laser/raycast hits |

### Grabbable

Allows grabbing any slot with a Collider.

| Field | Type | Description |
|-------|------|-------------|
| `ReparentOnRelease` | Bool | Reparent to `_lastParent` on drop |
| `PreserveUserSpace` | Bool | Reparent to Local User Space |
| `DestroyOnRelease` | Bool | Destroy slot on release |
| `GrabPriority` | Int | Priority when multiple grabbables overlap |
| `Scalable` | Bool | Allow two-hand scaling |
| `AllowSteal` | Bool | Other users can grab from holder |
| `AllowOnlyPhysicalGrab` | Bool | Disable remote/laser grabs |

### PBS_Metallic

Physically-based material using Metallic-Smoothness workflow.

| Field | Type | Description |
|-------|------|-------------|
| `AlbedoColor` | ColorX | Base color tint (default white) |
| `AlbedoTexture` | ITexture2D | Base color texture |
| `EmissiveColor` | ColorX | Emission color tint |
| `NormalMap` | ITexture2D | Surface detail normals |
| `Metallic` | Float | Metalness if no MetallicMap |
| `Smoothness` | Float | Smoothness if no MetallicMap |
| `MetallicMap` | ITexture2D | R=Metallic, G=AO/Height, A=Smoothness |

---

## Transform Drivers (75 components)

Essential components for driving values and transforms.

### Value/Reference Drivers

| Component | Description |
|-----------|-------------|
| `ValueCopy<T>` | Drive target's value from source's value |
| `ReferenceCopy<T>` | Drive target's reference from source's reference |
| `BooleanValueDriver<T>` | Drive value based on boolean condition |
| `BooleanReferenceDriver<T>` | Drive reference based on boolean condition |
| `ValueEqualityDriver<T>` | Drive boolean based on value equality |
| `ReferenceEqualityDriver<T>` | Drive boolean based on reference equality |

### Transform Drivers

| Component | Description |
|-----------|-------------|
| `CopyGlobalTransform` | Copy position/rotation from another slot |
| `CopyGlobalScale` | Copy scale from another slot |
| `LookAt` | Make slot face another slot |
| `LookAtUser` | Make slot face a user |
| `AutoLookAtUser` | Make slot face closest user |
| `Spinner` | Rotate around axis at constant speed |
| `SmoothTransform` | Lerp to target position/rotation/scale |

### Layout Components

| Component | Description |
|-----------|-------------|
| `AxisAligner` | Arrange children in line along axis |
| `CircleAligner` | Arrange children in circle |
| `SphereAligner` | Arrange children on sphere surface |
| `ObjectGridAligner` | Arrange children in planar grid |

### Animation/Mapping

| Component | Description |
|-----------|-------------|
| `LinearMapper1D` | Map float to float linearly |
| `LinearMapper2D` | Map float to Float2 linearly |
| `LinearMapper3D` | Map float to Float3 linearly |
| `LinearColorMapper` | Map float to Color linearly |
| `Panner1D/2D/3D/4D` | Drive float/vector from 0 to amount at speed |
| `SmoothValue<T>` | Smooth value towards target |
| `ValueGradientDriver<T>` | Drive based on gradient position |

### User-Specific

| Component | Description |
|-----------|-------------|
| `ValueUserOverride<T>` | Different value per user |
| `ReferenceUserOverride<T>` | Different reference per user |
| `UserDistanceValueDriver<T>` | Drive based on user distance |
