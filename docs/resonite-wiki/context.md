# Context

In [ProtoFlux](https://wiki.resonite.com/ProtoFlux), the **context** of any given node group determines many factors on how the ProtoFlux is internally processed. A few things that context will affect include how control flow is handled, what concepts the ProtoFlux is aware of, and how the ProtoFlux interacts with FrooxEngine, if at all.

There is only one baseline context available for ProtoFlux nodes, that being the ExecutionContext. There exist extensions to this context, with the only one being FrooxEngineContext. More contexts are to be expected in the future, such as a state machine context, an audio DSP context, and a shader context.

## ExecutionContext

The **ExecutionContext** context mirrors traditional [imperative programming](https://en.wikipedia.org/wiki/Imperative_programming). As of the time of writing, all ProtoFlux is under this context.

ExecutionContext is the most basic context for control flow in ProtoFlux. It establishes the concept of [impulses](impulses.md) (along with async control flow) and writes (but only to a ProtoFlux-specific value store, such as a Local or Store).

### FrooxEngineContext

The **FrooxEngineContext** context is an extension of the ExecutionContext that is aware of FrooxEngine. This allows nodes to interact with the data model by drives and writes to a field. FrooxEngineContext graphs are aware of:

- The **local user** executing the node
- The **IWorldElements** existing in a world
- The **world** and **session** themselves
- How to interface all of these concepts with ProtoFlux

## Context Types Summary

| Context | Description |
|---------|-------------|
| ExecutionContext | Basic imperative programming context with impulses and writes to ProtoFlux stores |
| FrooxEngineContext | Extension that enables interaction with FrooxEngine data model, drives, and world elements |

## Future Contexts

More contexts are planned for the future:
- State machine context
- Audio DSP context
- Shader context

Source: https://wiki.resonite.com/Context
