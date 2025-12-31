# Component:AvatarNameplateVisibilityDriver

> Source: https://wiki.resonite.com/Component:AvatarNameplateVisibilityDriver

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AvatarNameplateVisibilityDriver&diff=91181) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/9/9b/AvatarNameplateVisibilityDriverComponent.png/510px-AvatarNameplateVisibilityDriverComponent.png)](https://wiki.resonite.com/File:AvatarNameplateVisibilityDriverComponent.png) **AvatarNameplateVisibilityDriver** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

AvatarNameplateVisibilityDriver is used to drive the visibility of nameplates during certain scenarios.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `AlwaysShowToContacts` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Show to contacts regardless of whether it should be hidden or not. |
| `Visible` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | The boolean to drive for nameplate visiblity (like the active of the nameplate slot) |

Fields
Collapse

## Behavior

This disables the target of `Visible` when nameplates are hidden locally through the nameplate visibility facet on the Home tab of the [Dash Menu](https://wiki.resonite.com/Dash_Menu "Dash Menu"). This also drives the visibility of nameplates for other reasons, like when visibility of default nameplates is needed locally. It also hides the target nameplate during certain render contexts, like when a user is taking a picture with hide nameplates during pictures setting turned on.

## Examples

User default nameplates, and custom nameplates use this component so the nameplate is hidden when needed. Some users may inform you that your nameplate is broken if this component isn't being utilized on it.

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AvatarNameplateVisibilityDriver&oldid=91181](https://wiki.resonite.com/index.php?title=Component:AvatarNameplateVisibilityDriver&oldid=91181)"

Contents