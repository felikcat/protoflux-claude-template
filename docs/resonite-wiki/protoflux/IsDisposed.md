# ProtoFlux:IsDisposed

> Source: https://wiki.resonite.com/ProtoFlux:IsDisposed

Is Disposed

Element

\*

Elements

The `Is Disposed` node takes in a [worker world element](https://wiki.resonite.com/index.php?title=Type:Worker&action=edit&redlink=1 "Type:Worker (page does not exist)") and returns if that element was disposed from the world. Destruction of the slot prevents the result from changing, as by the time the slot is gone, it is too late. There is however a method to check if something did get disposed, see the examples below.

## Inputs

### Element ( [Worker](https://wiki.resonite.com/index.php?title=Type:Worker&action=edit&redlink=1 "Type:Worker (page does not exist)"))

The worker world element in question.

## Outputs

### \\* ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Returns if this element was disposed in this world.

## Examples

There is a certain setup required to detect when a slot gets disposed, here is what you need and why:

- A [Slot](https://wiki.resonite.com/Slot "Slot") that holds 2 components, a [Dynamic Variable Space](https://wiki.resonite.com/Component:DynamicVariableSpace "Component:DynamicVariableSpace") component and a [Dynamic Reference Variable](https://wiki.resonite.com/Component:DynamicReferenceVariable "Component:DynamicReferenceVariable") component (we will use the [Reference Type](https://wiki.resonite.com/Reference_Type "Reference Type") of a Worker). This will listen for any changes that happen.
- A [Dynamic Variable Input](https://wiki.resonite.com/ProtoFlux:Dynamic_Variable_Input "ProtoFlux:Dynamic Variable Input") node. Must be parented under the slot that is listening using the Dynamic Variable Space.
- This **IsDisposed** node, used to check if some element was disposed.
- A [Continuously Changing Relay](https://wiki.resonite.com/ProtoFlux:Continuously_Changing_Relay "ProtoFlux:Continuously Changing Relay") node, used to make sure it updates our value.
- A [Fire On True](https://wiki.resonite.com/ProtoFlux:Fire_On_True "ProtoFlux:Fire On True") node. We want to know when the element gets disposed at this exact moment.
- A [Host User](https://wiki.resonite.com/ProtoFlux:Host_User "ProtoFlux:Host User") or [Local User](https://wiki.resonite.com/ProtoFlux:Local_User "ProtoFlux:Local User") node, used for the Fire On True node.

With this setup, and when the target slot is destroyed (and there is no longer any references to it), the **DynamicReferenceVariable** component will still have it stored on its field, showing the old ID along with it. This in turn makes the **IsDisposed** set to `true`.

- [![IsDisposed Node Example 01](https://wiki.resonite.com/images/thumb/a/ab/IsDisposed_Node_Example_01.png/437px-IsDisposed_Node_Example_01.png)](https://wiki.resonite.com/File:IsDisposed_Node_Example_01.png "IsDisposed Node Example 01")

IsDisposed Node Example 01


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:IsDisposed&oldid=110111](https://wiki.resonite.com/index.php?title=ProtoFlux:IsDisposed&oldid=110111)"

Contents