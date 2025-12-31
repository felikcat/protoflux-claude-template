# ProtoFlux Overview

> Source: https://wiki.resonite.com/ProtoFlux

ProtoFlux is a Node based scripting language that can be manipulated in 3D space using the ProtoFlux Tool.

> ProtoFlux is the crown jewel of our creative tools - the most powerful visual programming language that our experienced team has designed to date, which lets you quickly prototype and build anything from simple interactions to complex games and systems - with full real-time collaboration support and immediate feedback. Build anything from avatar and world interactivity, to complex systems, and games.

## Usage

ProtoFlux is represented in the world as nodes that can be selected from the ProtoFlux Node Browser, and spawned from the ProtoFlux Tool.

You can easily spawn a ProtoFlux Tool from the _Resonite Essentials_ folder included in your Inventory to begin scripting with ProtoFlux (The tool itself is found in the Tools folder in the Essentials Folder).

### Spawning Nodes
1. Equip the ProtoFlux Tool
2. Open Context menu to access the node browser
3. Double click a node to select it (name appears above tool)
4. Double click again to spawn the selected node

You can also quick select nodes that already exist by tapping Secondary while pointing at the node.

### Connecting Nodes
- Point laser at a node's connection point
- Hold Primary (Trigger/Left Click)
- Drag the wire to another node's connection point
- Let go of Primary

### Cutting Connections
- Intersect the red line from the ProtoFlux Tool tip while holding Primary

## Interfacing With Components / Slots

To change or read slot/component properties with the ProtoFlux Tool:
1. Point at a field name (e.g., 'Position') and grab with your controller
2. While holding, open your Context menu
3. Choose one of three options:

| Option | Description |
|--------|-------------|
| **Source** | Spawns a node to read/write the field value |
| **Drive** | Spawns a node to continuously locally write a value |
| **Reference** | Spawns a node to get a reference to the field (useful for Tween nodes) |

## Variables

In ProtoFlux, there are 3 types of generic variables:

| Type | Description | Sync |
|------|-------------|------|
| **Data Model Store** | Automatically synced to all users upon being written to | Yes |
| **Store** | Similar to standard variables, not synced over network | No |
| **Local** | Instanced for different execution chains, discarded when execution ends | No |

### Data Model Store
- Simplest type
- Auto-synced across network
- Can impact performance if overused

### Store
- Not synced over network
- Alleviates network overhead
- Could lead to desync between users

### Local
- Instanced per execution chain
- If ProtoFlux called twice at once, each context uses unique instance
- Discarded when execution ends

## Packing / Unpacking ProtoFlux

### To Pack:
1. Hold Secondary while pointing at ProtoFlux nodes
2. Nodes become light blue (selected)
3. Create an empty Slot using the Inspector
4. Grab the slot and open Context menu
5. Select "Pack Into"

### To Unpack:
1. Grab the slot containing packed ProtoFlux
2. Open Context menu with ProtoFlux Tool equipped
3. Select "Unpack"

## See Also
- [Impulses](./impulses.md)
- [Dynamic Variables](./dynamic-variables.md)
