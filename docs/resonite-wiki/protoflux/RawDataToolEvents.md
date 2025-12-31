# ProtoFlux:RawDataToolEvents

> Source: https://wiki.resonite.com/ProtoFlux:RawDataToolEvents

Raw Data Tool Events

Equipped

Dequipped

ToolUpdate

PrimaryPressed

PrimaryHeld

PrimaryReleased

SecondaryPressed

SecondaryHeld

SecondaryReleased

Tool

null

∅

Tools

The `Raw Data Tool Events` node takes in a referenced [raw data tool](https://wiki.resonite.com/Component:RawDataTool "Component:RawDataTool"), and depending on the actions or inputs from the user, this node will fire specific events. This can let the user make a custom [tool](https://wiki.resonite.com/Tools "Tools") to run any custom flux when connected from this node.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you are looking for generic tool events, try the [Tool Events](https://wiki.resonite.com/ProtoFlux:Tool_Events "ProtoFlux:Tool Events") node instead.


## Outputs

### Equipped ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the tool is equipped.

### Dequipped ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Fires when the tool is dequipped.

### ToolUpdate ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Fires every frame when this tool is equipped on the user.

### PrimaryPressed ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Fires when primary is pressed by the user while this tool is equipped.

### PrimaryHeld ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Fires when primary is held by the user while this tool is equipped.

### PrimaryReleased ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Fires when primary is released by the user while this tool is equipped.

### SecondaryPressed ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Fires when secondary is pressed by the user while this tool is equipped.

### SecondaryHeld ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Fires when secondary is held by the user while this tool is equipped.

### SecondaryReleased ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Fires when secondary is released by the user while this tool is equipped.

## Globals

### Tool ( [RawDataTool](https://wiki.resonite.com/index.php?title=Type:RawDataTool&action=edit&redlink=1 "Type:RawDataTool (page does not exist)"))

The raw data tool component reference.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:RawDataToolEvents&oldid=110543](https://wiki.resonite.com/index.php?title=ProtoFlux:RawDataToolEvents&oldid=110543)"

Contents