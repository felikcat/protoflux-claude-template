# ProtoFlux:HitUVCoordinate

> Source: https://wiki.resonite.com/ProtoFlux:HitUVCoordinate

ProtoFlux Node

HitCollider

UV

HitTriangleIndex

IsValidUV

HitPoint

Physics

The `Hit UV Coordinate` node requires an [ICollider](https://wiki.resonite.com/Type:ICollider "Type:ICollider") to work, and returns if we hit anything and the UV coordinates of what we hit.

## Usage

This node is used frequently with [Raycaster](https://wiki.resonite.com/ProtoFlux:Raycaster "ProtoFlux:Raycaster") and [Raycast One](https://wiki.resonite.com/ProtoFlux:Raycast_One "ProtoFlux:Raycast One"), as well as applications requiring lasers, pointers, or clicking on screens or mouse clicks and desktop-based gadgets.

## Inputs

### HitCollider ( [ICollider](https://wiki.resonite.com/Type:ICollider "Type:ICollider"))

The collider we just hit.

### HitTriangleIndex ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The numbered triangle in this mesh.

### HitPoint ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The point where we want to hit.

## Outputs

### UV ( [float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))

The point we hit on this surface of this mesh, giving the result as a UV coordinate.

### IsValidUV ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Check if we actually hit a valid collider to get the UV information.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:HitUVCoordinate&oldid=109999](https://wiki.resonite.com/index.php?title=ProtoFlux:HitUVCoordinate&oldid=109999)"

Contents