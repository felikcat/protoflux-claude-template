# Component:WorldSwitcher

> Source: https://wiki.resonite.com/Component:WorldSwitcher

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This article describes a feature marked as legacy—this usually means there's a newer, better alternative. Legacy features might not be removed but they will not be updated, and the [team](https://wiki.resonite.com/Resonite_Team "Resonite Team") will not provide any support for them.


Collapse **Component image**

[File:WorldSwitcherComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=WorldSwitcherComponent.png "File:WorldSwitcherComponent.png") **World Switcher** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **WorldSwitcher** component is legacy content for switching worlds via rotating the wrist.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Show` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the switcher should be shown. |
| `IgnoreTouchesFrom` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | A slot to ignore touch events from. like the hand it is on. |
| `_repulsionTree` | **[RepulsionTreeSimulator](https://wiki.resonite.com/Component:RepulsionTreeSimulator "Component:RepulsionTreeSimulator")** | The repulsion tree used to arrange the orbs in the menu. |
| `_linesMesh` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[MultiSegmentMesh](https://wiki.resonite.com/Component:MultiSegmentMesh "Component:MultiSegmentMesh")** | A multi segment mesh used to create the selection and indication visuals. |
| `_slider` | **[Slider](https://wiki.resonite.com/Component:Slider "Component:Slider")** | The slider used as part of the selection menu. |
| `_centerOrb` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The center orb that moves the rest of the orbs to places around it. |
| `_visualRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot for all the visuals of the switcher. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``WorldOrbTouched:Action`2<WorldOrb, TouchEventInfo>`` | **[Action\`2](https://wiki.resonite.com/index.php?title=Type:Action%602&action=edit&redlink=1 "Type:Action`2 (page does not exist)") < [WorldOrb](https://wiki.resonite.com/Component:WorldOrb "Component:WorldOrb"), [TouchEventInfo](https://wiki.resonite.com/index.php?title=Type:TouchEventInfo&action=edit&redlink=1 "Type:TouchEventInfo (page does not exist)") >** | ✓ | Handles when a world orb is touched for switching to it. |
| ``WorldOrbLongPressed:Action`1<WorldOrb>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [WorldOrb](https://wiki.resonite.com/Component:WorldOrb "Component:WorldOrb") >** | ✓ | Handles when a world orb is long touched to bring up options. |

Triggers
Collapse

## Usage

Can be brought up through the legacy world switcher option in the legacy settings options.

## Examples

Used as part of the old systems older platforms had.

## See Also

- [World](https://wiki.resonite.com/World "World")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:WorldSwitcher&oldid=100818](https://wiki.resonite.com/index.php?title=Component:WorldSwitcher&oldid=100818)"

Contents