# ProtoFlux:SampleSpatialVariable

> Source: https://wiki.resonite.com/ProtoFlux:SampleSpatialVariable

Sample SpatialVar

Point

\*

Name

DefaultValue

Spatial

The **Sample Spatial Variable** node takes in a point in [3D space](https://wiki.resonite.com/Slot_transforms "Slot transforms"), a name that matches that space, and a default value if that space cannot be found, then returns the value found in the space, otherwise it will return the default value.

This node works with [spatial variable](https://wiki.resonite.com/Spatial_variables "Spatial variables") components, and will need a [BoxConstantValueSpatialVariable](https://wiki.resonite.com/Component:BoxConstantValueSpatialVariable "Component:BoxConstantValueSpatialVariable") or similar to function as expected.

## Inputs

### Point ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The point to check in global 3D space.

### Name ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The named space/area to look for.

### DefaultValue (Pseudo-Generic)

If a named space cannot be found, use this value.

## Outputs

### \\* (Pseudo-Generic)

Returns the value found in this space/area, otherwise return the default value.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:SampleSpatialVariable&oldid=110637](https://wiki.resonite.com/index.php?title=ProtoFlux:SampleSpatialVariable&oldid=110637)"

Contents