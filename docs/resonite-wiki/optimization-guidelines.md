# Optimization Guidelines

This page details information and various avenues related to optimizing assets or creations in Resonite, ranging from high-level concepts to technical details.

## Rendering

Resonite currently uses Direct3D 11 for rendering in Unity.

### Textures

The StaticTexture2D and StaticTexture3D components display resolution, compression format, and total VRAM usage.

**Two main metrics to optimize:**

| Metric | Description |
|--------|-------------|
| **Asset size** | Size of original file on disk (PNG, WEBP, etc.). Optimize for cloud storage savings. |
| **VRAM size** | Size in video RAM on GPU. More important - high VRAM usage causes performance drops. |

**Best practices:**
- Textures should only be as big as necessary for "good enough" visuals
- For avatars, 2048x2048 ("2k") is usually enough
- Larger textures may be needed for noisy normal maps, very large meshes, or texture atlasing
- **Always use block compression** to reduce VRAM size (except for pixel art needing color perfection)
- Keep texture dimensions as power of two for better mipmap generation
- At minimum, dimensions should be multiples of 4 for efficient block compression
- Consider **atlasing** multiple small textures into one large texture

### Blendshapes

For every frame a mesh renders with nonzero blendshapes, every vertex is recalculated. This calculation does NOT scale with blendshape amount - 1 nonzero blendshape is about as heavy as several.

**Best practices:**
- Separate mesh parts not affected by blendshapes
- Bake non-zero blendshapes that don't change
- Separate high-density blendshape parts (like face tracking heads) from rest of mesh

Resonite provides automatic optimization buttons under SkinnedMeshRenderer:
- `Separate parts of mesh unaffected by blendshapes`
- `Bake non-driven blendshapes`

### Materials

- Some materials (notably Fur material) are much more expensive than others
- Use `Opaque` or `Cutout` blend mode when possible (uses deferred rendering pipeline)
- `Alpha`, `Transparent`, `Additive`, `Multiply` use forward rendering (more expensive)

### Procedural Assets

If not driving procedural mesh parameters, bake into a static mesh:
- Procedural meshes are per-world (duplicated with item)
- Static meshes are automatically instanced across worlds (single copy in memory)

### GPU Mesh Instancing

Multiple copies of same mesh/material combination are instanced, reducing draw calls.

**Not eligible for instancing:**
- SkinnedMeshRenderers
- Different material property blocks on same mesh

### Mirrors and Cameras

Very expensive, especially at higher resolutions in complex worlds.

**Optimization tips:**
- Use appropriate near/far clip values
- Use selective/exclusive render lists
- Localize with ValueUserOverride so users can opt in
- Provide resolution options

### Reflection Probes

- Baked probes are cheap (especially at 128x128 default)
- Realtime probes are extremely expensive (comparable to six cameras)
- For frequently-changing scenes, use timer-based updates instead of continuous

### Lighting

- Light impact proportional to pixels lit (visible light volume size)
- Short range or partially occluded lights are cheaper
- **Shadow-casting lights are much more expensive**
- Point lights with shadows are very expensive (render scene six times)
- Use spot or directional lights for shadows when possible

## ProtoFlux

### General Guidelines

- Less ProtoFlux is not always better - make calculations do less work
- Don't avoid ProtoFlux thinking "only components" is more optimal
- Choose best tool for the job case-by-case

### Writes and Drives

- **Impulse chains (writes)**: More explicit evaluation control
- **Drive chains**: More implicit evaluation timing

Writing to a field incurs network traffic at end of update. To prevent:
- Drive the field instead
- Use self-driven ValueCopy with writeback to "localize" the field

### Dynamic Impulses

Dynamic impulses recursively check all children of input slot for receivers.

**Best practice:** Minimize scope of dynamic impulses when called frequently.

### Continuously Changing Drive Chains

Nodes marked `ContinuouslyChanging` cause listener nodes to re-evaluate entire input chain every update.

If using heavy nodes (like `BodyNodeSlot` or `FindChildByName`) in such chains:
- Write results to a `Store` when they need updating
- Prevents heavy node re-evaluation every frame

### Measuring ProtoFlux Runtime

Use `Utc Now` with a variable storing value before execution. Subtract to get duration.

**Note:** This doesn't measure indirect impacts like network load or physics updates.

## Common Performance Myths

| Myth | Truth |
|------|-------|
| Slot count affects performance | No - only matters if something iterates over slots |
| ProtoFlux vs components have different performance | Case-by-case - depends on complexity |

## Culling

Resonite has built-in frustrum culling for meshes, but this doesn't affect CPU-based ProtoFlux or components.

For large/complex worlds, set up additional world-based culling.

## Profiling

Methods for profiling:

| Tool | Description |
|------|-------------|
| **Debug facet** | Dashboard home screen - shows world update cycle timings |
| **ResoniteMetricsCounter mod** | Timings for slot hierarchies, ProtoFlux chains, components |
| **dotnet-trace** | In-depth FrooxEngine traces (advanced) |
| **SteamVR Performance Graph** | GPU frametimes |
| **fpsVR** | CPU/GPU timings, VRAM/RAM usage |

Source: https://wiki.resonite.com/Optimization_guidelines
