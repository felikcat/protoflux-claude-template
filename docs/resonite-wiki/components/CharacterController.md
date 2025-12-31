# Component:CharacterController

> Source: https://wiki.resonite.com/Component:CharacterController

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/37/CharacterControllerComponent.png/510px-CharacterControllerComponent.png)](https://wiki.resonite.com/File:CharacterControllerComponent.png) **Character Controller** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

## Description

The Character Controller component is primarily designed to be part of the [Locomotion](https://wiki.resonite.com/Component:PhysicalLocomotion "Component:PhysicalLocomotion") system and is what used for user movement and simulating physics relating to this.

It has many settings and values that can alter the way on how a user can control either their self or another slot (For example: Vehicles). These Settings allow you to control the mass, speed, force, etc. This flexibility also allows for uses far beyond it's original intended design.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

When getting the character controller of a user, avoid using the character controller under the user root slot. Instead use the node [Find Character Controller From User](https://wiki.resonite.com/ProtoFlux:Find_Character_Controller_From_User "ProtoFlux:Find Character Controller From User").


Keep in mind that the character controller under the user root slot is currently useless (as in, not used besides it needing to be there) at this time. And removing it just recreates it back on the user root slot.

For this component, when using some features, you may need to either write/drive the field `SimulatingUser`. This will activate the character controller on the slot and make it start simulating. Doing this also lets you use some nodes such as [Is Character Controller](https://wiki.resonite.com/ProtoFlux:Is_Character_Controller "ProtoFlux:Is Character Controller") and [Is Character On Ground](https://wiki.resonite.com/ProtoFlux:Is_Character_On_Ground "ProtoFlux:Is Character On Ground"), and without a simulating user, the values from some nodes would not be updated.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `SimulatingUser` | **[User](https://wiki.resonite.com/Type:User "Type:User")** | The user who is currently simulating and networking this Character Controller. |
| `CharacterRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to simulate, can be any inputted slot. |
| `HeadReference` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | Dictates where to simulate the collider and based on the slot's forward direction, will decide what a "forward" movement is based on your joystick/input. |
| `SimulateRotation` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Allow the object simulated by this object to rotate, essentially making it a rigid body. See warning. |
| `MassScaling` | **[PhysicsScalingMode](https://wiki.resonite.com/Type:PhysicsScalingMode "Type:PhysicsScalingMode")** | How to scale the mass based on this component's slot scale. |
| `ForceScaling` | **[PhysicsScalingMode](https://wiki.resonite.com/Type:PhysicsScalingMode "Type:PhysicsScalingMode")** | How to scale the force based on this component's slot scale. |
| `SpeedScaling` | **[PhysicsScalingMode](https://wiki.resonite.com/Type:PhysicsScalingMode "Type:PhysicsScalingMode")** | How to scale the speed based on this component's slot scale. |
| `JumpScaling` | **[PhysicsScalingMode](https://wiki.resonite.com/Type:PhysicsScalingMode "Type:PhysicsScalingMode")** | How to scale the jump force based on this component's slot scale. |
| `GravityScaling` | **[PhysicsScalingMode](https://wiki.resonite.com/Type:PhysicsScalingMode "Type:PhysicsScalingMode")** | How to scale the gravity effect based on this component's slot scale. |
| `LinearDamping` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how fast the character controller slows down when no other forces are being applied to it |
| `AngularDamping` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how fast thus character slows down its rotation when no other forces are being applied to it. |
| `Margin` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Unused. |
| `StepUpHeight` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How big of a ledge the character controller can step up |
| `StepUpCheckDistance` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | determines the distance the shape is swept in the movement direction to determine if it's free of other obstacles |
| `KillVerticalVelocityAfterStepUp` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | will convert any vertical velocity into directional one in the current planar direction of the movement and push the player back down, preventing the player from getting too much air when running off a ramp or stairs. |
| `EdgeDetectionDepth` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the smallest size an edge can be that the character can stand on while against a wall |
| `Speed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast this character controller can move. |
| `SlidingSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how fast the character controller moves when sliding down a slope |
| `AirSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how fast the character moves in the air |
| `TractionForce` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much force is needed to overcome standing friction. |
| `SlidingForce` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How much force is needed to stay moving |
| `AirForce` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | the force needed to move in the air |
| `MaximumGlueForce` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Reduces the velocity of breaking contact from a surface vertically be under this speed. This is useful for simulating sticky surfaces, where the user cannot jump as high. |
| `MaximumTractionSlope` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Maximum Traction angle (degrees) before user slides down a slope, even if they are actively trying to walk up it. |
| `MaximumSupportSlope` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Maximum Support angle (degrees) before user slides down a slope, when not working against the slope. |
| `JumpSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The speed of the velocity applied when jumping on a slope with an angle less than or equal to `MaximumTractionSlope`. |
| `SlidingJumpSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The speed of the velocity applied when jumping on a slope with an angle greater than `MaximuSupportSlope`. |
| `Gravity` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | Force of Gravity for this character controller |
| `GravitySpace` | _direct_ **[RootSpace](https://wiki.resonite.com/Type:RootSpace "Type:RootSpace")** | The coordinate space in which `Gravity` is applied in. applying gravity to world space using this field, can allow a user to stay upright despite a floor they're parented under is being rotated. which generates interesting effects. |
| `DebugVisualDuration` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | Allows for the component to visualize the force vectors acting on the character simulator if set above 0. |
| `__height` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Height of the driven [CapsuleCollider (Component)](https://wiki.resonite.com/CapsuleCollider_(Component) "CapsuleCollider (Component)") Currently does nothing. |
| `__radius` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Radius of the driven [CapsuleCollider (Component)](https://wiki.resonite.com/CapsuleCollider_(Component) "CapsuleCollider (Component)") Currently does nothing. |
| `__mass` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Mass of the of the driven [CapsuleCollider (Component)](https://wiki.resonite.com/CapsuleCollider_(Component) "CapsuleCollider (Component)") Currently does nothing. |
| `__collideWithOtherCharacters` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Currently does nothing. |
| `__ignoreRaycasts` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Currently does nothing. |
| `__rootAtBottom` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Currently does nothing. |

Fields
Collapse

## Usage

This component is usually used internally by Resonite to simulate user movement physics like walking and climbing.

But the component can also be manipulated to create "Fake Players" commonly known by Resonite users as "NPC's". Before doing this, know that the physics simulation is always inconsistent when viewed by different players in the same session. It also causes high amounts of networking and FPS lag. Use too many and you may start rising in [Queued Packets](https://wiki.resonite.com/index.php?title=Queued_Packets&action=edit&redlink=1 "Queued Packets (page does not exist)").

The character controller can also be used as a ball and simulates rolling, falling, collisions and momentum transfer, but for individual things that fly or bounce, using a [Trajectory Position](https://wiki.resonite.com/ProtoFlux:Trajectory_Position "ProtoFlux:Trajectory Position") ProtoFlux node is vastly superior.

This component is also used in certain types of vehicles and making them controllable by the user. This is done by having a vehicle you want to make controllable, then making an anchor for the user to sit in, then setting up this component to make that user become the simulating user, thus making their controls change in such a way where they are controlling a vehicle they are sitting on.

The CharacterRoot slot input when null will do its transforms on the slot the CharacterController component is on, however when given a slot the component will instead make those transforms happen on the slot inputted. Combined with defining the HeadReference, you can control external slots without moving where the CharacterController component is and have them work with physical obstacles. For a quick example of this behavior, you can modify your current active locomotion's CharacterController on the CharacterRoot field to point towards another slot while defining the HeadReference to instead move the inputted slot while you stand still.

This component can use sphere, box and other colliders that have volume in addition to the capsule collider.

Note, due to the unique behavior of the HeadReference input defining where the CharacterController's collider is in the simulation, visualizing the collider via the inspector will not be correct.

## Examples

A Shrike NPC running around the cloud home:

[![](https://wiki.resonite.com/images/thumb/5/53/BallPitExample.png/300px-BallPitExample.png)](https://wiki.resonite.com/File:BallPitExample.png) A simple Ball Pit made with CharacterController demonstrating physics. (Worlds: 'ball pit')

[![A 4 foot tall Avali NPC with the likeness of a user named Shrike, running in the Resonite Default Cloud Home. It is set to Nighttime and the NPC is near the Reading Nook running towards it.](https://wiki.resonite.com/images/thumb/6/6a/Example_Of_A_CharacterController_NPC.webp/200px-Example_Of_A_CharacterController_NPC.webp.png)](https://wiki.resonite.com/File:Example_Of_A_CharacterController_NPC.webp "A 4 foot tall Avali NPC with the likeness of a user named Shrike, running in the Resonite Default Cloud Home. It is set to Nighttime and the NPC is near the Reading Nook running towards it.")

## See also

### Protoflux Notes

Using [Character Controller User](https://wiki.resonite.com/ProtoFlux:Character_Controller_User "ProtoFlux:Character Controller User") will give you the Simulating User of this Character Controller Component.

Using [Get User From Component](https://wiki.resonite.com/ProtoFlux:Get_User_From_Component "ProtoFlux:Get User From Component") will give you the Owner User of this Character Controller Component.

Using [Allocating User](https://wiki.resonite.com/ProtoFlux:Allocating_User "ProtoFlux:Allocating User") will give you the User that spawned out a slot that has this Character Controller Component.

### Components

The Physical Locomotion modules use a [Capsule Collider](https://wiki.resonite.com/Component:CapsuleCollider "Component:CapsuleCollider") who's bounds are generated from the [SingleShapeCharacterControllerManager](https://wiki.resonite.com/Component:SingleShapeCharacterControllerManager "Component:SingleShapeCharacterControllerManager") component. This controls how an avatar interacts with the world.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CharacterController&oldid=114277](https://wiki.resonite.com/index.php?title=Component:CharacterController&oldid=114277)"

Contents