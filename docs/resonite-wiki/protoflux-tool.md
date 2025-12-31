# ProtoFlux Tool

The ProtoFlux Tool is one of the most useful tools in Resonite, allowing you to create, connect, and pack ProtoFlux nodes.

## Where to Get the Tool

Found in: **Resonite Essentials** (public folder in every new user's inventory)

## Using the Tool

Equip like any standard tool. While equipped, your context menu gains extra options:

| Option | Description |
|--------|-------------|
| **Browse nodes** | Summon a ProtoFlux node browser |
| **Toggle Overview mode** | Changes visual complexity of nodes |
| **Unequip** | Unequip the tool |

## Connecting Wires

1. Point laser at a node's input or output
2. Hold primary
3. Wire connects to tip of ProtoFlux tool
4. Point laser at another node's input or output
5. Release primary to connect

**Tip:** While dragging a wire, hit secondary to create a display or an input.

## Cutting Wires

1. Hold primary (creates red beam)
2. Cross wires with beam (highlights them red)
3. Release while highlighting a wire to destroy connection

**Desktop mode:** Ctrl+Left-click nodes while in UI focus mode to cut wires.

## Copying Nodes

1. Select the nodes you want to copy
2. Press secondary

## Selecting a Group of Nodes

1. Point laser at a node
2. Hold secondary
3. Packing indicator circle fills, then nodes turn blue

While selected, you can:
- Move the group
- Destroy the group
- Duplicate the group
- Pack the group

Additional context menu option:
- **Clear Selection** - Clears currently selected nodes

## Packing ProtoFlux Nodes

1. Select the group of nodes to pack
2. Grab the target slot from Scene Inspector
3. Open context menu while holding the slot reference

Options appear:
- **Pack Into** - Pack selected nodes into the held slot
- **Unpack** - Unpack nodes from held slot for editing

If you open context menu while hovering over a node:
- **Pack In Place** - Packs nodes to their current parent

### Accidental Pack In Place Recovery

If Pack In Place targets world Root or problematic parent:
1. Find any one node from that group
2. Unpack it
3. Select any unpacked node to bring back entire group

Source: https://wiki.resonite.com/ProtoFlux_Tool
