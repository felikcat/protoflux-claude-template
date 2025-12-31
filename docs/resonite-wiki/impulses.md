# Impulses

> Source: https://wiki.resonite.com/Impulses

**Impulses** (or calls) are discrete actions within ProtoFlux's ExecutionContext - one of the two basic chain types. Unlike continuous input/output chains, impulses push task execution along the chain, similar to imperative programming.

## Overview

Nodes performing discrete actions require an impulse to execute. For example, duplicating a slot can't trigger whenever it wants.

### Impulse Flow
- Special input `*` of type _Call_ triggers the action
- Chain continues via `Next` output
- Upon receiving impulse, node evaluates all non-impulse inputs

### Sync Behavior
- Impulses are local runtime by default
- Actions affecting FrooxEngine data model get synced across users:
  - Writing to non-driven synced fields
  - Managing slots
  - Setting non-driven dynamic variables

## Context

Impulses are attached to a particular ExecutionContext instance, carrying values throughout the chain:
- Local values
- Action node outputs

### Context Preservation
- Context kept when passing through same _node group_
- Context lost when execution disconnects to different node group
- Node groups = all nodes connected through wires or references

### Example
If a dynamic impulse triggers another, which writes to a local, the change will NOT be seen by the first trigger's `Next` path - execution left the node group.

## Impulse Flow Types

### Non-Async (Synchronous)
- Runs entirely in one engine update
- Halts engine until complete
- Only syncs difference between initial state and end of update
- Example: Duplicating and removing slots in one chain syncs nothing

### Async (Asynchronous)
Required when actions may take multiple engine updates.

Features:
- Suspend and resume execution at will
- Preserves locals and outputs across updates
- Explicit suspend: `Delay` node
- Implicit wait: `Play One Shot And Wait`

#### Starting Async from Sync
Use `Start Async Task` node:
- Creates _branched_ ExecutionContext at `OnTriggered`
- Values duplicated into new context
- Neither context affects the other after

#### Async Context Sharing
Other async nodes _share_ context:
- Local modified in `Delay`'s `OnTriggered` reflects in `Next`
- Makes async flow powerful for complex sequences

### Performance Consideration
For processing lots of data, use async flow to spread execution across frames - prevents framerate hitch at cost of slightly longer total time.

## Common Impulse Sources

| Source | Description |
|--------|-------------|
| `Call Input` | Created by dragging impulse input + secondary |
| `Dynamic Impulses` | Cross-hierarchy impulse triggers |
| `Button Events` | UI button interactions |
| `Fire On X` | Fire On True/False/Change |
| `World/Item Events` | OnStart, OnActivated, etc. |

## Variable Types and Context

| Variable | Context Scope | Synced |
|----------|---------------|--------|
| Data Model Store | World Model (all users) | Yes |
| Store | Per user | No |
| Local | Per impulse chain | No |

### Local Variables
- Only valid within impulse chain and ProtoFlux group
- Outside impulses: contain default value (0 or null)
- Cannot view directly - must capture to non-local first

## See Also
- [ProtoFlux:Local](https://wiki.resonite.com/ProtoFlux:Local)
- [ProtoFlux:Store](https://wiki.resonite.com/ProtoFlux:Store)
- [ProtoFlux:Data Model Store](https://wiki.resonite.com/ProtoFlux:Data_Model_Store)
- [Category:ProtoFlux:Flow](https://wiki.resonite.com/Category:ProtoFlux:Flow)
