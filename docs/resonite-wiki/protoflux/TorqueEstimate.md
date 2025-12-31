# ProtoFlux:TorqueEstimate

> Source: https://wiki.resonite.com/ProtoFlux:TorqueEstimate

Torque Estimate

InitialTorque

\*

Drag

Time

Physics

The **Torque Estimate** node takes in the initial torque, drag resistance, and the amount of time it is simulating, then returns the torque simulation value (as a [floatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")) that object will rotate in.

## Inputs

### InitialTorque ( [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))

The amount of push for this torque.

### Drag ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The amount of resistance for this torque.

### Time ( [float](https://wiki.resonite.com/Type:Float "Type:Float"))

The time in between the initial torque and now.

## Outputs

### \\* ( [floatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ"))

Returns the estimated torque within that time period.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:TorqueEstimate&oldid=110863](https://wiki.resonite.com/index.php?title=ProtoFlux:TorqueEstimate&oldid=110863)"

Contents