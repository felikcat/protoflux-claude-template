# Flux SDK ProtoGraph Project

Always ultrathink!

ProtoGraph project using Flux SDK to build ProtoFlux for Resonite VR.

## ⚠️ MANDATORY: CHECK RESONITE WIKI FIRST

**BEFORE doing ANYTHING Resonite-related:** STOP → SEARCH → READ → VERIFY → then code (if needed).

```bash
grep -ril "keyword" docs/resonite-wiki/components/ | head -20
grep -ril "keyword" docs/resonite-wiki/protoflux/ | head -20
cat docs/resonite-wiki/components/INDEX.md | grep -i "keyword"
```

**Built-in UI (no ProtoFlux needed):** `Inventory → Resonite Essentials → Default UI`:
Keyboard, AudioStreamController, TextDisplay, UrlDisplay, NoticeDisplay, AudioPlayer, DocumentDisplay, VideoPlayer, ProgressBar, ColorDialog

---

## Project Structure

| Directory | Purpose | Created By |
|-----------|---------|------------|
| `specs/*.nodespec.yaml` | Node specifications | protoflux-reference (FIRST) |
| `source/*.pg` | ProtoGraph source | protograph-dev |
| `build/*.brson` | Compiled output | flux-sdk build |
| `docs/` | Documentation | - |
| `froox-nodes.yaml` | 3400+ node reference | flux-sdk froox-docs |

**Tech:** ProtoGraph (.pg) → flux-sdk CLI (F#) → .brson (Brotli BSON) → Resonite VR

## Build Commands

```bash
flux-sdk build -o build/Module.pg.brson source/Module.pg        # Single module
for f in source/*.pg; do flux-sdk build -o "build/$(basename "$f").brson" "$f"; done  # All
flux-sdk froox-docs -o froox-nodes.yaml                          # Regenerate node ref
```

**Flags:** `-o` = output path, `-d` = project directory (NOT output!)

---

## CRITICAL: Syntax Rules

### Variable Placement
```protograph
module Example
in Input: Slot              // Header: in/out only
out Output: float
where {
    store State: float;     // INSIDE where: store/sync/local
    sync Shared: int;
    local Temp: float3;
}
```

### Input Types
| Declaration | Creates | Resonite UX |
|-------------|---------|-------------|
| `in X: Slot` | ReferenceSource | **Easier** - drag to Reference field |
| `in X: Slot element` | ElementSource | Harder - requires parenting |

### Operators (prefer native)
```protograph
Result = A + B;  Result = A - B;  Result = A * B;  Result = A / B;  Result = A mod B;
IsLess = A < B;  IsGreater = A > B;  IsEqual = A == B;  NotEqual = A != B;
// AVOID: ValueAdd<float>(A=A, B=B) - unnecessarily verbose
```

### Naming Conventions

**Modules:** PascalCase, must match filename exactly (e.g., `module MyModule` → `MyModule.pg`)

**Node Patterns:**

| Category | Pattern | Examples |
|----------|---------|----------|
| User Properties | `User{Property}` | UserUsername, UserUserID, UserFPS, UserPing |
| User Booleans | `IsUser{State}` | IsUserPresent, IsUserHost, IsUserSilenced |
| User VR | `UserVR_Active` | Note underscore |
| World | `World{Property}` | WorldName, WorldUserCount, WorldMaxUsers |
| User Roots | `User{Root}` | UserUserRoot, UserRootSlot, UserRootGlobalScale |
| Head Tracking | `Head{Property}` | HeadPosition, HeadRotation, HeadSlot (need UserRoot!) |
| Conversions | `ToString_{Type}` | ToString_Int, ToString_Float, ToString_Float3 |
| Math | `{Op}_{Type}` | FloorToInt_Float, Lerp_Color, Sin_Float |
| Local Refs | `Local{Thing}` | LocalUser, LocalUserRoot, LocalUserSlot |
| Time | Specific | UtcNow, LocalTimeOffset, FormatDateTimeAsTime, FormatTimespan |

**WRONG → CORRECT:**

| Wrong | Correct | Wrong | Correct |
|-------|---------|-------|---------|
| User_Username | UserUsername | Sin / SinFloat | Sin_Float |
| User_IsHost | IsUserHost | Distance | Distance_Float3 |
| SessionName | WorldName | PackFloat3 | Pack_Float3 |
| FloorToInt | FloorToInt_Float | JoinStrings | StringJoin |

### Multi-Output Nodes (dot notation)
```protograph
Position = Slot->GlobalTransform.GlobalPosition;  // float3
Rotation = Slot->GlobalTransform.GlobalRotation;  // floatQ
Scale = Slot->GlobalTransform.GlobalScale;        // float3
// Also: LocalTransform, UnpackXYZ (.X, .Y, .Z)
```

---

## CRITICAL: Patterns

### Continuous Updates
```protograph
where {
    store Time: float;
    switch LocalUpdate | OnUpdate |> impulse { Time <- Time + DeltaTime; };
}
// Timed: switch SecondsTimer(Interval=1.0f) | OnUpdate |> impulse { ... };
```

### Conditional Values
```protograph
Value = ValueConditional<float>(Condition=IsTrue, OnTrue=1.0f, OnFalse=0.0f);
```

### String Formatting (FormatString with ->as<object>)
```protograph
// CORRECT - use FormatString with explicit casting
Output = FormatString(Format="User: {0}\nFPS: {1}", Parameters=[Username->as<object>, FPS->as<object>]);
// WRONG - $"FPS: {Val}" causes type inference errors
// Alternative: ConcatenateString("FPS: ", Val->ToString_Int)
```

**String nodes:** FormatString (preferred), ConcatenateString, ConcatenateMultiString, StringJoin, ToString_{Type}

### Type-Specific Nodes
```protograph
Result = Value->FloorToInt_Float;    // Not FloorToInt
IsEq = ValueEquals<int>(A, B);       // Generic with type param
```

### UserRoot vs User
```protograph
UserRoot = LocalUser->UserUserRoot;
HeadPos = UserRoot->HeadPosition;    // These require UserRoot, not User
HeadRot = UserRoot->HeadRotation;
Scale = UserRoot->UserRootGlobalScale;
```

---

## CRITICAL: Display & Output Limitations

`display()`, `ValueDisplay<T>`, `ObjectDisplay<T>` show values **on ProtoFlux nodes only**, NOT in world space.

ProtoFlux **cannot create** slots/components/visuals. It can: process data ✓, drive existing fields ✓, trigger impulses ✓.

**To display in world:**
1. Import .brson → Create Text object → Create `Drive<string>` node → Connect output → Drag TextRenderer's Content to Drive target

**Dynamic variable alternative:**
```protograph
switch OnStart | Trigger |> TargetSlot->~write("Output/Text", Value=MyString);
```

---

## Built-in UI Assets

**Location:** `Inventory → Resonite Essentials → Default UI`

| Asset | Purpose | Key Fields |
|-------|---------|------------|
| Keyboard | Virtual keyboard | - |
| AudioStreamController | Audio stream control | - |
| TextDisplay | Display text | - |
| UrlDisplay | Display URLs | - |
| NoticeDisplay | Notices/alerts | - |
| AudioPlayer | Audio playback | - |
| DocumentDisplay | Documents | - |
| VideoPlayer | Video playback | - |
| ProgressBar | Progress indicator | - |
| ColorDialog | RGB/HSV color picker | TargetColor, Continuous, AllowAlpha, AllowHDR |

**Use built-in when:** color picking, video/audio, text display, progress, keyboard input.
**Write ProtoFlux when:** custom logic, value processing, unsupported features.

**ColorDialog example (no ProtoFlux):** Create box → Add material → Spawn ColorDialog → Inspector → Drag material's AlbedoColor → Drop on ColorDialogInterface's TargetColor. Done.

**Other paths:** Tools at `Resonite Essentials → Tools`, 3D Models at `Assets → Resonite Assets → 3D Models`, CC0 at `CC0 Assets → DuskModular`

---

## Local Documentation

**Priority:** 1) `docs/resonite-wiki/components/` (built-in check) → 2) `froox-nodes.yaml` (3400+ nodes) → 3) `docs/resonite-wiki/protoflux/` (1,093 nodes) → 4) `docs/flux-sdk/` → 5) External

**Flux SDK docs (`docs/flux-sdk/`):** 01-introduction, 02-getting-started, 03-basic-syntax, 04-types-and-variables, 05-expressions-and-operators, 06-impulse-control-flow, 07-dynamics, 08-modules-and-packages, 09-froox-prelude

**Resonite Wiki (`docs/resonite-wiki/`):** 1,093 ProtoFlux nodes in `protoflux/`, 1,519 components in `components/`, overview files: impulses.md, dynamic-variables.md, slots-and-hierarchy.md, protoflux-overview.md, components-overview.md, rgb-cube-tutorial.md

```bash
# Search commands
grep -l "Node" docs/resonite-wiki/protoflux/*.md    # Find node by name
grep -ril "concept" docs/resonite-wiki/protoflux/   # Search nodes
cat docs/resonite-wiki/protoflux/INDEX.md           # List all nodes
grep -l "Comp" docs/resonite-wiki/components/*.md   # Find component
grep -ril "feature" docs/resonite-wiki/components/  # Search components
cat docs/resonite-wiki/components/INDEX.md          # List all components
```

**External (last resort):** https://flux-sdk.samsmucny.com/, https://wiki.resonite.com/, VS Code: papaltine.protograph

---

## Agent Definitions

### ALL AGENTS: First Step
```bash
grep -ril "keyword" docs/resonite-wiki/components/ | head -20
grep -ril "keyword" docs/resonite-wiki/protoflux/ | head -20
# Check Default UI list above. If built-in exists and you write ProtoFlux, you have FAILED.
```

---

### protoflux-reference
**Purpose:** Research nodes, produce verified specifications. **MANDATORY before protograph-dev.**

**Workflow:**
1. Check built-in solutions (grep components, check Default UI)
2. If none, research nodes (grep protoflux, verify in froox-nodes.yaml)
3. Write `specs/ModuleName.nodespec.yaml`
4. Validate via `flux-sdk froox-docs -o froox-nodes.yaml`

**Specification format:**
```yaml
module: ModuleName
description: Brief description
builtin_solution: null  # or path if applicable
inputs:
  - name: TargetSlot
    type: Slot
    element: false  # true=ElementSource, false=ReferenceSource
    description: The slot to animate
outputs:
  - name: Result
    type: float
    description: The computed result
nodes_required:
  - name: GlobalTransform
    verified: true
    wiki_doc: docs/resonite-wiki/protoflux/GlobalTransform.md
    inputs: {Instance: Slot}
    outputs: {GlobalPosition: float3, GlobalRotation: floatQ, GlobalScale: float3}
    notes: Multi-output, use dot notation
patterns:
  continuous_update: |
    switch LocalUpdate | OnUpdate |> impulse { ... };
warnings: ["Distance_Float3 not Distance", "store/sync/local INSIDE where {}"]
verified_by: flux-sdk froox-docs
verified_at: YYYY-MM-DD
```

**Node categories:** User{Property} (42+), IsUser{State} (11), World{Property} (24), Head{Property} (6, need UserRoot!), Local{Thing} (20+), ToString_{Type} (40+), {Func}_{Type} (Sin_Float, Distance_Float3, Pack_Float3)

---

### protograph-dev
**Purpose:** Write ProtoGraph code. **BLOCKED until protoflux-reference completes.**

**Prereqs:** `specs/ModuleName.nodespec.yaml` must exist.

**Workflow:** Read spec → Write code using ONLY verified nodes → Build → Report errors

**Code template:**
```protograph
module MyModule  // PascalCase, matches filename
in TargetSlot: Slot
out Result: float
where {
    store PreviousValue: float;
    sync SharedState: int;
    Computed = PreviousValue + 1.0f * 0.5f;
    Position = TargetSlot->GlobalTransform.GlobalPosition;
    Value = ValueConditional<float>(Condition=IsTrue, OnTrue=1.0f, OnFalse=0.0f);
    switch LocalUpdate | OnUpdate |> impulse {
        PreviousValue <- Computed;
        SetLocalScale(Instance=TargetSlot, Scale=Pack_Float3(X=1.0f, Y=1.0f, Z=1.0f));
    };
}
```

**After writing:** Build, report errors (use flux-build if needed), confirm node count, update Lessons Learned.

---

### flux-build
**Purpose:** Handle compiler errors. Check docs before fixing, never guess node names.

| Error | Cause | Fix |
|-------|-------|-----|
| "module name does not match" | Case mismatch | Match exactly (PascalCase) |
| "not a valid module name" | Lowercase start | Capitalize |
| "could not be constructed" | Wrong node name | Search froox-nodes.yaml |
| "Unknown Identifier" | Node doesn't exist | Verify in froox-nodes.yaml |
| "unknown type for parameter" | Type inference | Use `->as<object>` |
| "Parameters has unknown type" | FormatString issue | FormatString with `->as<object>` |
| "INTERNAL(0:0 to 0:0)" | Variables in header | Move store/sync/local INTO where {} |
| Wrong output location | Used -d not -o | Use `-o build/File.brson` |

---

### impulse-architect
**Purpose:** Design async flows and multiplayer logic.

**Read first:** `docs/resonite-wiki/impulses.md`, `docs/resonite-wiki/dynamic-variables.md`, `docs/flux-sdk/06-impulse-control-flow.md`

**Key nodes:** OnStart, OnActivated, OnDeactivated, OnDestroy, SecondsTimer, Delay, DelaySecondsInt, AsyncFor, AsyncWhile, AsyncSequence, DynamicImpulseTrigger, DynamicImpulseReceiver, LocalFireWhileTrue, LocalImpulseTimeoutSeconds

**Multiplayer:** LocalUser (per client), HostUser, IsUserHost, `sync` for synchronized state, `store` for local-only.

---

## Workflow Chain

```
protoflux-reference → specs/*.nodespec.yaml
        ↓
protograph-dev → source/*.pg + build/*.brson
        ↓ (if errors)
flux-build → fixed code
```

**For complex impulse design:** impulse-architect → protoflux-reference → protograph-dev

**FORBIDDEN:** Running protograph-dev without spec, writing code without verified nodes, skipping built-in check.

---

## Quick Reference

```bash
# Build
flux-sdk build -o build/Module.pg.brson source/Module.pg
for f in source/*.pg; do flux-sdk build -o "build/$(basename "$f").brson" "$f"; done

# Node reference
flux-sdk froox-docs -o froox-nodes.yaml
grep "^NodeName:" froox-nodes.yaml
grep -A10 "^NodeName:" froox-nodes.yaml
grep "^[A-Z]" froox-nodes.yaml | wc -l  # Count nodes

# Documentation
cat docs/resonite-wiki/protoflux/INDEX.md
cat docs/resonite-wiki/components/INDEX.md
cat docs/resonite-wiki/impulses.md
cat docs/resonite-wiki/dynamic-variables.md
```

---

## Lessons Learned

### BouncingCube (2024-12)
Scales cube up/down, pauses when moving.

**Discoveries:** `-d` = project dir, `-o` = output | Variables INSIDE where {} | `in X: Slot` easier than `Slot element` | Use arithmetic operators | Sin_Float not Sin, Distance_Float3 not Distance, Pack_Float3 not PackFloat3 | Dot notation for multi-output | `switch LocalUpdate | OnUpdate |>` pattern | ValueConditional<T> for ternary

```protograph
where {
    store LastPosition: float3;
    store AnimTime: float;
    CurrentPos = Slot->GlobalTransform.GlobalPosition;
    IsStationary = Distance_Float3(CurrentPos, LastPosition) < 0.001f;
    TimeIncrement = ValueConditional<float>(Condition=IsStationary, OnTrue=DeltaTime, OnFalse=0.0f);
    NewAnimTime = AnimTime + TimeIncrement;
    switch LocalUpdate | OnUpdate |> impulse { AnimTime <- NewAnimTime; LastPosition <- CurrentPos; };
}
```

### ColorChanger (2024-12)
User wanted color picker for box.

**Discovery:** ColorDialog exists at Default UI! Don't overengineer. Legacy UI deprecated, UIX is modern.

**Correct:** Create box → Material → Spawn ColorDialog → Inspector → Drag AlbedoColor → Drop on TargetColor. Done.

### Template
```markdown
### ModuleName (YYYY-MM)
Description.
**Discoveries:** 1. Learned 2. Failed 3. Worked
**Pattern:** \`\`\`protograph ... \`\`\`
```

---

## Self-Improvement Protocol

**Every task:** STOP → SEARCH docs → READ → VERIFY built-in → DECIDE → CODE (if needed)

**After tasks:** Update Lessons Learned with wrong/correct approaches.

**Remember:** Search first is NOT optional. Built-in > Custom ProtoFlux.
