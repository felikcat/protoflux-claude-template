# Scene Inspector

The **Scene Inspector** is used to navigate all objects (slots) in a world to view and edit properties. It lets you modify absolutely anything in your current world.

**Caution:** This includes things that could break world interaction. Be careful with unfamiliar things, especially on the root slot. You can always quit and return to reset; nothing breaks permanently unless you save changes.

## Basic Layout

### Left Pane

- Current root object slot name (prefixed with "Root: ")
- Scene hierarchy

#### Scene Hierarchy Navigation

| Action | How To |
|--------|--------|
| Select slot | Double-trigger-click |
| Re-parent slot | Drag with grip button, release on target |
| Open new inspector | Grab slot with grip, then press trigger |
| Reference in ProtoFlux | ProtoFlux tool + grab slot + context menu → "Reference" |
| Expand children | Click box with arrow |
| Collapse | Click downward arrow |
| Go up one level | Click root up button |
| Navigate to object root | Click object root button |
| Set current as visible root | Click set root button |

**Visual indicators:**
- Filled circle = no children
- Box with arrow = has children (expandable)
- Downward arrow = expanded
- Orange items = non-persistent (won't be saved)
- Yellow name = currently selected

### Right Pane

- Currently selected slot name (prefixed with "Slot: ")
- Destroy preserving assets button
- Insert parent button
- Slot properties
- Component list
- Attach Component button

## Slot Properties

| Property | Description |
|----------|-------------|
| **Name** | Slot name shown in hierarchy. Use Ø to null. |
| **Parent** | Parent slot reference. Ø sets to world root. |
| **Tag** | String variable assigned to every slot. Default null. |
| **Active** | Boolean for slot and children active state. Inactive slots are darker. |
| **Persistent** | Boolean for save behavior. Non-persistent = orange in hierarchy. |
| **Position** | float3 (x, y, z) relative to parent |
| **Rotation** | floatQ (euler x, y, z) relative to parent |
| **Scale** | float3 (x, y, z) relative to parent |
| **Order Offset** | Controls processing order among siblings |

**Coordinate Space:**
- X: +Right / -Left
- Y: +Up / -Down
- Z: +Forward / -Backward

### Slot Buttons

| Button | Function |
|--------|----------|
| Reset Position | Set to (0, 0, 0) |
| Reset Rotation | Set to (0, 0, 0) |
| Reset Scale | Set to (1, 1, 1) |
| Create Pivot At Center | Creates empty parent at bounding box center |
| Jump To | Teleport you to the selected item |
| Bring To | Teleport item to you |
| Parent Under Local User Space | Parent under your user's slot |
| Parent Under World Root | Parent under world root |

## Component List

Scrollable area displaying all components on selected slot.

All components have:
- Component name and type (e.g., `ValueCopy<int>`)
- Duplicate button
- Destroy button

**Moving/Duplicating:** Grab component header, move to another inspector → option to move or duplicate.

## Buttons

| Icon | Name | Use |
|------|------|-----|
| Destroy | Destroys slot and children |
| Destroy Preserving Assets | Destroys but keeps materials/meshes in Assets Slot |
| Insert Parent | Inserts empty parent, transfers transforms |
| Add Child | Adds empty child slot |
| Duplicate | Creates copy of selected slot |
| Set Root | Sets selected as hierarchy view root |
| Pin | Pins inspector to you (moves with you) |
| Close | Closes inspector |
| Object Root | Focuses on object root for selected slot |
| Root Up | Focuses on parent of current root |

## Advanced Features

1. **Field value transfer:** With Dev Tool equipped, grab field button and drop value onto another field name to copy values

2. **Reset list elements:** On list components, click and hold button, flick in any direction to reset element to default

3. **Numerical field options:** Press Primary on field button for context menu:
   - Set all members to one value
   - Set to average
   - Reset to default

Source: https://wiki.resonite.com/Scene_Inspector
