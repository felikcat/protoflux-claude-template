# ProtoFlux:SampleMinMaxSpatialVariable

> Source: https://wiki.resonite.com/ProtoFlux:SampleMinMaxSpatialVariable

Sample Min/Max SpatialVar

Point

Min

Name

Max

FoundAny

Spatial

The **Sample Min Max Spatial Variable** node takes in a point in [3D space](https://wiki.resonite.com/Slot_transforms "Slot transforms"), and a name that matches that space, then returns the values found in the space that defined a min and max range.

This node works with [spatial variable](https://wiki.resonite.com/Spatial_variables "Spatial variables") components, and will need a [BoxConstantValueSpatialVariable](https://wiki.resonite.com/Component:BoxConstantValueSpatialVariable "Component:BoxConstantValueSpatialVariable") or similar to function as expected.

## Inputs

### Point ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The point to check in global 3D space.

### Name ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The named space/area to look for.

## Outputs

### Min (Pseudo-Generic)

Returns the min value found in this space/area.

### Max (Pseudo-Generic)

Returns the max value found in this space/area.

### FoundAny ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Returns if there is a matching space/area at all.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:SampleMinMaxSpatialVariable&oldid=110631](https://wiki.resonite.com/index.php?title=ProtoFlux:SampleMinMaxSpatialVariable&oldid=110631)"

Contents