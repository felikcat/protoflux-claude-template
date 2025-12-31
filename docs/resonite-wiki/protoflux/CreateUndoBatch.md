# ProtoFlux:CreateUndoBatch

> Source: https://wiki.resonite.com/ProtoFlux:CreateUndoBatch

Create Undo Batch

\*

Create

Description

OnCreated

Undo

The **Create Undo Batch** node Begins an undo batch, executes the Create call, then ends the undo batch all in one frame.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Calls an impulse to create an undo batch.

### Description ( [String](https://wiki.resonite.com/String "String"))

The description for this undo batch. The description will be automatically prepended with "Undo" in bigger text in the context menu.

## Outputs

### Create ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

The impulse created when the undo batch is started but not ended.

### OnCreated ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

The impulse created after the undo batch is ended.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:CreateUndoBatch&oldid=109593](https://wiki.resonite.com/index.php?title=ProtoFlux:CreateUndoBatch&oldid=109593)"

Contents