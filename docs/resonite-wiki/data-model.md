# Data Model

The **data model** refers to the declaration, structure, and handling of types, data, and changes on data within FrooxEngine. It allows for:
- Change detection
- Value synchronization
- Unified structure
- Serialization of all types

## Elements

Everything managed by the data model implements the `IWorldElement` interface, which provides:
- A reference ID
- Possible parent element
- Whether the element is persistent

Since all types implementing this interface have a reference ID, every element is itself a reference type.

Three types of elements directly implement this interface:
- **Sync elements**
- **Workers**
- **Worlds**

## Sync Elements

Sync elements represent a value or object that can be:
- Written to
- Linked
- Send/receive change events

Mainly comprise of fields and collections—usually any type name starting with `Sync` derives from a sync element.

### Synchronization

When a sync element changes (with few exceptions like RawOutput<T>):
- It and its entire parent hierarchy propagate a change event
- Elements get put in the world's update manager
- Values synchronize at end of update loop

### Linkage

Two types of linkage exist:

| Type | Inspector Color | Description |
|------|-----------------|-------------|
| **Link** | Cyan | Can only be changed by driver; sends data model events normally |
| **Drive** | Purple | Like link, but value NOT synchronized across network; allows per-user values |

## Workers

Workers are containers for sync elements and other workers to provide specific tasks. Examples:
- Slots
- Components
- Sub-classes of components
- Streams

Workers can:
- Receive events from children
- Propagate events to parent
- Are local constructs but usually exist in sync element collections

## Events

A big part of the data model is capturing and propagating changes across elements.

**Example:** A Changeable Source node referencing a slot plugged into Get Slot Active:
- Updates connected listener nodes when slot's active state changes
- This works because it receives events from the data model

**Contrast:** An Input node will NOT update listeners the same way (doesn't receive data model events).

## World

The heart of the data model is a world. The world update loop controls:
- Communication between all data model concepts
- UpdateManager - manages "dirty" sync elements and their changes
- LinkManager - manages all linkage within a world

## Strict Exclusivity

The data model only works when everyone in a session agrees on what it should be.

If one client tells another about an unknown element or worker type:
- Recipient won't know what to do with the information
- Won't know how to sync element values

This is why plugins marked as "core" assembly type cause incompatible sessions with those who don't have the plugin.

Source: https://wiki.resonite.com/Data_model
