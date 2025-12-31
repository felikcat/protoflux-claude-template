# ProtoFlux:ReadDynamicVariable

> Source: https://wiki.resonite.com/ProtoFlux:ReadDynamicVariable

Read Dynamic Variable

Source

FoundValue

Path

Value

Variables

The `Read Dynamic Variable` node takes in a [Slot](https://wiki.resonite.com/Slot "Slot") as a source and goes down the hierarchy to find the first [dynamic space](https://wiki.resonite.com/Component:DynamicVariableSpace "Component:DynamicVariableSpace") that contains the path specified. This returns the matching type's value if one is found. For more information, see [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables").

![](https://wiki.resonite.com/images/d/dd/InformationIcon.svg)

Although you cannot jump or skip variable spaces using this node from your provided string path, you can however use multiple of these nodes in conjunction together and provide more path strings to get to where you want to search for in the hierarchy (best showcased when using Slots as your returning value).


## Inputs

### Source ( [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot"))

This is the source slot that this node reads from. If the slot for this isn't provided, the engine will default the source slot to the slot of the node itself.

### Path ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The string input to find where to read from.

## Outputs

### FoundValue ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Whether the value we are searching for is found or not.

### Value (Generic)

The value that is found.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:ReadDynamicVariable&oldid=111823](https://wiki.resonite.com/index.php?title=ProtoFlux:ReadDynamicVariable&oldid=111823)"

Contents