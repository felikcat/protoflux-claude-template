# ProtoFlux:ApplyCharacterForce

> Source: https://wiki.resonite.com/ProtoFlux:ApplyCharacterForce

Apply Character Force

\*

Next

Force

Character

IgnoreMass

Physics

The `Apply Character Force` node takes in a [character controller](https://wiki.resonite.com/Component:CharacterController "Component:CharacterController") reference and a force, then pushes the character controller in the direction.

Unlike [Impulse](https://wiki.resonite.com/ProtoFlux:Apply_Character_Impulse "ProtoFlux:Apply Character Impulse") where you send a force once to send the character controller in a direction, this node is made to apply a force in a direction over time.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Calls to push this character controller.

### Force ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The force to push this character controller.

### Character ( [Character Controller](https://wiki.resonite.com/Component:CharacterController "Component:CharacterController"))

The character controller reference.

### IgnoreMass ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

The option to ignore mass in the character controller component when being sent in a direction.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Continues execution from here.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ApplyCharacterForce&oldid=109261](https://wiki.resonite.com/index.php?title=ProtoFlux:ApplyCharacterForce&oldid=109261)"

Contents