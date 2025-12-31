# Frequently Asked Questions

## General Questions

### What platforms and hardware does Resonite support?

Resonite is currently available on Windows and Linux. It supports all of the major headsets, including SteamVR/OpenVR, Oculus, and Windows Mixed Reality (via SteamVR).

Resonite also supports a wide range of hardware peripherals:
- Up to 64 trackers via SteamVR
- 8 for full-body tracking (feet, knees, hip, chest, and elbows)
- Additional trackers for tracking objects
- Leap Motion for finger tracking
- Eye Tracking via Vive Pro Eye and standalone modules
- HTC's lip tracking
- Controllers such as the etee controllers

### What are Resonite's hardware requirements?

**CPU:** Powerful quad-core CPU - at least Intel i5-4590 (Haswell), AMD FX 8350 (Piledriver), or newer. Strong single-core performance greatly benefits Resonite.

**RAM:** At least 8 GB recommended, 16 GB or 32 GB+ greatly beneficial.

**GPU:** VR-capable card - Nvidia GTX 1060 or AMD RX 570 recommended. Stronger GPUs increase resolution and framerate.

### Can I put Resonite in a window?

Yes! Press Alt + Enter at any time to place Resonite into a window. You can also use command line arguments:

```
-screen-fullscreen 0 -screen-width 1280 -screen-height 720
```

### Can I play Resonite on the desktop?

Yes! With no VR hardware it launches in desktop mode by default. While in VR, toggle to desktop with F8.

### Is Resonite open source?

Currently, most of Resonite is not open source.

### Is Resonite running on Unity?

Most of Resonite runs on FrooxEngine, a custom engine crafted over many years since around 2015 with around 500,000 lines of code. Unity is used primarily for its renderer and the runtime environment (Mono/.NET).

## Beginner Questions

### What are the basic controls in Resonite?

- **Joystick:** Navigation and movement
- **Trigger:** Primary actions (activating buttons)
- **Joystick/touchpad click:** Secondary actions (jumping, tool use)
- **Grip button:** Grabbing/moving objects
- **Context menu button:** Context-sensitive actions, undo/redo, locomotion modes

### How can I equip an avatar?

- From inventory: Select avatar, press "Equip avatar" in top left corner
- In world: Click on the avatar

### How do I save objects to my inventory?

Grab the object, then either open your context menu or inventory in your dash and press the blue floppy disk button. You can only save into folders you've created.

### How can I mute myself?

On your dashboard, find voice control options in the top left facet:
- **Mute:** Silences you (toggle)
- **Whisper:** Dampens outside noise, prevents others outside bubble from hearing
- **Normal:** Typical spatialized voice mode
- **Shout:** Increased volume and range
- **Broadcast:** Disables spatialization, heard from anywhere

## Avatars and Assets

### How can I import my assets?

- Drag and drop from file browser onto Resonite window
- Copy and paste asset or link
- Use "Paste Content From Clipboard" in session menu
- Navigate filesystem from File Browser in Dash Menu

### What kinds of assets does Resonite support?

Models, textures, sounds, fonts, LUTs, and more in commonly accepted formats.

### What are the rig requirements?

Resonite requires a general bone naming convention and hierarchy. Avatar rigs set up for other platforms should generally be compatible. See Humanoid rig requirements for IK for full details.

### Can I import my `.unitypackage` avatar?

Not directly. `.unitypackage` is Unity-specific. However, if your model exists as a .fbx file within the Unity project folder, you can use that instead.

### What about custom shaders?

Custom shaders are not supported as there's no way to compile JIT shaders at runtime. However, many visual effects can be achieved through ProtoFlux and components.

### Does Resonite support dynamic bones?

Yes! Use the DevTool to open your avatar, navigate to the bone to start the chain from, and attach the DynamicBoneChain component. Select "Setup From Children" at the bottom of the component.

## Resonite Features

### What is ProtoFlux?

ProtoFlux is the node-based visual scripting language of Resonite. It forms the basis of many gadgets, toys, and game mechanics. It's a powerful tool for managing and manipulating data within a world.

### Can I stream Resonite?

Yes, as long as content follows the Guidelines and platform terms. Use the "Mirror To Display" option in the Camera / Streaming tool. A LIVE badge appears over your head while enabled.

## Account Questions

### How do I get more cloud storage space?

Additional storage is a Patreon perk. $1/month grants 5 GB additional storage.

### How do I turn on two-factor authentication?

Enable 2FA from your dash Tools facet using a TOTP authenticator app like Authy or Google Authenticator.

**Important:** Protect your secret code and recovery codes. If you lose them, you'll PERMANENTLY lose access to your account!

## Troubleshooting

### What do I do if Resonite crashes/I encounter a bug?

Collect your logs and file a GitHub issue at https://github.com/Yellow-Dog-Man/Resonite-Issues/

### How can I report a Security Issue / Exploit?

Review the Security & Exploit Reporting Policy on the wiki.

Source: https://wiki.resonite.com/Frequently_Asked_Questions
