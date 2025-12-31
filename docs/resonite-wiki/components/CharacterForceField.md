# Component:CharacterForceField

> Source: https://wiki.resonite.com/Component:CharacterForceField

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/ab/CharacterForceFieldComponent.png/510px-CharacterForceFieldComponent.png)](https://wiki.resonite.com/File:CharacterForceFieldComponent.png) **Character Force Field** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

_This article or section is a stub. You can help the Resonite wiki by expanding it._

This component creates a force field that allows the setting of or applying force to the velocity of [Character Controllers](https://wiki.resonite.com/Component:CharacterController "Component:CharacterController").

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TriggersOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to only allow trigger colliders attached to character controller objects to activate the force field. |
| `Force` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | force direction and magnitude to apply a character controller within range with. |
| `ForceMode` | **[CharacterForceField.Mode](https://wiki.resonite.com/Component:CharacterForceField#Mode)** | Whether to use impulse, apply, or set velocity using `Force` |
| `ForceSpace` | **[CharacterForceField.Space](https://wiki.resonite.com/Component:CharacterForceField#Space)** | Whether to do the force direction in local or global space (so should `Force` be scaled and rotated by the slot this is on or not?) |
| `RadialForceRadius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The range of effect this force field has. |
| `ForceSlotSpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | Override the transform space for `Force` with this if set. |
| `MinActivationVelocity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum velocity a character controller has to be going to trigger this force field. |
| `MaxForceVelocity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast the character controller's velocity can be at max after being affected by this component when the user isn't holding [Jump](https://wiki.resonite.com/Controls "Controls") |
| `HoldJumpMaxForceVelocity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast the character controller's velocity can be at max after being affected by this component when the user is holding [Jump](https://wiki.resonite.com/Controls "Controls") |
| `PreseveDirectionAcrossPlane` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Calculates a plane that is perpendicular to the vector `Force` (like a stick stuck into a piece of paper) and maintains the initial direction of the velocity of the character controller in either the forward or backwards facing direction of this plane. |
| `IgnoreParentUser` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to ignore the active user when finding character controllers within range of `RadialForceRadius`. This does not ignore character controllers that are simulated by the user. |
| `NoJumpMultiplier` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to multiply the effect of `Force` when the user isn't holding [Jump](https://wiki.resonite.com/Controls "Controls") |
| `HoldJumpMultiplier` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much to multiply the effect of `Force` when the user is holding [Jump](https://wiki.resonite.com/Controls "Controls") |
| `MaxCharacterVelocity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The maximum velocity this component can set a character controller's speed to after setting a force on it. |
| `MinCharacterVelocity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum velocity this component can set a character controller's speed to after setting a force on it. |
| `CharacterVelocityDampeningSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast to slow the user down. this can be used to give the effect of jumping into molasses. |

Fields
Collapse

## Behavior

Needs a collider on the same hierarchy to allow triggering this component.

## Examples

## See Also

[Character Controllers](https://wiki.resonite.com/Component:CharacterController "Component:CharacterController")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CharacterForceField&oldid=97434](https://wiki.resonite.com/index.php?title=Component:CharacterForceField&oldid=97434)"

Contents