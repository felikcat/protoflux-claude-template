<!--
Source: https://flux-sdk.samsmucny.com/ProtoGraph/Getting-Started.html
License: CC BY-NC-SA 4.0
Author: Sam (Papaltine) Smucny
-->

# Getting Started

## Installation

1. **Install the .NET SDK**: Install the [dotnet (.NET) SDK](https://dotnet.microsoft.com/en-us/download). Run `dotnet --info` to verify you have a .NET 10.X (or greater) SDK installed (Make sure you have the SDK, not just the runtime).

2. **Install Flux SDK**: Install the dotnet tool [Papaltine.FluxSDK](https://www.nuget.org/packages/Papaltine.FluxSDK):
   ```
   dotnet tool install --global --version <version_number> Papaltine.FluxSDK
   ```

3. **Find Resonite DLL folder**: It should be located under `Resonite` inside of the Steam installation. There are several ways you can point to the DLLs:

   - If it is in a normal installation location, flux-sdk may find it automatically. If you can run `flux-sdk froox-docs --out protoflux-nodes.yaml` successfully then you're all good!
   - Set the `RESONITE_MANAGED_DATA_PATH` system environment variable to the directory of the Resonite managed data
   - Use the -L/--library-path command line argument each time when you run the compiler

### Optional: IDE Setup

Flux SDK provides an LSP compatible language server, and a VSCode compatible extension is available on the marketplace with the name [ProtoGraph](https://marketplace.visualstudio.com/items?itemName=papaltine.protograph).

> The LSP setup will also allow you to share your ProtoGraph code to Resonite in real time using Code Share.

## Writing your First Program

Create a new file called `HelloWorld.pg` and add the following to it:

```
module HelloWorld
where {
    display("Hello World!")
}
```

In this file we are creating a new module called `HelloWorld` that will generate two nodes, a display and a string. The module name will be used to name the slot that contains our generated ProtoFlux. The stuff after the `where` defines the body of our module. The `display` keyword creates a ValueDisplay/ObjectDisplay and the `"Hello World!"` is a string literal that will become a constant node input.

## Build

Build the module by running:
```
flux-sdk build HelloWorld.pg
```

This will generate a file called `HelloWorld.pg.brson` which is our Resonite Record.

## Import to Resonite

Open up Resonite and import `HelloWorld.pg.brson` into Resonite. You can either drag and drop it from your desktop file system or use the in game file browser to navigate and open it. Once it is in Resonite you can open an inspector on it to see the generated ProtoFlux which will be under the `HelloWorld` slot.

The generated ProtoFlux bundle is compatible with [Moduprint](https://wiki.resonite.com/Moduprint) and can be opened in it to view tabs, comments, etc.

## Language Primer

Depending on your background, ProtoGraph may be very different to how you have previously programmed.

> The best way to learn ProtoGraph will almost always be learning from someone else who already knows it. Reach out to others in the Resonite Discord or Resonite sessions in the ProtoGraph world for help and advice.

### For ProtoFlux Practitioners

The most important thing to remember is that ProtoGraph is just a way to describe your ProtoFlux connections. All your knowledge of ProtoFlux in Resonite transfers over.

**Modules = Nodes**

A module in ProtoGraph can be thought of as a node in ProtoFlux. You invoke a module by writing its name followed by (). You connect values to inputs by adding arguments inside the parentheses:

```
module DisplayLogValue
where {
    Log10Result = Log10_Float(N=1000.0);
    display(Log10Result);
}
```

You can use the `->` symbol to write in a more visual style:

```
module DisplayLogValue
where {
    1000.0->Log10_Float->display;
}
```

**Impulses Flow Opposite to Data**

Impulses are treated like they are on the opposite side of the node from the data:

```
module BooperDebouncer
in TouchButton: IButton global
in Clip: IAssetProvider<AudioClip>
in Booper: Slot element

where {
    Play = PlayOneShot(Clip=Clip, Root=Booper);
    Timeout = LocalImpulseTimeoutSeconds(Timeout=1.0, Next=Play);
    ButtonEvents(Pressed=Timeout.Trigger, Button=TouchButton);
}
```

### For Imperative Programmers (C, Python, JavaScript)

**Expression Oriented**

Everything in ProtoGraph is an expression. Every term you write is a 'thing' that has some value. This includes things you'd expect like numbers and strings but also nodes as well as control flow like `if` and `for` loops.

**Records**

Records are named tuples that join multiple expressions into a single expression:

```
module Records
where {
    Country = {
        Name = "United States";
        Population = 3.1e8;
    };
    display(Country.Name);
}
```

**Values over Variables**

When you give a name to a value, you cannot change it to something else later. If you need mutable state, you must explicitly mark it with `sync`/`store`/`local`:

```
module UpdatingVariable
where {
    sync PersistantData: int;
    UpdateData = {
        InnerValue = 2;
        PersistantData <- PersistantData + InnerValue;
    };
    CallInput(UpdateData);
    display(PersistantData);
}
```

**Explicit Sequencing with Impulses**

Impulses indicate that some effect has happened. Use the `impulse` context and `bind` for monadic sequencing:

```
module TestUrl
in UrlString: string
out this: AsyncImpulse
out Body: string

where impulse {
    Url = uri(UrlString);
    bind _ = If(Url->NotNull).OnTrue;
    bind Result = GET_String(Url).OnResponse;
    Body = Result.Content;
}
```

**Lazy Dataflow**

Expressions in ProtoGraph are 'lazy' - the value is computed when needed, not when defined. This matters when using mutable state.

### For Functional Programmers (Haskell, Elm, F#)

**Records = Named Tuples**

Records serve double duty as contexts for evaluation and data structures. The final expression is 'returned' as `this`.

**Modules = Functions**

Modules are the equivalent to functions. The public API is in the module header.

**Impulse = Continuation Monad**

Monadic sequencing uses impulses - essentially the continuation monad. Special syntax with `switch` and `impulse` contexts make composition easier (like Haskell do notation).

**Lazy Dataflow + Mutable State**

The combination of lazy evaluation and mutable state is manageable because all ProtoFlux nodes are total. Explicit ordering uses monadic impulses.

## Troubleshooting

### Invalid characters in path

Project directories and ProtoGraph source files should avoid using reserved characters in their paths. Restrict directory and file names to alphanumeric characters, dashes, and underscores.
