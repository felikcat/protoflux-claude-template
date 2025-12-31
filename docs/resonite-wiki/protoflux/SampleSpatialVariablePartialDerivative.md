# ProtoFlux:SampleSpatialVariablePartialDerivative

> Source: https://wiki.resonite.com/ProtoFlux:SampleSpatialVariablePartialDerivative

Sample SpatialVar Partial Derivative

Point

X

Orientation

Y

Name

Z

Mode

BaseValue

SamplingDistance

Spatial

The **SampleSpatialVariablePartialDerivative** node samples a numerical [spatial variable](https://wiki.resonite.com/Spatial_variable "Spatial variable") and returns the [partial derivatives](https://en.wikipedia.org/wiki/Partial_derivative) of the variable in the x, y, and z directions according to an orientation. In essence, it computes the numerical [gradient](https://en.wikipedia.org/wiki/Gradient) of the sampled spatial variable.

## Inputs

### Point ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The point at which to sample the spatial variable. This point is in [global space](https://wiki.resonite.com/Global_space "Global space").

### Orientation ( [floatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ"))

The orientation that the partial derivatives will be calculated in. This essentially defines the coordinate space of the calculation.

### Name ( [string](https://wiki.resonite.com/Type:String "Type:String"))

The name of the spatial variable to sample.

### Mode ( [ValueSpatialVariableMode](https://wiki.resonite.com/Type:ValueSpatialVariableMode "Type:ValueSpatialVariableMode"))

If multiple spatial variables of the same name and type exist at the sampled point, this input will determine how the value of the spatial variable will be calculated.

### BaseValue (Generic)

If a spatial variable does not exist at the point or at any of the partial derivative calculation points, this value will be substituted instead.

### SamplingDistance ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The length of sample that the partial derivative calculation will use. The calculation will sample the spatial variable at a distance of `SamplingDistance / 2` in each direction for each axis.

## Outputs

### X (Generic)

The partial derivative in the X direction.

### Y (Generic)

The partial derivative in the Y direction.

### Z (Generic)

The partial derivative in the Z direction.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:SampleSpatialVariablePartialDerivative&oldid=113489](https://wiki.resonite.com/index.php?title=ProtoFlux:SampleSpatialVariablePartialDerivative&oldid=113489)"