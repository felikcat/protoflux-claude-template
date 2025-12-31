# Command Line Arguments

Desktop builds of Resonite support several command line arguments. Set them within Steam launch options or use for standalone experiences.

## Forcing Specific Hardware

| Argument | Description |
|----------|-------------|
| *none* | Auto-detect hardware |
| `-Screen` | Forces screen mode |
| `-Device SteamVR` | Forces SteamVR |
| `-Device WindowsMR` | Forces Windows Mixed Reality |
| `-Device Oculus` | Forces Oculus Rift and Touch controllers |
| `-Device OculusQuest` | Forces Oculus Quest and Touch controllers |
| `-Device Screen360` | Forces screen mode with 360° projection |
| `-Device StaticCamera` | Non-interactive camera mode |
| `-Device StaticCamera360` | Non-interactive 360° equirectangular camera mode |
| `-LegacySteamVRInput` | Legacy SteamVR input (workaround for devices with bad hand skeletal model) |
| `-ForceSRAnipal` | Force SRAnipal SDK for HTC eye/lip tracking |
| `-ForceBabble` | Force Babble driver for Project Babble face tracking |

## Joining Sessions & Opening Worlds

| Argument | Description |
|----------|-------------|
| `-Join Auto` | Auto-joins active LAN sessions, follows session with most users |
| `-Join <URL>` | Joins session at provided URI on start |
| `-Open <resrec_URL>` | Opens world at provided resrec URL on start |
| `-AnnounceHomeOnLAN` | Home and userspace accessible from LAN by default |
| `-Bootstrap <class>` | Runs custom bootstrap function |

## Networking

| Argument | Description |
|----------|-------------|
| `-ForceLANOnly` | Sessions announced only on LAN, not accessible from internet |
| `-CloudProfile` | Which cloud API servers (Production, Staging, Local) |

## Drone Camera Presets

| Argument | Description |
|----------|-------------|
| `-CameraBiggestGroup` | Drone follows biggest group |
| `-CameraTimelapse` | Timelapse mode |
| `-CameraStayBehind` | Stay behind subjects |
| `-CameraStayInFront` | Stay in front of subjects |
| `-UseResoniteCamera` | Spawn as Resonite Camera with zoom/preview |

## Data Folders

| Argument | Description |
|----------|-------------|
| `-DataPath <path>` | Path to database directory |
| `-CachePath <path>` | Path to cache directory |
| `-LogsPath <path>` | Redirect log files to custom directory |

## Post Processing

| Argument | Description |
|----------|-------------|
| `-ctaa` | Enables Cinematic Temporal Anti-Aliasing |
| `-ctaaTemporalEdgePower <num>` | Sets CTAA TemporalEdgePower |
| `-ctaaSharpnessEnabled <bool>` | Enable/disable CTAA Sharpness |
| `-ctaaAptiveSharpness <num>` | Sets CTAA AptiveSharpness amount |

## Misc

| Argument | Description |
|----------|-------------|
| `-Watchdog <filepath>` | Periodically write current time to file (for restart on freeze) |
| `-LoadAssembly <path>` | Load extra CLR assembly |
| `-Kiosk` | Kiosk mode (hides userspace items, disables teleporting for guests) |
| `-NoUI` | Hides userspace UI |
| `-CubemapResolution <res>` | Force 360 rendering cubemap resolution |
| `-DoNotAutoLoadHome` | Don't auto-load cloud home on start |
| `-ResetDash` | Reset dash layout to default |
| `-SkipIntroTutorial` | Prevent intro tutorial |
| `-ForceIntroTutorial` | Force intro tutorial |
| `-Invisible` | Force invisible status on login |
| `-EngineConfig <filepath>` | Specify custom config file |
| `-Verbose` | More detailed initialization logs |
| `-ForceReticleAboveHorizon` | Disallow looking below horizon in desktop first person |

## Custom Protocol Handler (Steam only)

Open Resonite to specific location when clicking links:

```
Resonite:?world=resrec:///U-ProbablePrime/R-9ce872e1-ffb8-4194-bb91-3d3ab5f157a1
```

For platforms restricting protocol handlers, use redirect:
```
https://api.resonite.com/open/world/U-ProbablePrime/R-9ce872e1-ffb8-4194-bb91-3d3ab5f157a1
```

## How to Use Command Line Arguments

### Launching from Steam

1. Open Steam
2. Right click Resonite in library
3. Select "Properties" → "Set Launch Options"
4. Enter commands and run Resonite

### Using a Shortcut

1. Find Resonite.exe, right-click → "Create Shortcut"
2. Move shortcut somewhere convenient
3. Right-click shortcut → "Properties"
4. In "Target" text box, add space after filepath, then add arguments
5. Click "Apply" and "OK"

### Example

Combine `-Invisible` and `-CachePath`:
```
"C:\Program Files\Steam\steamapps\common\Resonite\Resonite.exe" -Invisible -CachePath "D:\Temporary files\ResoniteCache\"
```

Source: https://wiki.resonite.com/Command_line_arguments
