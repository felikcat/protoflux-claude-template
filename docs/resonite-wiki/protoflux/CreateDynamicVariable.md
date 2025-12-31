# ProtoFlux:CreateDynamicVariable

> Source: https://wiki.resonite.com/ProtoFlux:CreateDynamicVariable

Create Dynamic Variable

\*

OnNotFound

Target

OnCreated

Path

OnAlredyExists

CreateDirectlyOnTarget

OnFailed

CreateNonPersistent

InitialValue

Variables

Create Dynamic Variable is a ProtoFlux node that is able to create dynamic variables under a slot. For more info on Dynamic Variables, see [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables"). This node will only attach the variable if `Path` were to be used on the slot it's attaching to would be able to bind. Otherwise the dynamic variable will not be created and it will impulse `OnNotFound`.

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

Keep in mind that the top most output is **OnNotFound**. This can be confusing (especially if you're not paying attention when connecting nodes) when the code fires and nothing happens.


## Inputs

### Target ( [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot"))

The slot to search for a dynamic variable space from to put the variable into

### Path ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The path for the created dynamic variable. To see how this influences attaching see the paragraph at the beginning of this page.

### CreateDirectlyOnTarget ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Whether to attach the new dynamic variable when created to the slot the dynamic variable space component is on (false) or directly on the slot specified on `Target` (true)

### CreateNonPersistent ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

If true, this will create the dynamic variable component with disabled `Persistent>`.

### InitialValue (Generic)

Any type of value, reference, or object that the variable should store.

See also: [#1254](https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/1254)

## Outputs

### OnNotFound ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when `*` is fired and the variable would not able to bind when created at `Target`. The variable was not created when this impulses.

### OnCreated ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when `*` is fired and a variable has been created and the variable didn't exist before. This will only create the variable if it can bind, which is explained on the [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") page.

### OnAlredyExists ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when `*` is fired and a variable already exists with same `Path`.

### OnFailed ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when `*` is fired and `InitialValue` it's local element.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:CreateDynamicVariable&oldid=111819](https://wiki.resonite.com/index.php?title=ProtoFlux:CreateDynamicVariable&oldid=111819)"

Contents