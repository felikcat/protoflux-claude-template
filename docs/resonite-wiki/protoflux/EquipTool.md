# ProtoFlux:EquipTool

> Source: https://wiki.resonite.com/ProtoFlux:EquipTool

Equip Tool

\*

OnEquipped

Tool

OnEquipFail

User

Side

DequipExisting

Tools

The **Equip Tool** node equips a [tool](https://wiki.resonite.com/Tools "Tools") to the [user](https://wiki.resonite.com/User "User"), optionally dequipping an existing tool.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Receives an impulse to equip the tool to a user.

### Tool ( [ITool](https://wiki.resonite.com/Type:ITool "Type:ITool"))

The tool to equip.

If the tool is null or the tool is already equipped `OnEquipFail` will fire.

### User ( [User](https://wiki.resonite.com/User "User"))

The user to equip the tool to.

If the user is null then the [execution context's](https://wiki.resonite.com/ExecutionContext "ExecutionContext") local user will be used, and if that local user is null then `OnEquipFail` will fire.

### Side ( [Chirality](https://wiki.resonite.com/Type:Chirality "Type:Chirality"))

The chirality of the user to equip this tool.

If an [interaction handler](https://wiki.resonite.com/Component:InteractionHandler "Component:InteractionHandler") for the side can not be found then `OnEquipFail` will fire.

### DequipExisting ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Should this tool dequip an already held tool.

If an another tool is already equipped and `DequipExisting` is false then `OnEquipFail` will fire.

## Outputs

### OnEquipped ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires if the tool successfully equips to a user.

### OnEquipFail ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires if the tool fails to equip.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:EquipTool&oldid=109729](https://wiki.resonite.com/index.php?title=ProtoFlux:EquipTool&oldid=109729)"

Contents