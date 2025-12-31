# Linkage (Links, Drives, and Hooks)

**Linkage** is a way to give exclusive control of the value of a sync element—usually a field—to one singular source in various ways.

## Links

The most basic form of linkage. **Linked elements appear as cyan** in the inspector.

- Establishes exclusive control of the linked element to the driver
- Only the driver can update the value
- This relation is synced across all users (except for network delays)
- Rarely used directly; mainly for specific purposes like driving a FieldDrive<T> type

## Drives

An extension of links and the **most common form of linkage**. **Driven elements appear as purple** in the inspector.

- Establishes exclusive control like links
- **Unlike links, changes are NOT synchronized over network**
- Value of driven element is local to each user
- Used to reduce network traffic by having each user calculate values locally

### Creating Drives

**With Components:**
- Find drivers under Transform/Drivers or Relations categories

**With ProtoFlux:**
1. Hold the ProtoFlux Tool
2. Drag a field from an inspector
3. Open context menu while holding the field
4. Choose "Drive" option
5. Creates a Value Field Drive or Object Field Drive node

**Alternative:** Use the FieldHook node for lower-level control:
- Start/stop drives using impulses
- Optionally use a hook to allow other sources to write

## Hooks

An optional part of linkage that certain drivers may utilize. It's a function run when the linked element attempts to be changed.

### WriteBack

The most common hook. When you attempt to write to the driven field:
- The write goes through
- Writes to both the source value and driven value at once

**Interesting effect:** If you ValueCopy a field onto itself with WriteBack enabled:
- The field becomes a local field with data model support
- Acts like a ProtoFlux Store but backed by the data model

## How Linked Fields Are Updated

Linkage is separate from how values get updated:
- Linkage ensures sync element is controlled by one source only
- **When** and **how** the element gets updated is the driver's responsibility
- Could be every engine update, on detected changes, or any other method

### ProtoFlux Drives

In ProtoFlux FrooxEngineContext, a FieldDrive node is a listener node:
- Evaluates input when notified of changes from input context
- Makes ProtoFlux drives **lazy by default** (only evaluating when needed)
- If input graph has a ContinuouslyChanging node, drive evaluates every engine update

### Breaking/Opening Drives

Click the tag to the left of field name for options:
- **Break** the drive/link
- **Find the source** of the link/drive
- **Reset** field to default (may have no effect on driven fields)

**Caution:** Be careful when breaking drives/links unless you understand what they're doing.

Source: https://wiki.resonite.com/Linkage
