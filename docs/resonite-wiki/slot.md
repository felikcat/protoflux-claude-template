# Slot

Every object in Resonite exists as a **Slot**. Slots form *hierarchies*, are positioned in 3D space via their *transformation*, and may contain components to add additional behavior.

## Basic Properties

### Hierarchy

A slot can contain zero or more slots, forming a **hierarchy** or "**tree**". A slot is a **child** if it is contained within another slot; that slot is its **parent**. The only slot without a parent is the **root** of the world, which contains all other slots.

This hierarchy is used for organization, transformation (see below), and many other features in Resonite.

### Transformation

Each slot has a 3D transformation consisting of translation, rotation, and scale. A child slot's transformation is specified in *local space*, i.e. relative to its parent slot's transformation, so even though a child may use the default transforms, it may be transformed in *world space* due to its parents' transforms.

### Components

Slots contain **components**, which provide almost all the functionality in Resonite. See the components documentation for details.

## Fields

| Field | Type | Description |
|-------|------|-------------|
| `Name` | string | The name of the component, as shown in the scene inspector. |
| `Parent` | Slot | A reference to the parent slot in the hierarchy. |
| `Tag` | string | A string Tag used for identifying slots in various systems. |
| `Active` | bool | A general-purpose field to "disable" this slot and its components. If a slot is deactivated, its children are deactivated too. Note that not all components and features respect this field. |
| `Persistent` | bool | Whether this slot will be saved, for example to the Inventory. If disabled, the slot and all its descendants will not be saved. |
| `Position` | float3 | This slot's position in local space. |
| `Rotation` | floatQ | This slot's rotation in local space. |
| `Scale` | float3 | This slot's scale in local space. Defaults to (1, 1, 1). |
| `OrderOffset` | long | Controls the sort order of this slot relative to its siblings. Slots with a higher value are processed after siblings with a lower value. |

## Working With Slots

### With the Scene Inspector

As a user, slots are primarily manipulated through the Scene Inspector. You can view, create, destroy and modify slots and their components.

### With ProtoFlux

ProtoFlux has a set of nodes for working with the slot hierarchy. See the ProtoFlux:Slots category for a list.

### Limitations

- There is no way to access a Slot's components with ProtoFlux directly.

## Other Features

### Slot Transferring

Slots can be moved across worlds via a feature called Transfer Grabbing by focusing to a different world while holding a slot.

Source: https://wiki.resonite.com/Slot
