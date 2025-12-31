# ProtoFlux:StartAsyncTask

> Source: https://wiki.resonite.com/ProtoFlux:StartAsyncTask

Start Async Task

\*

TaskStart

OnStarted

OnFailed

Async

The **Start Async Task** node starts a new [ExecutionContext](https://wiki.resonite.com/ExecutionContext "ExecutionContext") using [async flow](https://wiki.resonite.com/Async_flow "Async flow") at the current impulse.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Start the async task.

## Outputs

### TaskStart ( [AsyncResumption](https://wiki.resonite.com/Impulses\#ASync "Impulses"))

The new ExecutionContext made by the node. This impulse chain is [async](https://wiki.resonite.com/Async "Async") and will run until it encounters any sort of delay, at which it will continue execution along the `OnStarted` chain and follow standard sync/async flow.

The context made by this node is _nested_, meaning that any context-specific things, such as [locals](https://wiki.resonite.com/ProtoFlux:Local "ProtoFlux:Local"), are duplicated from the context that `*` comes from. Any future changes to context-specific things will not be reflected in the `OnStarted` chain and vice versa.

### OnStarted ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires once `TaskStart` encounters any sort of delay, effectively running at the same time given the now-separate contexts.

### OnFailed ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires if the task was unable to be started. This only fires if `TaskStart` is not connected to any node.

## See Also

- [Impulses#Async](https://wiki.resonite.com/Impulses#Async "Impulses") for more information about async flow.
- [ExecutionContext](https://wiki.resonite.com/ExecutionContext "ExecutionContext") for more information about the context this node creates.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:StartAsyncTask&oldid=110765](https://wiki.resonite.com/index.php?title=ProtoFlux:StartAsyncTask&oldid=110765)"

Contents