# ProtoFlux:ReadCloudVariable

> Source: https://wiki.resonite.com/ProtoFlux:ReadCloudVariable

Read Cloud Variable

\*

OnRequest

Path

OnDone

VariableOwnerId

OnFail

Value

Cloud

Read Cloud Variable is a node that is able to read cloud variables that are already defined. For more information on how to define the permissions/security of cloud variables, and how to create them, see [Cloud Variables](https://wiki.resonite.com/Cloud_Variables "Cloud Variables")

## Inputs

### \\* ( [AsyncCall](https://wiki.resonite.com/Impulses\#ASync "Impulses"))

Will read from the cloud variable upon impulse. Is restricted by cloud variable rate limits.

### Path ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The definition owner + "." + The variable name.

Examples: "G-Resonite.UserSettings.Color.Primary", "U-ProbablePrime.testing.bool"

### VariableOwnerId ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The id of the person you want to read the value for the variable definition specified in Path.

Examples: "U-Frooxius", "U-Nexulan"

## Outputs

### OnRequest ( [SyncResumption](https://wiki.resonite.com/Impulses\#Async "Impulses"))

Sent when the node has sent the request for the value to be read. This can be used to chain more asynchronous calls together to happen in parallel like more reading from other variable definitions.

### OnDone ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

The impulse during which Value will have the read data.

### OnFail ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

The impulse caused if the variable hit an error. including but not limited to: Invalid Path, improper permissions for the variable definition in Path, Invalid userID, UserID has not made a definition for the variable definition in Path.

### Value (Pseudo-generic)

The value you read for the user in VariableOwnerID in the variable definition defined in Path. This only exists during the OnDone Impulse. Write the output to a [Data Model Store](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store") to keep it for longer than the impulse.

Examples: [ColorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"), [float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"), [String](https://wiki.resonite.com/Type:String "Type:String"), [DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime").

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ReadCloudVariable&oldid=110557](https://wiki.resonite.com/index.php?title=ProtoFlux:ReadCloudVariable&oldid=110557)"

Contents