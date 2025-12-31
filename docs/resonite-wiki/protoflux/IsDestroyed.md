# ProtoFlux:IsDestroyed

> Source: https://wiki.resonite.com/ProtoFlux:IsDestroyed

Is Destroyed

Element

\*

Elements

The `Is Destroyed` node takes in a [destroyable world element](https://wiki.resonite.com/Type:IDestroyable "Type:IDestroyable") and returns if that element was destroyed from the world. Destruction of the slot prevents the result from changing, as by the time the slot is gone, it is too late. There is however a method to check if something did get destroyed, see the examples below.

## Inputs

### Element ( [IDestroyable](https://wiki.resonite.com/Type:IDestroyable "Type:IDestroyable"))

The destroyable world element in question.

## Outputs

### \\* ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Returns if this element was destroyed in this world.

## Examples

There is a certain setup required to detect when a slot gets destroyed, here is what you need and why:

- A [Slot](https://wiki.resonite.com/Slot "Slot") that holds 2 components, a [Dynamic Variable Space](https://wiki.resonite.com/Component:DynamicVariableSpace "Component:DynamicVariableSpace") component and a [Dynamic Reference Variable](https://wiki.resonite.com/Component:DynamicReferenceVariable "Component:DynamicReferenceVariable") component (we will use the [Reference Type](https://wiki.resonite.com/Reference_Type "Reference Type") of an IDestroyable). This will listen for any changes that happen.
- A [Dynamic Variable Input](https://wiki.resonite.com/ProtoFlux:Dynamic_Variable_Input "ProtoFlux:Dynamic Variable Input") node. Must be parented under the slot that is listening using the Dynamic Variable Space.
- This **IsDestroyed** node, used to check if some element was destroyed.
- A [Continuously Changing Relay](https://wiki.resonite.com/ProtoFlux:Continuously_Changing_Relay "ProtoFlux:Continuously Changing Relay") node, used to make sure it updates our value.
- A [Fire On True](https://wiki.resonite.com/ProtoFlux:Fire_On_True "ProtoFlux:Fire On True") node. We want to know when the element gets destroyed at this exact moment.
- A [Host User](https://wiki.resonite.com/ProtoFlux:Host_User "ProtoFlux:Host User") or [Local User](https://wiki.resonite.com/ProtoFlux:Local_User "ProtoFlux:Local User") node, used for the Fire On True node.

With this setup, and when the target slot is destroyed (and there is no longer any references to it), the **DynamicReferenceVariable** component will still have it stored on its field, showing the old ID along with it. This in turn makes the **IsDestroyed** set to `true`.

- [![IsDestroyed Node Example 01](https://wiki.resonite.com/images/thumb/6/60/IsDestroyed_Node_Example_01.png/437px-IsDestroyed_Node_Example_01.png)](https://wiki.resonite.com/File:IsDestroyed_Node_Example_01.png "IsDestroyed Node Example 01")

IsDestroyed Node Example 01


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:IsDestroyed&oldid=110107](https://wiki.resonite.com/index.php?title=ProtoFlux:IsDestroyed&oldid=110107)"

Contents