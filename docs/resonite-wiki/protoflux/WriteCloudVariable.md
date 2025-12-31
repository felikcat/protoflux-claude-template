# ProtoFlux:WriteCloudVariable

> Source: https://wiki.resonite.com/ProtoFlux:WriteCloudVariable

Write Cloud Variable

\*

OnRequest

Path

OnDone

VariableOwnerId

OnFail

Value

Cloud

Write Cloud Variable is a node that is able to write to cloud variables that are already defined. For more information on how to define the permissions/security of cloud variables, and how to create them, see [Cloud Variables](https://wiki.resonite.com/Cloud_Variables "Cloud Variables")

## Inputs

### \\* ( [AsyncCall](https://wiki.resonite.com/Impulses\#ASync "Impulses"))

Will Write the cloud variable upon impulse. Is restricted by cloud variable rate limits.

### Path ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The definition owner + "." + The variable name.

Examples: "G-Resonite.UserSettings.Color.Primary", "U-ProbablePrime.testing.bool"

### VariableOwnerId ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The id of the person writing a value to the variable specified in Path.

Examples: "U-Frooxius", "U-Nexulan"

### Value (Pseudo-generic)

The value you want to write to this cloud variable.

Examples: [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"), [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"), [String](https://wiki.resonite.com/Type:String "Type:String"), [DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime").

## Outputs

### OnRequest ( [SyncResumption](https://wiki.resonite.com/Impulses\#Async "Impulses"))

An async impulse sent when the node has sent the request for the value to be written. This can be used to chain more asynchronous calls together to happen in parallel like more writing to other variable definitions.

### OnDone ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

The impulse during which Value will have written the data.

### OnFail ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

The impulse caused if the variable hit an error. including but not limited to: Invalid Path, improper permissions for the variable definition in Path, Invalid userID.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:WriteCloudVariable&oldid=111165](https://wiki.resonite.com/index.php?title=ProtoFlux:WriteCloudVariable&oldid=111165)"

Contents