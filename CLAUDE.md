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
flux-sdk build -d build source/ModuleName.pg
```

## File Extensions
- `.pg` - ProtoGraph source files (in `source/`)
- `.brson` - Compiled output for Resonite import (in `build/`)
- `froox-nodes.yaml` - Authoritative node reference (3400+ nodes, in root)

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
// Correct module declaration
module MyModule  // PascalCase, matches filename MyModule.pg

// Correct user info access
User = LocalUser;
Username = User->UserUsername;
IsHost = User->IsUserHost;

// Correct position access (needs UserRoot)
UserRoot = User->UserUserRoot;
Pos = UserRoot->HeadPosition;

// BEST: FormatString with explicit object casting
Output = FormatString(
    Format="User: {0} | FPS: {1} | Ping: {2}ms",
    Parameters=[
        Username->as<object>,
        FPS->as<object>,
        Ping->as<object>
    ]
);

// Alternative: ConcatenateString for simple cases
NumStr = Value->ToString_Int;
Display = ConcatenateString("Count: ", NumStr);
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
flux-sdk build -d build source/ModuleName.pg

# Build all source files
flux-sdk build -d build source/*.pg

# Regenerate node reference
flux-sdk froox-docs -o froox-nodes.yaml
```

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
3. **Build** - Run `flux-sdk build -d build source/ModuleName.pg`
4. **Fix errors** (flux-build agent) - Reference YAML for corrections
5. **Deploy** (resonite-deploy) - Import `.brson` from `build/` into Resonite

---

## Quick Reference Commands

```bash
# Build a single module (source/ → build/)
flux-sdk build -d build source/ModuleName.pg

# Build all modules
flux-sdk build -d build source/*.pg

# Regenerate node reference
flux-sdk froox-docs -o froox-nodes.yaml

# Search for nodes
grep "^User" froox-nodes.yaml
grep -A10 "^NodeName:" froox-nodes.yaml
grep -i "searchterm" froox-nodes.yaml

# Count nodes
grep "^[A-Z]" froox-nodes.yaml | wc -l
```

## External Documentation
- Flux SDK: https://flux-sdk.samsmucny.com/
- Resonite ProtoFlux: https://wiki.resonite.com/ProtoFlux
- VS Code Extension: papaltine.protograph
