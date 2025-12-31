# Resonite Wiki Reference

Comprehensive Resonite Wiki documentation scraped from wiki.resonite.com using crawl4ai.

> Original source: https://wiki.resonite.com/
> License: [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)

## Directory Structure

```
resonite-wiki/
├── protoflux/              # 1,093 ProtoFlux node documentation files
│   ├── INDEX.md           # Alphabetical listing of all nodes
│   └── *.md               # Individual node documentation
├── components/             # 1,519 Resonite component documentation files
│   ├── INDEX.md           # Alphabetical listing of all components
│   └── *.md               # Individual component documentation
└── *.md                    # Overview files (this directory)
```

## ProtoFlux Nodes (`protoflux/`)

**1,093 node documentation files** - Complete reference for all ProtoFlux nodes.

- **Browse all:** [protoflux/INDEX.md](./protoflux/INDEX.md)
- **Read a node:** `cat protoflux/LocalUser.md`
- **Search:** `grep -ril "impulse" protoflux/`

## Components (`components/`)

**1,519 component documentation files** - Complete reference for all Resonite components.

- **Browse all:** [components/INDEX.md](./components/INDEX.md)
- **Read a component:** `cat components/TextRenderer.md`
- **Search:** `grep -ril "collider" components/`

## Overview Files

### Core Concepts
| File | Description |
|------|-------------|
| [protoflux-overview.md](./protoflux-overview.md) | ProtoFlux visual programming basics |
| [protoflux-main.md](./protoflux-main.md) | ProtoFlux main reference (variables, packing) |
| [protoflux-tool.md](./protoflux-tool.md) | ProtoFlux Tool usage guide |
| [impulses.md](./impulses.md) | Impulse system and execution context |
| [context.md](./context.md) | ProtoFlux context (ExecutionContext, FrooxEngineContext) |
| [dynamic-variables.md](./dynamic-variables.md) | Dynamic variable system |
| [components-overview.md](./components-overview.md) | Component categories and essential components |
| [component.md](./component.md) | What components are and how they work |
| [slots-and-hierarchy.md](./slots-and-hierarchy.md) | Slot system and hierarchy |
| [slot.md](./slot.md) | Slot reference (fields, properties) |

### Data & Architecture
| File | Description |
|------|-------------|
| [data-model.md](./data-model.md) | FrooxEngine data model (elements, workers, events) |
| [linkage-drives.md](./linkage-drives.md) | Links, drives, and hooks |

### Tools & Controls
| File | Description |
|------|-------------|
| [tools.md](./tools.md) | All Resonite tools reference |
| [basic-controls.md](./basic-controls.md) | Controller and desktop controls |
| [scene-inspector.md](./scene-inspector.md) | Scene Inspector guide |

### World & Avatar Creation
| File | Description |
|------|-------------|
| [world-creation-basics.md](./world-creation-basics.md) | World creation guide |
| [humanoid-rig-requirements.md](./humanoid-rig-requirements.md) | Avatar rig requirements for IK |
| [gestures.md](./gestures.md) | Facial animations and gestures |
| [optimization-guidelines.md](./optimization-guidelines.md) | Performance optimization guide |

### Reference
| File | Description |
|------|-------------|
| [faq.md](./faq.md) | Frequently Asked Questions |
| [command-line-arguments.md](./command-line-arguments.md) | Launch arguments reference |
| [rgb-cube-tutorial.md](./rgb-cube-tutorial.md) | Complete beginner tutorial |

## Quick Reference

### Variable Types
| Type | Scope | Synced | Use |
|------|-------|--------|-----|
| Data Model Store | World | Yes | Shared state |
| Store | Per User | No | User-persistent |
| Local | Per Impulse | No | Temporary |

### Impulse vs Drive
| Impulses | Drives |
|----------|--------|
| Discrete actions | Continuous |
| Can sync to network | Local only |
| `switch` statements | Direct assignment |
| Write nodes | Drive nodes |

### Essential Components
- `MeshRenderer` - Render 3D meshes
- `PBS_Metallic` - PBR material
- `BoxCollider` - Physics collision
- `Grabbable` - Allow grabbing
- `DynamicVariableSpace` - Variable scoping
- `ValueCopy<T>` - Drive values

### ProtoGraph Dynamic Variable Syntax
```protograph
// Read
Value = Slot->~read<float>("VarName").Value;

// Write (impulse)
switch Slot->~write("VarName", Value=MyValue)
| OnSuccess |> impulse { };

// Input source
Input = ~input<float>("VarName");
```

## External Links
- [Resonite Wiki](https://wiki.resonite.com/)
- [ProtoFlux Node Browser](https://wiki.resonite.com/Category:ProtoFlux)
- [Component List](https://wiki.resonite.com/Category:Components)
- [Flux SDK Docs](https://flux-sdk.samsmucny.com/)
