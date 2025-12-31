# ProtoFlux:SampleNumericSpatialVariable

> Source: https://wiki.resonite.com/ProtoFlux:SampleNumericSpatialVariable

Sample Numeric SpatialVar

Point

\*

Name

Mode

BaseValue

Spatial

The **Sample Numeric Spatial Variable** node takes in a point in [3D space](https://wiki.resonite.com/Slot_transforms "Slot transforms"), a name that matches that space, a priority mode, and a default (base) value if that space cannot be found, then returns the (weighted) value found in the space, otherwise it will return the default value.

This node works with [spatial variable](https://wiki.resonite.com/Spatial_variables "Spatial variables") components, and will need a [BoxConstantValueSpatialVariable](https://wiki.resonite.com/Component:BoxConstantValueSpatialVariable "Component:BoxConstantValueSpatialVariable") or similar to function as expected.

## Inputs

### Point ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The point to check in global 3D space.

### Name ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The named space/area to look for.

### Mode ( [ValueSpatialVariableMode](https://wiki.resonite.com/Type:ValueSpatialVariableMode "Type:ValueSpatialVariableMode"))

The priority mode used to determine the value of this sample. (`HighestPriority`, `WeightedAverage`, `PrioritySortedBlend`, or `Additive`)

### BaseValue (Pseudo-Generic)

If a named space cannot be found, use this value.

## Outputs

### \\* (Pseudo-Generic)

Returns the value found in this space/area, otherwise return the default (base) value.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:SampleNumericSpatialVariable&oldid=110633](https://wiki.resonite.com/index.php?title=ProtoFlux:SampleNumericSpatialVariable&oldid=110633)"

Contents