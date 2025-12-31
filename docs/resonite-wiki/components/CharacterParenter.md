# Component:CharacterParenter

> Source: https://wiki.resonite.com/Component:CharacterParenter

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/0/00/CharacterParenterComponent.png/510px-CharacterParenterComponent.png)](https://wiki.resonite.com/File:CharacterParenterComponent.png) **Character Parenter** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Character Parenters are a component that allow for parenting or aligning the gravity of a user when they hit a collider.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TriggersOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to only allow trigger colliders that are part of this component's slot hierarchy to activate parenting. |
| `NestIntoSpace` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Parent the user into the slot `ParentSpace` or not. |
| `MustBeOnGround` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The user must be on the ground according to the [character controller](https://wiki.resonite.com/Component:CharacterController "Component:CharacterController") before they will be aligned/parented. |
| `Filters` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[CharacterParenter.AlignmentFilter](https://wiki.resonite.com/Component:CharacterParenter#AlignmentFilter)** | What directions a user must be aligned to relative to the slot this component is on for them to get parented. |
| `IgnoreParentUser` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Ignore the active user of this component when attempting to parent a user. |
| `ParentSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The coordinate space that calculations should be done in. |

Fields
Collapse

## Behavior

Disabling the collider the CharacterParenter is connected to might be preferred compared to disabling the slot or the CharacterParenter's enabled state itself, as disabling the collider will throw a ContactEnd event to the CharacterPareneter and correctly de-parent the user's inside.

Disabling the CharacterParenter itself while users are inside the ParentSpace will mean the component can't de-parent users correctly and might not be wanted behavior.

## Examples

This component is used in many different zones where keeping a user moving with something is essential. Objects like this include: platforms, elevators, mech control rooms, parkour platforms, spaceships, and the list can go on.

## See Also

[Issue 353, bumpiness issues when on another user](https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/353)

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CharacterParenter&oldid=113350](https://wiki.resonite.com/index.php?title=Component:CharacterParenter&oldid=113350)"

Contents