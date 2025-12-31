# RGB Cube Tutorial

> Source: https://wiki.resonite.com/Tutorial:RGB_Cube

A comprehensive tutorial covering Entity Component System (Slots/Components) and ProtoFlux programming.

## Part 1: Basic Visuals

### Creating an Object
1. Equip **Dev Tool** (from Inventory: Resonite Essentials/Tools)
2. Open context menu, select `Create New...` > `Empty Object`
3. This creates an empty **Slot** (container for components)

### Adding a Mesh
1. Click `Attach Component` in inspector
2. Select `Assets/Procedural Meshes/BoxMesh`
3. Add `Rendering/MeshRenderer` component
4. Grab BoxMesh header, drop on MeshRenderer's `Mesh` field

### Adding a Material
1. Add `Assets/Materials/PBS_Metallic` component
2. In MeshRenderer, click `Add` under `Materials (list):`
3. Drag PBS_Metallic reference to the new material slot

## Part 2: Basic Interaction

### Adding Physics
1. Add `Physics/BoxCollider` component
2. Laser now hits the box

### Making it Grabbable
1. Add `Transform/Interaction/Grabbable` component
2. Enable `Scalable` for two-hand scaling

## Part 3: Data Binding

### ValueCopy Component
Instead of manually copying values between BoxMesh and BoxCollider sizes:

1. Add `Transform/Drivers/ValueCopy` component
2. Set `Source` = BoxMesh's `Size` field
3. Set `Target` = BoxCollider's `Size` field

Driven fields appear **pink** in inspector:
- Value computed from source
- Cannot be manually edited
- Each user computes locally (not synced)

Enable `WriteBack` to allow editing either field.

## Part 4: ProtoFlux Programming

### Creating a Source Node
1. Equip **ProtoFlux Tool** (from Essentials/Tools)
2. Grab a property name (e.g., `AlbedoColor`)
3. Select `Source` from context menu

### Creating a Display
- Hold primary on output, tap secondary to create `Value Display`
- Shows value on the node itself

### Creating a Write Node
1. Open node browser (context menu > `Browse nodes`)
2. Navigate to `Actions/Write/ValueWrite<T>/ValueWrite<colorX>`
3. Double-click to select, double-click empty space to spawn

### Write Node Anatomy
| Element | Purpose |
|---------|---------|
| `*` input (white triangle) | Trigger with impulse |
| `Value` input (orange) | Value to write |
| `OnWritten` output | Continues on success |
| `OnFail` output | Continues on failure |
| `Variable` field | Target to write to |

### Creating Inputs
- Drag from input, tap secondary to create:
  - `Call Input` for impulse triggers
  - `Input` node for values

## Part 5: Automation

### Random Color on Hit
```
On Contact Start → If (IsLocalUser) → Write<colorX> → Play One Shot
                                          ↑
                                   Random Hue ColorX
```

### Key Components
| Node | Purpose |
|------|---------|
| `On Contact Start` | Fires when collider touches something |
| `Random Hue ColorX` | Generates random color |
| `Play One Shot` | Plays audio clip |
| `If` | Conditional branching |
| `Is Local User` | Check if impulse is from local user |

### Packing ProtoFlux
1. Hold secondary on nodes until selected (light blue)
2. Grab slot from inspector
3. Context menu > `Pack Into`

## Part 6: Drives vs Impulses

### Impulses (Imperative)
- Discrete actions that happen once
- Trigger network sync
- Good for: events, button presses, collisions

### Drives (Declarative)
- Continuous evaluation
- Computed locally per user
- No network traffic
- Good for: animations, smooth transitions

### RGB Color Drive Example
```
World Time Float → ColorX Hue → Value Field Drive<colorX>
                                        ↓
                                  AlbedoColor
```

## Part 7: Variables

### Three Variable Types

| Type | Scope | Synced | Use Case |
|------|-------|--------|----------|
| Data Model Store | World | Yes | Shared state |
| Store | Per User | No | User-specific persistent |
| Local | Per Impulse | No | Temporary calculations |

### Display Behavior
- Data Model Store: Updates immediately
- Store: Requires re-creating display to see changes
- Local: Only valid during impulse chain

## Part 8: Flash Effect

Combine impulses and drives for flash-on-hit:

```protograph
// Store time of last hit
store T_lastHit: float;

// Calculate time since hit
TimeSinceHit = WorldTimeFloat - T_lastHit;

// Exponential decay (1 → 0)
FlashAmount = Pow(0.01f, TimeSinceHit);

// Lerp between normal and boosted color
BoostedColor = ColorXMulRGB(BaseColor, 10.0f);
FinalColor = Lerp(BaseColor, BoostedColor, FlashAmount);

// On collision, update last hit time
switch OnContactStart
| OnEvent |> If (IsLocalUser) |> impulse {
    T_lastHit <- WorldTimeFloat;
};
```

## Part 9: Filtering Impulses

### Prevent Self-Hits
```
Active User Self ≠ Active User (from hit slot)
        ↓
       AND ← Is Local User
        ↓
       If → Continue...
```

### Timeout Between Hits
Use `LocalImpulseTimeoutSeconds` to prevent rapid re-triggering.

## Key Takeaways

1. **Slots** are containers for components
2. **Components** provide functionality
3. **Drivers** continuously update values (local, no sync)
4. **Impulses** trigger discrete actions (can sync)
5. **Pack** ProtoFlux into slots for saving
6. Use **Data Model Store** for synced values
7. Use **Drives** for smooth animations
8. Filter impulses with **If** nodes for proper multiplayer behavior
