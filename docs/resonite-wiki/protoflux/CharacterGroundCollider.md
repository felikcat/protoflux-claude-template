# ProtoFlux:CharacterGroundCollider

> Source: https://wiki.resonite.com/ProtoFlux:CharacterGroundCollider

Character Ground Collider

Character

\*

Physics

The `Character Ground Collider` node takes in a [character controller](https://wiki.resonite.com/Component:CharacterController "Component:CharacterController") reference and returns an [ICollider](https://wiki.resonite.com/Type:ICollider "Type:ICollider") from what it detects under this slot's character controller component. "Ground" refers to your local rotation, so you could be standing on the ceiling and this would detect that the ceiling is your "ground".

## Inputs

### Character ( [Character Controller](https://wiki.resonite.com/Component:CharacterController "Component:CharacterController"))

The Character Controller reference.

## Outputs

### \\* ( [ICollider](https://wiki.resonite.com/Type:ICollider "Type:ICollider"))

The "ground" this character controller detects (whatever it thinks ground is, determined by what is under it).

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:CharacterGroundCollider&oldid=109351](https://wiki.resonite.com/index.php?title=ProtoFlux:CharacterGroundCollider&oldid=109351)"

Contents