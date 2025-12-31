# Local Documentation

This directory contains comprehensive offline documentation for Flux SDK and Resonite development.

**Always use local documentation before external sources!**

## Directory Structure

```
docs/
├── flux-sdk/                    # ProtoGraph language reference (9 files)
├── resonite-wiki/               # Resonite Wiki documentation
│   ├── protoflux/              # 1,093 ProtoFlux node docs
│   │   └── INDEX.md            # Alphabetical node listing
│   ├── components/             # 1,519 Resonite component docs
│   │   └── INDEX.md            # Alphabetical component listing
│   └── *.md                    # Overview files (impulses, slots, etc.)
└── README.md                    # This file
```

## Flux SDK Documentation (`flux-sdk/`)

Complete ProtoGraph language reference:

| File | Topic |
|------|-------|
| [01-introduction.md](flux-sdk/01-introduction.md) | Overview of ProtoGraph and its goals |
| [02-getting-started.md](flux-sdk/02-getting-started.md) | Installation, setup, and first program |
| [03-basic-syntax.md](flux-sdk/03-basic-syntax.md) | File structure, comments, keywords, grouping |
| [04-types-and-variables.md](flux-sdk/04-types-and-variables.md) | Type system, literals, variables (sync/store/local) |
| [05-expressions-and-operators.md](flux-sdk/05-expressions-and-operators.md) | Expressions, records, operators, bindings |
| [06-impulse-control-flow.md](flux-sdk/06-impulse-control-flow.md) | Impulses, froox vs impulse context, async |
| [07-dynamics.md](flux-sdk/07-dynamics.md) | Dynamic variables and impulses (~read, ~write, ~trigger) |
| [08-modules-and-packages.md](flux-sdk/08-modules-and-packages.md) | Module I/O, packages, dependencies |
| [09-froox-prelude.md](flux-sdk/09-froox-prelude.md) | Available nodes and modules |

## Resonite Wiki Documentation (`resonite-wiki/`)

### ProtoFlux Nodes (1,093 nodes)

Complete documentation for all ProtoFlux nodes scraped from wiki.resonite.com:

- **Location:** `resonite-wiki/protoflux/`
- **Index:** [resonite-wiki/protoflux/INDEX.md](resonite-wiki/protoflux/INDEX.md)

### Components (1,519 components)

Complete documentation for all Resonite components:

- **Location:** `resonite-wiki/components/`
- **Index:** [resonite-wiki/components/INDEX.md](resonite-wiki/components/INDEX.md)

### Overview Files

| File | Topic |
|------|-------|
| [protoflux-overview.md](resonite-wiki/protoflux-overview.md) | ProtoFlux visual programming basics |
| [impulses.md](resonite-wiki/impulses.md) | Impulse system and execution context |
| [dynamic-variables.md](resonite-wiki/dynamic-variables.md) | Dynamic variable system |
| [components-overview.md](resonite-wiki/components-overview.md) | Component categories and essentials |
| [slots-and-hierarchy.md](resonite-wiki/slots-and-hierarchy.md) | Slot system and hierarchy |
| [rgb-cube-tutorial.md](resonite-wiki/rgb-cube-tutorial.md) | Complete beginner tutorial |

## Searching Documentation

```bash
# Find a ProtoFlux node
cat docs/resonite-wiki/protoflux/LocalUser.md

# Search ProtoFlux nodes for a concept
grep -ril "impulse" docs/resonite-wiki/protoflux/ | head -20

# Find a component
cat docs/resonite-wiki/components/TextRenderer.md

# Search components for a feature
grep -ril "collider" docs/resonite-wiki/components/ | head -20

# Browse all nodes/components
cat docs/resonite-wiki/protoflux/INDEX.md
cat docs/resonite-wiki/components/INDEX.md
```

## Source Attribution

- **Flux SDK:** Sourced from [Flux SDK](https://flux-sdk.samsmucny.com/) by Sam (Papaltine) Smucny. Licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/).
- **Resonite Wiki:** Scraped from [wiki.resonite.com](https://wiki.resonite.com/) using crawl4ai. Licensed under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).

## Quick Reference

### Module Structure
```
module ModuleName

in  InputName: type
in  SlotInput: Slot element
in  ButtonInput: IButton global

out OutputName: type
out this: type

use OtherModule

where {
    // Body expressions
}
```

### Variable Types
- `sync` - Synchronized with all users (network traffic)
- `store` - Persistent, local only
- `local` - Ephemeral, per impulse chain

### Key Operators
- `->` Pipe (forward composition)
- `<-` Write (assignment to variable)
- `|>` Branch (impulse routing in switch)
- `.` Field accessor

### Control Flow
```
// Switch expression
switch If(Condition=expr)
| OnTrue  |> impulse { ... }
| OnFalse |> impulse { ... };

// Impulse context with bind
impulse {
    bind Result = SomeAsyncNode().OnResponse;
    Variable <- Result.Value;
};

// Syntax sugar
if Condition then impulse { ... } else impulse { ... };
for i = 0 to 10 do impulse { ... };
while Condition do impulse { ... };
```

### Dynamic Operations
```
// Dynamic variables
~input<T>("VariableName")
Slot->~read<T>("Tag")
Slot->~write("Path", Value=value)

// Dynamic impulses
Slot->~trigger("Tag")
Slot->~trigger<T>("Tag", data)
switch ~receive<T>("Tag") | OnTriggered R |> impulse { ... };
```
