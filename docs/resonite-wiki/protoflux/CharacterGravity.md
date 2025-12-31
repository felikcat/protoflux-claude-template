# ProtoFlux:CharacterGravity

> Source: https://wiki.resonite.com/ProtoFlux:CharacterGravity

Character Gravity

Character

Gravity

Actual Gravity

Physics

The `Character Gravity` node returns a referenced [character controller](https://wiki.resonite.com/Component:CharacterController "Component:CharacterController") gravity. The gravity output is used when you want the character controller's current gravity it is aiming for when simulating. The actual gravity is what the character controller is simulating now, and can be varied when using it dependiong on the settings on the character controller (specifically the gravity scale field).

## Usage

You can use the actual gravity output of this node to control how gravity works for certain character controllers that need to have different values effect them in different ways (using both the user's transform scale and the component's gravity scale). You can set the simulating user's gravity scale to cubic and have their gravity be effected by their size. Using Linear will keep the gravity the same no matter the size of the user. (Tested on users jumping while changing the gravity scale field in the character controller component).

## Inputs

### Character ( [Character Controller](https://wiki.resonite.com/Component:CharacterController "Component:CharacterController"))

The character controller reference.

## Outputs

### Gravity ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The current gravity from this character controller that it "should" try to simulate.

### Actual Gravity ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The actual gravity this character controller is simulating.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:CharacterGravity&oldid=109349](https://wiki.resonite.com/index.php?title=ProtoFlux:CharacterGravity&oldid=109349)"

Contents