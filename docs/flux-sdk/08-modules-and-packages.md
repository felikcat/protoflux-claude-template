<!--
Source: https://flux-sdk.samsmucny.com/ProtoGraph/Modules-and-Packages.html
License: CC BY-NC-SA 4.0
Author: Sam (Papaltine) Smucny
-->

# Modules and Packages

Modules are the primary unit of abstraction in ProtoGraph. When translated to ProtoFlux, they can be thought of as custom/nested nodes with reusable code. Each module lives in its own file, and the filename must match the module name. So `SampleModule` would be in `SampleModule.pg`.

A directory with one or more modules is called a package. The directory name is the package name (Pascal Case). Packages can be nested. A module within a package uses `/` to separate path parts: `PackageA/PackageB/ModuleC` would be at `DirectoryA/DirectoryB/ModuleC.pg`.

## Use Other Modules

Use the `use` keyword followed by the module name. For multiple modules from a single package, enclose items in `( )`:

```
module MainModule

use ModuleA                   // ModuleA.pg
use X/Y/ModuleB               // X/Y/ModuleB.pg
use X (DoW, DoV, DoU)         // X/DoW.pg & X/DoV.pg & X/DoU.pg
```

All module names are relative to the project root (working directory when you run build).

### Use Aliases

Alias imports with `as`:

```
module MainModule

use ModuleA as A
use X/Y/ModuleB as B
use X (DoW as W, DoV, DoU)
```

## Module I/O

Define a public API using inputs and outputs.

### Inputs (Sources)

Define with the `in` keyword. Every input needs a name and data type:

```
module InputModuleExample

/// This text will be displayed.
/// Any valid <i>string</i> is valid.
in Text: string

where {
    display(Text)
}
```

Documentation comments are included in packed ProtoFlux as dynamic variables for help text.

#### Elements (Changeable Sources)

Mark an input as `ElementSource` with the `element` modifier:

```
module ElementSourceExample

/// This is an <i>ElementSource</i>.
in Target: Slot element

where {
    Target->GetSlotName->display;
}
```

#### Globals

Inputs can be designated as `global`:

```
module GlobalSource

in ButtonSrc: IButton global
in GlobalUser: User global

where {
    ButtonEvents(Button=ButtonSrc, Pressed=ImpulseDisplay);
    SecondsTimer(1.0, UpdatingUser=GlobalUser, OnUpdate=ImpulseDisplay)
}
```

### Outputs (Drives)

Define with the `out` keyword:

```
module OutputModuleExample

/// The answer to life, the universe, and everything.
out Answer: int

where {
    Answer = 42;
}
```

#### `this` Output

A special output indicating the module returns a default value. It's the final unlabeled expression in the context:

```
module ThisModuleExample

out this: string

where {
    "Some string value."
}
```

## Importing Packages

External packages require a `protograph.toml` manifest file and variation on `use`.

### ProtoGraph Manifest

Located at project root, contains metadata and dependencies:

```toml
# name and version are required if publishing as a package
name = "PackageName"
version = "0.0.0"

# List dependencies
[dependencies]
DependencyA = { uri = "https+pgzip://..." }
LocalDependency = { uri = "file://..." }
```

### Dependencies

- `file://` schema for local directories (ignored by restoration and lock file)
- `https+pgzip://` schema for remote `.pgzip` archives

#### Restoring Dependencies

```
flux-sdk restore
```

Or implicitly with `flux-sdk build` (unless `--skip-restore` is used).

Downloaded packages are stored in a global content-addressed cache. Set custom location with `PROTOGRAPH_PACKAGE_CACHE` environment variable.

#### Using Dependencies

Use `from` keyword with `use`:

```
module ModuleWithExternalDependency

from DependencyA use Full/Module/Path
```

The name after `from` is the key in the manifest `dependencies` table.

#### Lock File

Add `--lock` argument to write a lock file (`protograph.lock`) after restoring:

```
flux-sdk restore --lock
```

The lock file contains URIs and cryptographic hashes for reproducible builds. Check it into version control.

## Creating Packages

Use `flux-sdk pack` to create a `.pgzip` archive.

Before publishing:
- Include `name` and `version` in manifest
- Add metadata fields
- Customize files with `include` and `exclude` tables (glob patterns)

Default includes: `*.pg`, `protograph.*`, `LICENSE`
Default excludes: `.*` (dot files), `pgx` directory

Create a lock file before packing: `flux-sdk restore --lock`

## Cleaning Packages

```
flux-sdk clean
```

Cleans project and global packages from caches. After cleaning global cache, you'll need to clean project packages and run `restore` again.
