# ProtoFlux:WriteOrCreateDynamicVariable

> Source: https://wiki.resonite.com/ProtoFlux:WriteOrCreateDynamicVariable

Write Or Create Dynamic Variable

\*

OnFound

Target

OnCreated

Path

OnFailed

CreateDirectlyOnTarget

CreateNonPersistent

Value

Variables

Write Or Create Dynamic Variable is a ProtoFlux node that is able to create or find previously created dynamic variables under a slot. For more info on Dynamic Variables, see [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables"). This node will only attach the variable if `Path` were to be used on the slot it's attaching to would be able to bind. Otherwise the dynamic variable will not be created and it will impulse `OnFailed`.

For an example, if you are reading a gigantic string of data from an API like a blog post, and it gives you something like:

```
{
  "date":"4/5/2020",
  "poster":"josh",
  "text":"I caught a fish",
  "comments":{
    "898dw3juez":{
      "poster":"Jared",
      "text":"This is cool!"
    }
  }
}
```

assuming you have already read this with protoflux reliably, how would you store this into a data you could read? Well using create or write dynamic variables, you can create a dynamic variable list by having a dynamic variable space named `PostViewer` and then write a bunch of variables. The variables for the above data could be written as follows:

`PostViewer/Post.Date`

`PostViewer/Post.Poster`

`PostViewer/Post.Text`

`PostViewer/Comments.898dw3juez.poster`

`PostViewer/Comments.898dw3juez.text`

then using [Read Dynamic Variable](https://wiki.resonite.com/ProtoFlux:Read_Dynamic_Variable "ProtoFlux:Read Dynamic Variable") this information can be read. Note the dots allow the variables to follow the allows naming schema but act as separators for different data under the variable space. Reading such data can be done by concatinating strings together with dots in between like one would do with a path and slashes.

## Inputs

### Target ( [Slot](https://wiki.resonite.com/Type:Slot "Type:Slot"))

The slot to search for a dynamic variable space from to put the variable into

### Path ( [String](https://wiki.resonite.com/Type:String "Type:String"))

The path for the created dynamic variable. To see how this influences attaching see the paragraph at the beginning of this page.

### CreateDirectlyOnTarget ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Whether to attach the new dynamic variable when created to the slot the dynamic variable space component is on (false) or directly on the slot specified on `Target` (true)

### CreateNonPersistent ( [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

If true, this will make the created dynamic value variable non-persistent.

### Value (Generic)

Any type of value, reference, or object that the variable should store.

See also: [#1254](https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/1254)

## Outputs

### OnFound ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when `*` is fired and `FindExisting` is true and a variable already exists that can be read through `Target`

### OnCreated ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when `*` is fired and a variable has been created because either `FindExisting` was false, or the variable didn't exist before. This will only create the variable if it can bind, which is explained on the [Dynamic Variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") page.

### OnFailed ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when `*` is fired and the variable would not able to bind when created at `Target`. The variable was not created when this impulses.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:WriteOrCreateDynamicVariable&oldid=111825](https://wiki.resonite.com/index.php?title=ProtoFlux:WriteOrCreateDynamicVariable&oldid=111825)"

Contents