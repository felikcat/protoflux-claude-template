# ProtoFlux:ApplyCharacterImpulse

> Source: https://wiki.resonite.com/ProtoFlux:ApplyCharacterImpulse

Apply Character Impulse

\*

Next

Impulse

Character

IgnoreMass

Physics

Applies a [impulse](https://en.wikipedia.org/wiki/Impulse_(physics) "wikipedia:Impulse (physics)") to a character controller, impulses are similar but different from the [force](https://wiki.resonite.com/ProtoFlux:Apply_Character_Force "ProtoFlux:Apply Character Force") node from a physics perspective.

Impulse is the change in momentum of an object, or otherwise an "normalized" version of force.

In this case, the impulse node takes Force and applies it across [dT](https://wiki.resonite.com/ProtoFlux:Div_Delta_Time "ProtoFlux:Div Delta Time"), making it framerate independent.

## Inputs

### Input ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Calls to trigger the character impulse.

### Impulse ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The direction to send the slot holding the character controller component.

### Character ( [Character Controller](https://wiki.resonite.com/Component:CharacterController "Component:CharacterController"))

The reference itself to be sent in a direction.

### Ignore Mass ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

The option to ignore mass in the character controller component when being sent in a direction.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Continues execution from here.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ApplyCharacterImpulse&oldid=109263](https://wiki.resonite.com/index.php?title=ProtoFlux:ApplyCharacterImpulse&oldid=109263)"

Contents