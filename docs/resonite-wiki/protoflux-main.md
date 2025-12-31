# ProtoFlux

ProtoFlux is a Node based scripting language that can be manipulated in 3D space using the ProtoFlux Tool.

> ProtoFlux is the crown jewel of our creative tools - the most powerful visual programming language that our experienced team has designed to date, which lets you quickly prototype and build anything from simple interactions to complex games and systems - with full real-time collaboration support and immediate feedback. Build anything from avatar and world interactivity, to complex systems, and games.

## Usage

ProtoFlux is represented in the world as nodes that can be selected from the ProtoFlux Node Browser, and spawned from the ProtoFlux Tool.

You can easily spawn a ProtoFlux Tool from the *Resonite Essentials* folder included in your Inventory to begin scripting with ProtoFlux (The tool itself is found in the Tools folder in the Essentials Folder).

### Spawning Nodes

1. Equip the ProtoFlux Tool from the Essentials folder
2. Open your Context menu to access the ProtoFlux node browser
3. Double click a node to select it (name appears above the tool)
4. Double click again to spawn the selected node

You can also quick select nodes that already exist by tapping Secondary while pointing at the node.

### Connecting Nodes

- Point the laser at a node's connection point
- Hold Primary (Trigger/Left Click)
- Drag the wire to another node's connection point
- Release Primary

To cut connections, intersect the red line from the ProtoFlux Tool tip while holding Primary.

## Interfacing With Components / Slots

To read/change properties of a slot or component:

1. Point at the field name with the ProtoFlux Tool (e.g., 'Position' on a slot)
2. Grab with your controller (or right click)
3. Open your Context menu while grabbing

This gives you three options:

| Option | Description |
|--------|-------------|
| **Source** | Spawns a node that references the source of the property. Used to read or write the field value. |
| **Drive** | Spawns a node to continuously locally write a value to the variable. |
| **Reference** | Spawns a node to get the reference to the field. Useful for nodes like Tween Value. |

## Packing / Unpacking ProtoFlux

### Packing

1. Hold Secondary while pointing at a group of ProtoFlux (becomes light blue when selected)
2. Create an empty Slot using the Inspector
3. Grab the slot so its name appears above the ProtoFlux Tool
4. Open Context menu and select "Pack Into"

Once packed, ProtoFlux still functions but no longer shows visuals and applies optimizations.

### Unpacking

1. Grab the slot the ProtoFlux was packed into
2. Open Context menu with ProtoFlux Tool equipped
3. Select the unpack option

## Variables

In ProtoFlux, there are 3 types of generic variables:

| Variable Type | Description |
|--------------|-------------|
| **Data Model Store** | Automatically synced to all users upon being written to. Most simple scripts can use these, but can impact performance if overused. |
| **Store** | Similar to standard variables in most languages. Not synced over network, alleviates overhead but could lead to desync. |
| **Local** | Instanced for different execution chains. If ProtoFlux is called twice at once, each context uses a unique instance that gets discarded when execution ends. |

## Impulses

See [Impulses](impulses.md) for detailed information.

## Trivia

- ProtoFlux's codename in development was "Spaghett"

Source: https://wiki.resonite.com/ProtoFlux
