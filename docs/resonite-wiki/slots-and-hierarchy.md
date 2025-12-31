# Slots and Hierarchy

> Source: https://wiki.resonite.com/Slot

Every object in Resonite exists as a **Slot**. Slots form hierarchies, are positioned in 3D space via transformation, and contain Components for functionality.

## Basic Properties

### Hierarchy

- Slots contain zero or more child slots, forming a tree
- A slot inside another is a **child**; the containing slot is its **parent**
- Only the world **root** has no parent
- Hierarchy is used for organization, transformation, and many features

### Transformation

Each slot has 3D transformation:
- **Position** (translation)
- **Rotation**
- **Scale**

Child transformations are in **local space** (relative to parent). Even with default transforms, a child may be transformed in world space due to parent transforms.

### Components

Slots contain **components** which provide almost all Resonite functionality.

## Slot Fields

| Field | Type | Description |
|-------|------|-------------|
| `Name` | String | Display name in scene inspector |
| `Parent` | Slot | Reference to parent slot |
| `Tag` | String | String tag for identification |
| `Active` | Bool | "Disable" slot and children (not all features respect this) |
| `Persistent` | Bool | Whether slot saves (to Inventory, etc.) |
| `Position` | Float3 | Local space position |
| `Rotation` | FloatQ | Local space rotation (quaternion) |
| `Scale` | Float3 | Local space scale (default 1,1,1) |
| `OrderOffset` | Long | Sort order relative to siblings |

## Working With Slots

### Scene Inspector

Primary tool for manipulating slots - view, create, destroy, modify slots and components.

### ProtoFlux Nodes

Category `ProtoFlux:Slots` contains slot manipulation nodes:
- `GetSlot` - Get slot from component
- `GetSlotName` - Get slot's name
- `SetSlotActive` - Enable/disable slot
- `DuplicateSlot` - Clone a slot
- `DestroySlot` - Remove a slot
- `FindChild` / `FindParent` - Navigate hierarchy
- `GetParent` / `GetChild` - Direct hierarchy access

### Limitations

- No way to access a Slot's components directly with ProtoFlux (Issue #57)

## Slot Transferring

Slots can be moved across worlds via **Transfer Grabbing** - focus to different world while holding a slot.

## ProtoGraph Slot Usage

```protograph
// Get slot from component/input
in TargetSlot: Slot

// Access slot's transform
Position = TargetSlot->GlobalTransform.GlobalPosition;
Rotation = TargetSlot->GlobalTransform.GlobalRotation;
Scale = TargetSlot->GlobalTransform.GlobalScale;

// Set local scale (requires impulse)
switch SomeEvent
| OnTriggered |> impulse {
    SetLocalScale(Instance=TargetSlot, Scale=Pack_Float3(X=1.0f, Y=2.0f, Z=1.0f));
};

// Get slot name
Name = TargetSlot->GetSlotName;

// Check if slot is active
IsActive = TargetSlot->GetSlotActiveSelf;
```

## Common Slot Components

| Component | Purpose |
|-----------|---------|
| `Grabbable` | Allow grabbing the slot |
| `BoxCollider` | Physical collision box |
| `MeshRenderer` | Render a 3D mesh |
| `PBS_Metallic` | PBR material |
| `DynamicVariableSpace` | Define dynamic variable scope |
