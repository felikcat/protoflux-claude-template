# ProtoFlux:TransformBounds

> Source: https://wiki.resonite.com/ProtoFlux:TransformBounds

Transform Bounds

Bounds

\*

SourceSpace

TargetSpace

Bounds

The **Transform Bounds** node transforms the input bounding box from the [local coordinate space](https://wiki.resonite.com/Coordinate_spaces#Global_vs._Local "Coordinate spaces") of the SourceSpace slot to that of the TargetSpace slot.

## Inputs

### Bounds ( [BoundingBox](https://wiki.resonite.com/Type:BoundingBox "Type:BoundingBox"))

The bounding box is to be transformed. Default is a bounding box with center \[0;0;0\] and size \[0;0;0\].

### SourceSpace ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot in whose local coordinate space the Bounds are interpreted. Default is null, which results in the global coordinate space being used.

### TargetSpace ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot in whose local coordinate space the Bounds are transformed. Default is null, which results in the global coordinate space being used.

## Outputs

### \\* ( [BoundingBox](https://wiki.resonite.com/Type:BoundingBox "Type:BoundingBox"))

The transformed bounding box.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:TransformBounds&oldid=110871](https://wiki.resonite.com/index.php?title=ProtoFlux:TransformBounds&oldid=110871)"

Contents