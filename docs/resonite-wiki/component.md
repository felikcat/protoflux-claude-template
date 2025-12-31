# Component

A **Component** is something attached to a Slot to add functionality. Without components, slots would be nothing but points in a void. They are behind almost every feature in Resonite, ranging from storing data to animating your avatar.

For a list of all components, see the Components category. Components are organized in categories that match the game.

## Basic Properties

### Fields

Components contain fields that store data for configuration, internal operation, and output.

All components include these built-in fields:

| Field | Type | Description |
|-------|------|-------------|
| `persistent` | bool | Whether this component will be saved (e.g., to Inventory). If `false`, component won't be persisted when saved. |
| `UpdateOrder` | int | Controls update order relative to all other components in the World. Higher values update after lower values. Many components don't use the common updating system. |
| `Enabled` | bool | Controls whether component is "enabled". Disabled components (`false`) generally do nothing. Not all components respect this property. |

## Working With Components

### With the Scene Inspector

Components are primarily manipulated through the Scene Inspector. It allows you to:
- Create and destroy components
- Manipulate their fields
- Access custom functionality (commonly through buttons)

**Moving/Duplicating:** Grab a component by its header and move to another scene inspector. You'll get the option to move or duplicate.

### With ProtoFlux

ProtoFlux currently has **limited ability** to directly interact with components:
- Cannot dynamically create, destroy, or locate components in slots
- Ref Hacking can attempt access but is **highly discouraged** due to its fragile nature

## See Also

- Slot - Components are attached to slots
- Scene Inspector - Primary tool for manipulating components
- Category:Components - Full list of all components

Source: https://wiki.resonite.com/Component
