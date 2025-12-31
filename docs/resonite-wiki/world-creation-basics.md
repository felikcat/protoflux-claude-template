# World Creation Basics

Unlike most VR social platforms, Resonite's strength is powerful in-game world creation tools that limit you only by what the game engine can do.

## Introduction

A World is a saved asset containing everything needed for a Resonite Host to start, setup and run an environment. Everything about a world can be edited via the Scene Inspector.

Create a new world using the "Create New World" button in your Dash.

## Default Worlds

The two most popular starting points:

### Grid World

Great for creating worlds "set on the ground":
- 1km square quad mesh with grid texture
- 0 thickness collider
- Use texture tool to change ground or replace with different mesh

### Platform

For space stations, floating islands, etc.:
- Flat 0.2 by 30m cylinder with matching collider
- Floating in nearly nothing

### Blank

No ground, left floating. For starting from nothing.

## Skyboxes/World Lighting

Default worlds come with a Skybox component (under Root -> Skybox) providing sky view and world reflections.

### Basic Skybox

Default uses ProceduralSkyMaterial creating a sky with sun. To change:
- Load any 360° texture into Material Tool
- Click Primary on the sky
- Use Light Tool in 'Sun' mode to aim where sun should be

**CC0/CC-BY Skybox sources:**
- Resonite Essentials → Assets → Resonite Assets → Skyboxes
- Metaverse Academia Public → World-Building Public Assets → CC0 Skyboxes
- Creator Jam Public → Skyboxes

### Dawn Sky

The Cloud Home has an advanced skybox system with:
- Night/day cycle
- Adjustable sun
- Backgrounds and flying creatures

Uses The Sun Gun instead of Light Tool for sun position.

## Terrain/Landscape

Three main approaches:

### 1. Using Objects/3D Meshes

Most flexible and fun method, done fully in-game:
- Spawn objects from public folders
- Use simple shapes (cubes, cones)
- Set colliders as required

**Useful tools:**
- **Grabbable Setter Tool** - Make objects moveable or fixed
- **Character Collider Setter Tool** - Make objects walkable
- **Dev Tool** - Secondary to select gives Gizmo for precision movement

### 2. Displacement Mesh/Textures

Uses greyscale image (black = low, white = high):
1. Use `GridMesh` component
2. Put greyscale texture in DisplacementTexture
3. Set DisplacementMagnitude (height), Points (resolution), Size
4. Apply MeshCollider with Type:Static, CharacterCollider:True

**Pros:** Easily edited by swapping texture
**Cons:** Can't create holes, overhangs, or complex 3D geometry

### 3. 2D Mesh (Traditional)

Relies on external 3D modeling tools:
- Can optimize triangle count for detail where needed
- Import and pair with MeshCollider

**In-game editor:** Terrain Lab MMC22 (rhenium) - easy and fun but creates "low poly" look

## Buildings/Structures

### Dawn Modular

Building set using Module Snapping Tool:
- Used in nearly all Official Worlds
- CC-BY licensed
- Location: Resonite Essentials → Assets → Resonite Assets → 3D Models → Dawn Assets

### Dusk Modular

CC0 licensed community addition:
- Fully compatible with Dawn set
- Simpler, higher performance styling
- Location: Resonite Essentials → Assets → CC0 Assets → DuskModular

### Kitbash

Amazing tool to build houses including importation tools and prefabs.

## Saving

Save your world and make it your home via the Homes system.

## Advanced Topics

- Moving stuff with inspectors (Gizmos) and transforms
- Moving Spawn Point location
- Indoor/outdoor lighting switching
- Particles systems
- Gravity systems
- World optimization
- Organizing world hierarchy

## In-Game Resources

Explore Resonite's published worlds for ideas. Use dev tool and scene inspectors to learn how things work.

**Be careful about copying assets** without knowing licenses or getting permissions.

### Public Folders with Known Licenses

| Title | Content | License |
|-------|---------|---------|
| Metaverse Academy Public | Many things | Assorted |
| world-building resources (Medra) | Resources | CC-BY |
| Resonite Assets | Team created | CC-BY 4.0 |
| Team Lagom Public | Various | TBA |

### Search Tools

- **RedX** - Searches public folders (web and in-game facet)
- **UniPocket** - Japanese asset publishing and search tool

Source: https://wiki.resonite.com/World_creation_basics
