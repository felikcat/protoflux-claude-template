# ProtoFlux:RaycastOne

> Source: https://wiki.resonite.com/ProtoFlux:RaycastOne

Raycast One

\*

OnHit

Origin

OnMiss

Direction

HitCollider

MaxDistance

HitDistance

HitTriggers

HitPoint

UsersOnly

HitNormal

DebugDuration

HitTriangleIndex

Root

Physics

The **Raycast One** node performs a single raycast check when an impulse is received. The input parameters determine from where, in what direction, and how far the ray should be cast as well as determining which colliders are valid hits. When a raycast detects a valid collider, it returns data pertaining to that hit and fires from the OnHit continuation output. If there is no valid hit, whether there were no colliders hit or the ones hit were not valid targets, the OnMiss continuation output fires.

The data output values are only valid for a given raycast hit for the duration of the impulse chain downstream of OnHit.

This node can be combined with the [Hit UV Coordinate](https://wiki.resonite.com/ProtoFlux:Hit_UV_Coordinate "ProtoFlux:Hit UV Coordinate") node to get further data from this hit, such as a 2D location point on the collider for example.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you want the same functionality as this node, but want to check for valid hits continuously, use [Raycaster](https://wiki.resonite.com/ProtoFlux:Raycaster "ProtoFlux:Raycaster") instead.


## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Performs a raycast with the input parameters when an impulse is received.

### Origin ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The starting position from which the ray is cast. Default is \[0;0;0\].

### Direction ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The direction in which the ray is cast. Default is \[0;0;0\] which results in no ray being cast. (Use for example \[0;0;1\] for directly forward.)

### MaxDistance ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The maximum distance the raycast should travel from its origin. Default is the maximum float value which is extremely high.

### HitTriggers ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Determines whether colliders with the Trigger, StaticTrigger or StaticTriggerAuto ColliderType value are valid hit targets. Default is False.

### UsersOnly ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Determines whether only user bone or simplified capsule colliders are valid targets. Default is False.

### DebugDuration ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

Determines the duration in seconds that a debug visual will be shown after each raycast. Default is -1 which disables the debug visual. When enabled, the visual shows a yellow line indicating the full path of the raycast along with the hit point (red spheres) and hit normal direction (blue arrows).

### Root ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot in whose coordinate space the Origin, Direction and MaxDistance values should be evaluated. Default is the world root slot, i.e. the values are treated as being in the [global coordinate space](https://wiki.resonite.com/Coordinate_spaces#Global_vs._Local "Coordinate spaces").

## Outputs

### OnHit ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires an impulse if a valid hit is found when performing a raycast.

### OnMiss ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires an impulse in any situation where a valid hit is not found when performing a raycast.

### HitCollider ( [ICollider](https://wiki.resonite.com/Type:ICollider "Type:ICollider"))

The first valid hit collider.

### HitDistance ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The distance from the Origin to the hit point in global coordinate space.

### HitPoint ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The global position at which the ray hit the collider.

### HitNormal ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The facing normal direction of the hit collider at the hit point.

### HitTriangleIndex ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The triangle index on the mesh corresponding to the hit collider. This value is 0 unless the HitCollider is a MeshCollider.

## Usage

There are a few ways in which the Raycast One node may not work as expected, particularly relating to directions and distances.

Firstly, the global scale of the input Root slot is taken into account when calculating a raycast's path. For example, assume that the Root slot input has global position \[0;0;0\] and global scale \[0.1;0.1;0.1\]; if the Origin input is \[0;0;0\], the raycast will start at global \[0;0;0\], however, if the Origin input is \[0;1;0\] the raycast will start at global \[0;0.1;0\] not global \[0;1;0\].
Similarly, the input Root slot's global scale affects the Direction vector and MaxDistance values too. With the same example input Root slot, a Direction of \[0;0;1\] and a MaxDistance of 1 result in a ray which travels only 0.1 units.

Secondly, the magnitude of the Direction vector affects the distance that the ray travels and the reported HitDistance output value. Assuming no input Root slot, a Direction input of \[0;0;1\] and MaxDistance of 1 will produce a ray 1 unit long. However, a Direction input of \[0;0;2\] and MaxDistance of 1 will produce a ray 2 units long. Additionally, the reported HitDistance value will be halved in the second case.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:RaycastOne&oldid=113250](https://wiki.resonite.com/index.php?title=ProtoFlux:RaycastOne&oldid=113250)"

Contents