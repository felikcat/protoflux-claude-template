# ProtoFlux:ComputeBoundingBox

> Source: https://wiki.resonite.com/ProtoFlux:ComputeBoundingBox

Compute Bounding Box

Instance

\*

IncludeInactive

CoordinateSpace

OnlyWithTag

Bounds

The **Compute Bounding Box** node calculates a bounding box for the input Instance slot hierarchy in the input CoordinateSpace with optional filtering for inactive and/or tagged slots.

Only components which implement the `IBounded` interface are used for bounding box calculation. These include: [Bounds](https://wiki.resonite.com/Component:Bounds "Component:Bounds"), [MeshRenderers](https://wiki.resonite.com/Component:MeshRenderer "Component:MeshRenderer"), [SkinnedMeshRenderers](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer"), [TextRenderers](https://wiki.resonite.com/Component:TextRenderer "Component:TextRenderer"), [UIX Canvases](https://wiki.resonite.com/Component:Canvas "Component:Canvas"), [CharacterControllers](https://wiki.resonite.com/Component:CharacterController "Component:CharacterController") and all [Colliders](https://wiki.resonite.com/Collider "Collider").

## Inputs

### Instance ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot for whose hierarchy a bounding box is calculated.

### IncludeInactive ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Determines whether inactive parts of the hierarchy are included when calculating the bounding box. Default is False which means that inactive slots and their children are ignored.

### CoordinateSpace ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot relative to whose coordinate space the bounding box is calculated. Default is null which results in the bounding box being calculated in [global coordinate space](https://wiki.resonite.com/Coordinate_spaces#Global_vs._Local "Coordinate spaces").

### OnlyWithTag ( [String](https://wiki.resonite.com/Type:String "Type:String"))

If specified, only slots with the given tag are included in the bounding box calculation. Default is null, which results in no filtering by tag. Unlike the handling of IncludeInactive, child slots with a matching tag are included even if their parent slot(s) are not tagged.

## Outputs

### \\* ( [BoundingBox](https://wiki.resonite.com/Type:BoundingBox "Type:BoundingBox"))

The calculated bounding box. Default is an empty bounding box if the Instance input is null or if there are no IBounded components present in it's hierarchy on slots which pass the filtering conditions.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ComputeBoundingBox&oldid=109555](https://wiki.resonite.com/index.php?title=ProtoFlux:ComputeBoundingBox&oldid=109555)"

Contents