# Flux SDK ProtoGraph Project

Always ultrathink!

This is a ProtoGraph project using the Flux SDK to build ProtoFlux for Resonite VR.

## Technology Stack
- Language: ProtoGraph (.pg files)
- Compiler: flux-sdk CLI (F#-based)
- Target: Resonite VR (ProtoFlux nodes)
- Output: .brson files (Brotli-compressed BSON)

## Directory Structure
```
project/
├── source/           # ProtoGraph source files (.pg)
│   └── ModuleName.pg
├── build/            # Compiled output (.brson)
│   └── ModuleName.pg.brson
├── docs/             # Documentation
├── froox-nodes.yaml  # Node reference (root)
└── CLAUDE.md         # Project instructions
```

**All `.pg` source files go in `source/`**
**All `.brson` compiled files go in `build/`**

## Build Command
```bash
# Build a module from source/ to build/
flux-sdk build -o build/ModuleName.pg.brson source/ModuleName.pg

# Build all modules in source/ to build/
for f in source/*.pg; do flux-sdk build -o "build/$(basename "$f").brson" "$f"; done
```

**Important flags:**
- `-o <path>` - Output file path (use this for build directory)
- `-d <path>` - Project directory for module resolution (NOT output!)

## File Extensions
- `.pg` - ProtoGraph source files (in `source/`)
- `.brson` - Compiled output for Resonite import (in `build/`)
- `froox-nodes.yaml` - Authoritative node reference (3400+ nodes, in root)

---

## CRITICAL: Variable Declarations

### Location Matters!
- **`store`, `sync`, `local` variables go INSIDE `where {}`** - NOT in the module header
- **`in` and `out` declarations go in the header** - before `where`

```protograph
module CorrectExample

in InputSlot: Slot        // Header: inputs
out OutputValue: float    // Header: outputs

where {
    store MyState: float;     // INSIDE where block
    sync SharedData: int;     // INSIDE where block
    local TempValue: float3;  // INSIDE where block

    // ... rest of code
}
```

### WRONG - Variables in Header
```protograph
module WrongExample

store MyState: float;  // WRONG! Will cause parse error

where {
    // ...
}
```

---

## CRITICAL: Input Types for Resonite

### `element` vs Plain Types
When declaring slot/component inputs, the keyword affects how users connect in Resonite:

| Declaration | Creates | Resonite UX |
|-------------|---------|-------------|
| `in Cube: Slot element` | ElementSource | Harder - must parent object or use specific workflow |
| `in Cube: Slot` | ReferenceSource | Easier - just drag slot reference to `Reference` field |

**Recommendation:** Use plain `in Name: Slot` for easier Resonite setup unless you specifically need ElementSource behavior.

```protograph
// EASIER to connect in Resonite
in TargetSlot: Slot

// HARDER to connect (requires parenting or specific workflow)
in TargetSlot: Slot element
```

---

## CRITICAL: Arithmetic Operators

### Use Native Operators - NOT Verbose Nodes
ProtoGraph supports standard arithmetic operators. **Prefer these over explicit node calls:**

```protograph
// PREFERRED - clean and readable
Result = A + B;
Result = A - B;
Result = A * B;
Result = A / B;
Result = A mod B;
Combined = (A + 1.0f) * 0.5f - B;

// AVOID - unnecessarily verbose
Result = ValueAdd<float>(A=A, B=B);
Result = ValueSub<float>(A=A, B=B);
Result = ValueMul<float>(A=A, B=B);
```

### Comparison Operators
```protograph
// Use these directly
IsLess = A < B;
IsGreater = A > B;
IsEqual = A == B;
NotEqual = A != B;
```

---

## CRITICAL: Node Reference

**ALWAYS consult `froox-nodes.yaml` before writing or fixing ProtoGraph code.**

This file contains all 3400+ available ProtoFlux nodes with their exact names, input types, output types, and parameters. Generate it with:
```bash
flux-sdk froox-docs -o froox-nodes.yaml
```

### Node Entry Format
```yaml
NodeName:
  FullName: FrooxEngine.ProtoFlux.Runtimes.Execution.Nodes.Category.NodeName
  ThisType: "returnType"
  Inputs:
    ParamName: paramType
  Outputs: {}
  Globals: {}
```

---

## CRITICAL: Naming Conventions

### Module Names
- **MUST start with a capital letter** (PascalCase)
- **MUST match the filename exactly**
- Example: `module UserInfoDisplay` → file `UserInfoDisplay.pg`

### Node Names - Common Patterns

| Category | Pattern | Examples |
|----------|---------|----------|
| User Properties | `User{Property}` | `UserUsername`, `UserUserID`, `UserMachineID`, `UserPlatform`, `UserFPS`, `UserPing` |
| User Booleans | `IsUser{State}` | `IsUserPresent`, `IsUserHost`, `IsUserSilenced`, `IsUserInEditMode` |
| User VR State | `UserVR_Active` | Note the underscore! |
| World/Session | `World{Property}` | `WorldName`, `WorldUserCount`, `WorldMaxUsers`, `WorldAccessLevel` |
| User Roots | `User{RootProperty}` | `UserUserRoot`, `UserRootSlot`, `UserRootGlobalScale` |
| Head Tracking | `Head{Property}` | `HeadPosition`, `HeadRotation`, `HeadSlot` (require `UserRoot` input!) |
| Type Conversions | `ToString_{Type}` | `ToString_Int`, `ToString_Float`, `ToString_Float3`, `ToString_Bool` |
| Math with Types | `{Operation}_{Type}` | `FloorToInt_Float`, `Add_Float3_Float`, `Lerp_Color` |
| Time | Specific names | `UtcNow`, `LocalTimeOffset`, `FormatDateTimeAsTime`, `FormatTimespan` |
| References | `Local{Thing}` | `LocalUser`, `LocalUserRoot`, `LocalUserSlot` |

### WRONG vs CORRECT Node Names

| WRONG (will fail) | CORRECT |
|-------------------|---------|
| `User_Username` | `UserUsername` |
| `User_IsHost` | `IsUserHost` |
| `User_IsPresent` | `IsUserPresent` |
| `SessionName` | `WorldName` |
| `SessionUserCount` | `WorldUserCount` |
| `FloorToInt` | `FloorToInt_Float` |
| `LocalDateTime` | `UtcNow` + `LocalTimeOffset` |
| `DateTimeToString` | `FormatDateTimeAsTime` or `FormatDateTimeAsDate` |
| `TimeSpanToString` | `FormatTimespan` |
| `JoinStrings` | `StringJoin` |
| `Sin` or `SinFloat` | `Sin_Float` |
| `Distance` | `Distance_Float3` |
| `PackFloat3` | `Pack_Float3` |

### Multi-Output Nodes (Dot Notation)
Some nodes have multiple outputs. Access them with `.OutputName`:

```protograph
// GlobalTransform has multiple outputs
Transform = Slot->GlobalTransform;
Position = Transform.GlobalPosition;    // float3
Rotation = Transform.GlobalRotation;    // floatQ
Scale = Transform.GlobalScale;          // float3

// Or chain directly
Position = Slot->GlobalTransform.GlobalPosition;
```

**Common multi-output nodes:**
- `GlobalTransform` → `.GlobalPosition`, `.GlobalRotation`, `.GlobalScale`
- `LocalTransform` → `.LocalPosition`, `.LocalRotation`, `.LocalScale`
- `UnpackXYZ` → `.X`, `.Y`, `.Z`

---

## CRITICAL: Continuous Update Patterns

### Every-Frame Updates with LocalUpdate
Use `LocalUpdate` with a switch statement for code that runs every frame:

```protograph
where {
    store AccumulatedTime: float;

    NewTime = AccumulatedTime + DeltaTime;

    switch LocalUpdate
    | OnUpdate |> impulse {
        AccumulatedTime <- NewTime;
        // Other per-frame operations...
    };
}
```

### Timed Updates with SecondsTimer
For periodic updates (not every frame):

```protograph
where {
    switch SecondsTimer(Interval=1.0f)
    | OnUpdate |> impulse {
        // Runs every 1 second
    };
}
```

### Conditional Values
Use `ValueConditional<T>` for ternary-like logic:

```protograph
// If IsMoving is true, use 0.0f, otherwise use DeltaTime
TimeIncrement = ValueConditional<float>(
    Condition=IsStationary,
    OnTrue=DeltaTime,
    OnFalse=0.0f
);
```

---

## CRITICAL: String Formatting

### Avoid String Interpolation
The `$"text {value}"` syntax has **type inference issues** with non-string parameters. The compiler cannot properly cast to `object[]`.

### BEST: Use FormatString with Explicit Casting (Recommended)
`FormatString` is the cleanest approach for multi-value strings. **Cast all parameters to `object`** using `->as<object>`:

```protograph
// CORRECT - FormatString with explicit object casting
User = LocalUser;
Username = User->UserUsername;
FPS = User->UserFPS->FloorToInt_Float;
Ping = User->UserPing;

Output = FormatString(
    Format="User: {0}
FPS: {1}
Ping: {2}ms",
    Parameters=[
        Username->as<object>,
        FPS->as<object>,
        Ping->as<object>
    ]
);
```

**Key points:**
- Use `{0}`, `{1}`, `{2}` etc. as placeholders
- **MUST cast each parameter** with `->as<object>`
- Supports multiline strings directly in Format
- Much cleaner than chained ConcatenateString (52 nodes vs 127)

### Alternative: ConcatenateString for Simple Cases
For simple two-value joins, explicit conversion and concatenation works:

```protograph
// CORRECT - explicit conversion and concatenation
FPSStr = FPSValue->ToString_Int;
Display = ConcatenateString("FPS: ", FPSStr);
```

### WRONG: String Interpolation
```protograph
// WRONG - causes type inference errors
Display = $"FPS: {FPSValue}";
```

### String Nodes Available
- `FormatString` - **Preferred** for multi-value formatting (requires `->as<object>` casting)
- `ConcatenateString` - Join two strings
- `ConcatenateMultiString` - Join multiple strings
- `StringJoin` - Join with separator (Inputs: `Separator`, `Inputs`)
- `ToString_{Type}` - Convert value to string (e.g., `ToString_Int`, `ToString_Float3`)

---

## CRITICAL: Type-Specific Nodes

Many nodes require type suffixes. Always check `froox-nodes.yaml`:

```protograph
// Math operations
Result = Value->FloorToInt_Float;     // Not just FloorToInt
Result = Lerp_Float(A, B, T);         // Not just Lerp

// Comparisons
IsEqual = ValueEquals<int>(A, B);     // Generic with type parameter

// Conversions
Str = Number->ToString_Int;
Str = Position->ToString_Float3;
```

---

## CRITICAL: UserRoot vs User

Some nodes require `UserRoot` not `User`:

```protograph
// Get UserRoot from User first
CurrentUser = LocalUser;
UserRoot = CurrentUser->UserUserRoot;

// These require UserRoot:
HeadPos = UserRoot->HeadPosition;
HeadRot = UserRoot->HeadRotation;
Scale = UserRoot->UserRootGlobalScale;
HeadSlotRef = UserRoot->HeadSlot;
```

---

## CRITICAL: Display Limitations

### `display()` Does NOT Create World-Space Text
The `display()` function (and `ObjectDisplay<T>`, `ValueDisplay<T>`) only shows values **on the ProtoFlux node itself** in the visual programming graph. It does **NOT** create a visible TextRenderer or UI element in world space.

### ProtoFlux Cannot Create Visual Components
ProtoFlux is a data processing system. It can:
- ✅ Process and transform data
- ✅ Drive existing component fields
- ✅ Trigger impulses
- ❌ Create new slots, components, or visual objects

### To Display Output in World Space
1. **Import the .brson** into Resonite
2. **Create a Text object** (DevTool → Create New → 3D Text, or from Essentials)
3. **Wire the output:**
   - Find the final string output node in your ProtoFlux
   - Create a `Drive<string>` node
   - Connect string output → Drive node
   - Drag TextRenderer's `Content` field onto Drive's target
4. **Save as prefab** for reuse

### Alternative: Dynamic Variables
Write output to a dynamic variable, read with `DynamicValueVariableDriver<string>` on TextRenderer:
```protograph
// In ProtoFlux - write to dynamic var (requires impulse trigger)
switch OnStart
| Trigger |> TargetSlot->~write("Output/Text", Value=MyString);
```

---

## Local Documentation

Complete Flux SDK documentation in `docs/flux-sdk/`:

| File | Topic |
|------|-------|
| 01-introduction.md | Overview of ProtoGraph |
| 02-getting-started.md | Installation and first program |
| 03-basic-syntax.md | File structure, comments, keywords |
| 04-types-and-variables.md | Type system, literals, variables |
| 05-expressions-and-operators.md | Expressions, records, operators |
| 06-impulse-control-flow.md | Impulses, async, control flow |
| 07-dynamics.md | Dynamic variables and impulses |
| 08-modules-and-packages.md | Module I/O, packages, dependencies |
| 09-froox-prelude.md | Common modules overview |

---

## Agent Definitions

### protograph-dev
**Purpose:** Write and refactor ProtoGraph code

**CRITICAL Instructions:**
1. **ALWAYS** read `froox-nodes.yaml` first to verify node names exist
2. **NEVER** guess node names - search the YAML file
3. Use `grep "^NodeName" froox-nodes.yaml` to find exact node names
4. Module names MUST be PascalCase and match filename
5. **Use `FormatString` with `->as<object>` casting** for multi-value strings
6. Avoid `$"..."` string interpolation - causes type inference errors
7. Check if nodes need `User` or `UserRoot` input
8. Remember `display()` only shows on nodes, not in world space
9. **Write source files to `source/` directory** (e.g., `source/MyModule.pg`)
10. **`store`/`sync`/`local` go INSIDE `where {}`** - NOT in header!
11. **Use `in X: Slot`** not `in X: Slot element` for easier Resonite connection
12. **Use arithmetic operators** (`+`, `-`, `*`, `/`) not verbose nodes
13. **Check Lessons Learned section** for patterns from previous modules

**Before writing code:**
```bash
# Find user-related nodes
grep "^User" froox-nodes.yaml

# Find a specific node pattern
grep -i "position\|rotation" froox-nodes.yaml

# Get node details
grep -A10 "^HeadPosition:" froox-nodes.yaml
```

**Code patterns:**
```protograph
// Correct module structure
module MyModule  // PascalCase, matches filename MyModule.pg

in TargetSlot: Slot           // Use plain Slot, not "Slot element"
out Result: float

where {
    // Variables go INSIDE where block
    store PreviousValue: float;
    sync SharedState: int;

    // Use arithmetic operators directly
    Computed = PreviousValue + 1.0f * 0.5f;

    // Access multi-output nodes with dot notation
    Position = TargetSlot->GlobalTransform.GlobalPosition;

    // Conditional values
    Value = ValueConditional<float>(Condition=IsTrue, OnTrue=1.0f, OnFalse=0.0f);

    // Every-frame updates
    switch LocalUpdate
    | OnUpdate |> impulse {
        PreviousValue <- Computed;
        SetLocalScale(Instance=TargetSlot, Scale=Pack_Float3(X=1.0f, Y=1.0f, Z=1.0f));
    };
}
```

**FormatString pattern:**
```protograph
Output = FormatString(
    Format="User: {0} | FPS: {1}",
    Parameters=[Username->as<object>, FPS->as<object>]
);
```

---

### protoflux-reference
**Purpose:** Look up node names, types, and parameters

**Instructions:**
1. Primary source: `froox-nodes.yaml` (authoritative, 3400+ nodes)
2. Secondary: `docs/flux-sdk/09-froox-prelude.md` (common nodes)
3. Use grep patterns to search efficiently

**Search commands:**
```bash
# List all nodes in a category
grep "^User" froox-nodes.yaml
grep "^World" froox-nodes.yaml
grep "^Is" froox-nodes.yaml
grep "^ToString_" froox-nodes.yaml

# Get full node definition with inputs
grep -A15 "^UserFPS:" froox-nodes.yaml

# Find nodes by partial name
grep -i "head" froox-nodes.yaml

# Count available nodes
grep "^[A-Z]" froox-nodes.yaml | wc -l
```

**Key node categories:**
- `User*` - User properties (42+ nodes)
- `IsUser*` - User state checks (11 nodes)
- `World*` - World/session info (24 nodes)
- `Head*` - Head tracking (6 nodes, require UserRoot)
- `Local*` - Local user/transform (20+ nodes)
- `ToString_*` - Type to string (40+ nodes)
- `Format*` - Formatting nodes (6 nodes)
- `Concatenate*` - String joining (5 nodes)
- `Sin_*`, `Cos_*` - Trig functions by type
- `Distance_*` - Distance calculations by type
- `Pack_*` - Vector packing (e.g., `Pack_Float3`)
- `Value*<T>` - Generic value operations
- `GlobalTransform`, `LocalTransform` - Multi-output transform nodes
- `SetLocalScale`, `SetGlobalPosition` - Transform setters (impulse nodes)

---

### flux-build
**Purpose:** Handle compiler errors and build issues

**Common errors and fixes:**

| Error | Cause | Fix |
|-------|-------|-----|
| "module name does not match file name" | Case mismatch | Rename file or module to match exactly (PascalCase) |
| "not a valid module name" | Lowercase start | Module names must start with capital letter |
| "could not be constructed" | Wrong node name | Search `froox-nodes.yaml` for correct name |
| "Unknown Identifier" | Node doesn't exist | Verify in `froox-nodes.yaml` |
| "unknown type for parameter" | Type inference failed | Use explicit `->as<object>` casting |
| "Parameters has unknown type" | FormatString/interpolation issue | Use `FormatString` with `->as<object>` on each param |
| "INTERNAL(0:0 to 0:0)" parse error | `store`/`sync`/`local` in header | Move variable declarations INSIDE `where {}` block |
| Build writes to wrong location | Used `-d` instead of `-o` | Use `-o build/File.pg.brson` for output path |

**FormatString fix pattern:**
```protograph
// WRONG - type inference fails
Output = $"Value: {MyInt}";

// CORRECT - explicit object casting
Output = FormatString(
    Format="Value: {0}",
    Parameters=[MyInt->as<object>]
);
```

**Build commands:**
```bash
# Standard build (source/ → build/)
flux-sdk build -o build/ModuleName.pg.brson source/ModuleName.pg

# Build all source files
for f in source/*.pg; do flux-sdk build -o "build/$(basename "$f").brson" "$f"; done

# Regenerate node reference
flux-sdk froox-docs -o froox-nodes.yaml
```

**Note:** `-o` sets output path, `-d` sets project directory (for module resolution, NOT output!)

---

### impulse-architect
**Purpose:** Design async flows and multiplayer logic

**Key nodes for impulses:**
- `OnStart`, `OnActivated`, `OnDeactivated`, `OnDestroy`
- `SecondsTimer` (with `OnUpdate`)
- `Delay`, `DelaySecondsInt`
- `AsyncFor`, `AsyncWhile`, `AsyncSequence`
- `DynamicImpulseTrigger`, `DynamicImpulseReceiver`
- `LocalFireWhileTrue`, `LocalImpulseTimeoutSeconds`

**Multiplayer considerations:**
- `LocalUser` - the viewing user (different per client)
- `HostUser` - session host
- `IsUserHost` - check if user is host
- Use `sync` variables for synchronized state
- Use `store` for local-only persistent state

---

### resonite-deploy
**Purpose:** Import and debug in Resonite VR

**Workflow:**
1. Build produces `.brson` file in `build/` directory
2. Import `.brson` from `build/` into Resonite via inspector or drag-drop
3. Check ProtoFlux node connections
4. **Wire outputs to visual components manually** (see below)

**Connecting Slot Inputs:**

For `in X: Slot` (ReferenceSource - recommended):
1. Open Inspector on the ProtoFlux input slot
2. Find `ReferenceSource<Slot>` component
3. Drag target slot reference → drop on `Reference` field

For `in X: Slot element` (ElementSource - harder):
1. Either parent the target under the input slot, OR
2. Open Inspector, find `ElementSource<Slot>`, set `Target` field

**IMPORTANT: `display()` only shows values on nodes, NOT in world space!**

To see output in world:
1. Create a Text object in Resonite
2. Find the string output node in ProtoFlux
3. Create `Drive<string>` node, connect output to it
4. Drag TextRenderer's `Content` field to Drive target
5. Save as prefab for reuse

**Debugging nodes (show on node only):**
- `display(value)` - Shows value on the node
- `ValueDisplay<T>` / `ObjectDisplay<T>` - Typed display on node
- `ImpulseDisplay` - Impulse debugging

---

## Recommended Workflow

1. **Research nodes first** - Search `froox-nodes.yaml` for needed functionality
2. **Write code** (protograph-dev agent) - Write to `source/` directory
3. **Build** - Run `flux-sdk build -o build/ModuleName.pg.brson source/ModuleName.pg`
4. **Fix errors** (flux-build agent) - Reference YAML for corrections
5. **Deploy** (resonite-deploy) - Import `.brson` from `build/` into Resonite

---

## Quick Reference Commands

```bash
# Build a single module (source/ → build/)
flux-sdk build -o build/ModuleName.pg.brson source/ModuleName.pg

# Build all modules in source/
for f in source/*.pg; do flux-sdk build -o "build/$(basename "$f").brson" "$f"; done

# Regenerate node reference
flux-sdk froox-docs -o froox-nodes.yaml

# Search for nodes
grep "^User" froox-nodes.yaml
grep -A10 "^NodeName:" froox-nodes.yaml
grep -i "searchterm" froox-nodes.yaml

# Count nodes
grep "^[A-Z]" froox-nodes.yaml | wc -l
```

**Remember:** `-o` = output file, `-d` = project directory (NOT output!)

## External Documentation
- Flux SDK: https://flux-sdk.samsmucny.com/
- Resonite ProtoFlux: https://wiki.resonite.com/ProtoFlux
- VS Code Extension: papaltine.protograph

---

## Lessons Learned (Self-Updating)

This section captures discoveries from building real modules. **Update this when you learn something new!**

### From BouncingCube (2024-12)
A module that scales a cube up/down but pauses when the cube is moving.

**Discoveries:**
1. **Build flag confusion:** `-d` is project directory, `-o` is output path
2. **Variable location:** `store`/`sync`/`local` go INSIDE `where {}`, not in header
3. **Input types matter:** `in X: Slot element` (ElementSource) is harder to connect than `in X: Slot` (ReferenceSource)
4. **Use arithmetic operators:** `A + B` not `ValueAdd<float>(A, B)`
5. **Node naming patterns:**
   - Trig functions: `Sin_Float`, `Cos_Float` (not `Sin` or `SinFloat`)
   - Distance: `Distance_Float3` (not `Distance`)
   - Packing: `Pack_Float3` (not `PackFloat3` or `Float3`)
6. **Multi-output access:** `Slot->GlobalTransform.GlobalPosition` (dot notation)
7. **Continuous updates:** `switch LocalUpdate | OnUpdate |>` pattern
8. **Conditional values:** `ValueConditional<T>` for ternary-like behavior

**Working pattern for animation with pause:**
```protograph
where {
    store LastPosition: float3;
    store AnimTime: float;

    CurrentPos = Slot->GlobalTransform.GlobalPosition;
    IsStationary = Distance_Float3(CurrentPos, LastPosition) < 0.001f;
    TimeIncrement = ValueConditional<float>(Condition=IsStationary, OnTrue=DeltaTime, OnFalse=0.0f);
    NewAnimTime = AnimTime + TimeIncrement;

    switch LocalUpdate
    | OnUpdate |> impulse {
        AnimTime <- NewAnimTime;
        LastPosition <- CurrentPos;
    };
}
```

---

### Template for New Lessons

When you discover something new while building a module, add it here:

```markdown
### From ModuleName (YYYY-MM)
Brief description of what the module does.

**Discoveries:**
1. What you learned
2. What failed and why
3. What pattern worked

**Working code pattern:**
\`\`\`protograph
// Minimal example of the pattern
\`\`\`
```

---

## Self-Improvement Protocol

When building ProtoGraph modules:

1. **Before coding:** Search `froox-nodes.yaml` for nodes
2. **After errors:** Document what went wrong in Lessons Learned
3. **After success:** Extract reusable patterns
4. **Update CLAUDE.md:** Add new CRITICAL sections for common pitfalls

This makes the documentation self-improving with each project.
