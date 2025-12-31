# ProtoFlux:Raycaster

> Source: https://wiki.resonite.com/ProtoFlux:Raycaster

Raycaster

Origin

HasHit

Direction

HitCollider

MaxDistance

HitDistance

HitTriggers

HitPoint

UsersOnly

HitNormal

Root

HitTriangleIndex

Physics

The **Raycaster** node performs a raycast check every update, essentially acting as a constant raycast. The input parameters determine from where, in what direction, and how far the ray should be cast as well as determining which colliders are valid hits. When a raycast detects a valid collider, it returns data pertaining to that hit from the node outputs.

This node can be combined with the [Hit UV Coordinate](https://wiki.resonite.com/ProtoFlux:Hit_UV_Coordinate "ProtoFlux:Hit UV Coordinate") node to get further data from this hit, such as a 2D location point on the collider for example. Since this node returns data per frame, it can be very useful for debugging and testing raycast hit detection.

![](https://wiki.resonite.com/images/c/c1/SuggestionIcon.svg)

If you want the same functionality as this node, but want to control when it checks for valid hits, use [Raycast One](https://wiki.resonite.com/ProtoFlux:Raycast_One "ProtoFlux:Raycast One") instead.


## Inputs

### Origin ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The starting position from which the ray is cast. Default is \[0;0;0\].

### Direction ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The direction in which the ray is cast. Default is \[0;0;0\] which results in no ray being cast.

### MaxDistance ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The maximum distance the raycast should travel from its origin. Default is the maximum float value which is extremely high.

### HitTriggers ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Determines whether colliders with the Trigger, StaticTrigger or StaticTriggerAuto ColliderType value are valid hit targets. Default is False.

### UsersOnly ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Determines whether only user bone or simplified capsule colliders are valid targets. Default is False.

### Root ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot in whose coordinate space the Origin, Direction and MaxDistance values should be evaluated. Default is the world root slot, i.e. the values are treated as being in the [global coordinate space](https://wiki.resonite.com/Coordinate_spaces#Global_vs._Local "Coordinate spaces").

## Outputs

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

There are a few ways in which the Raycaster node may not work as expected, particularly relating to directions and distances.

Firstly, the global scale of the input Root slot is taken into account when calculating a raycast's path. For example, assume that the Root slot input has global position \[0;0;0\] and global scale \[0.1;0.1;0.1\]; if the Origin input is \[0;0;0\], the raycast will start at global \[0;0;0\], however, if the Origin input is \[0;1;0\] the raycast will start at global \[0;0.1;0\] not global \[0;1;0\].
Similarly, the input Root slot's global scale affects the Direction vector and MaxDistance values too. With the same example input Root slot, a Direction of \[0;0;1\] and a MaxDistance of 1 result in a ray which travels only 0.1 units.

Secondly, the magnitude of the Direction vector affects the distance that the ray travels and the reported HitDistance output value. Assuming no input Root slot, a Direction input of \[0;0;1\] and MaxDistance of 1 will produce a ray 1 unit long. However, a Direction input of \[0;0;2\] and MaxDistance of 1 will produce a ray 2 units long. Additionally, the reported HitDistance value will be halved in the second case.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:Raycaster&oldid=103534](https://wiki.resonite.com/index.php?title=ProtoFlux:Raycaster&oldid=103534)"

Contents