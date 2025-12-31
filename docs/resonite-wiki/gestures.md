# Gestures (Facial Animations)

Facial animations in Resonite show expression on your avatar - from stars in eyes when pressing a button, to automatic confused looks when tilting head, to ears flopping down when frowning with a facial tracker.

## Keyboard-Based Gestures

Use any keyboard key to control expressions via ProtoFlux.

### Basic Setup

1. Plug a Key enum into **Key Pressed** node
2. Connect to **Fire On True** with user to check (usually **Get Active User Self**)
3. For key release: Use **Key Released** + **Fire On False**
4. Combine both impulses with **Data Model Boolean Toggle** for key state boolean

### Using the Output

- Plug into **Switches/Conditional** for branching logic
- Use **Zero One** to convert boolean to numbers
- Drive: facial expressions, shapekeys, materials, or bone positions

## Controller Button-Based Gestures

Many ProtoFlux nodes provide controller inputs:

| Node | Description |
|------|-------------|
| **Standard Controller** | Generic controller inputs |
| **Index Controller** | Valve Index specific |
| **Touch Controller** | Oculus Touch specific |

These provide:
- **Booleans** for button inputs
- **Float2s** for joystick positions
- TouchPad thumb position (Index)

Use with boolean logic nodes and math nodes to drive expressions.

## Body Gesture-Based

Use rotation or pointing direction of body limbs to drive expressions.

Useful nodes from:
- **Vector math** category
- **Transform** category

Good for users with:
- Only one controller
- Missing controller support
- No hands to use controllers

## Facial Tracker-Based

Resonite supports almost every facial tracker on the market.

### Supported Trackers

| Tracker | Supported | Limitations | Notes |
|---------|-----------|-------------|-------|
| Vive standalone tracker | Yes | None | Native support |
| Quest Pro | Yes | Steam Link only | Mod available for Virtual Desktop |
| Vive Pro Eye | Yes | None | Native support |

### How It Works

1. Connect facial tracker with its native driver software
2. Resonite automatically hooks in
3. Avatars with facial tracking support automatically animate

Facial movements are driven by the **AvatarExpressionDriver** component.

### Advanced Usage

You can use AvatarExpressionDriver to:
- Drive a ValueField component instead of shapekeys
- Use that field as input to ProtoFlux or other components

Source: https://wiki.resonite.com/Gestures
