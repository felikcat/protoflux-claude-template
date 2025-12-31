# ProtoFlux:SetTRS

> Source: https://wiki.resonite.com/ProtoFlux:SetTRS

Set TRS

\*

Next

Instance

TRS

Transform

The **Set TRS** node takes in a slot to transform (position, rotation, and scale) in 3D space along with the matrix value. Unlike [Set Global Transform Matrix](https://wiki.resonite.com/ProtoFlux:Set_Global_Transform_Matrix "ProtoFlux:Set Global Transform Matrix"), this node sets the slot's local transform value.

To create a transform matrix, the [ProtoFlux Matrix Catagory](https://wiki.resonite.com/Category:ProtoFlux:Operators:Matrix "Category:ProtoFlux:Operators:Matrix") has many helpful nodes to do this.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Calls an impulse to set the the slot position, rotation, and scale of a slot.

### Instance ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot to transform.

### TRS ( [float4x4](https://wiki.resonite.com/Type:Float4x4 "Type:Float4x4"))

The exact value to set the slot's transform.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Continues the flow of execution from here.

## See Also

- Wikipedia's definition of a [matrix](https://en.wikipedia.org/wiki/Matrix_(mathematics)).

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:SetTRS&oldid=110731](https://wiki.resonite.com/index.php?title=ProtoFlux:SetTRS&oldid=110731)"

Contents