# ProtoFlux:DataModelBooleanToggle

> Source: https://wiki.resonite.com/ProtoFlux:DataModelBooleanToggle

Boolean Latch

Set

Set

Reset

Reset

Toggle

\*

Flow

The **Data Model Boolean Toggle** or **Boolean Latch** is a node that can be pulsed to toggle a Data Model Boolean between true and false.

![](https://wiki.resonite.com/images/d/dd/InformationIcon.svg)

Data Model Boolean Toggle is a [Data Model Store](https://wiki.resonite.com/ProtoFlux:Data_Model_Store "ProtoFlux:Data Model Store") with impulses to set, reset and toggle itself. This means you can use a [Write](https://wiki.resonite.com/ProtoFlux:Write "ProtoFlux:Write") to change the value directly if you input the \* bool into the [Write](https://wiki.resonite.com/ProtoFlux:Write "ProtoFlux:Write")'s Variable field.


## Inputs

### Set ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Set the state to True.

### Reset ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Set the state to False.

### Toggle ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Toggle the state to the opposite state.

## Outputs

### OnSet ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when Set is pulsed or Toggle has switched the state to True.

### OnReset ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when Reset is pulsed or Toggle has switched the state to False.

### \\* ( [bool](https://wiki.resonite.com/Types:Bool "Types:Bool"))

The current state.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:DataModelBooleanToggle&oldid=109597](https://wiki.resonite.com/index.php?title=ProtoFlux:DataModelBooleanToggle&oldid=109597)"

Contents