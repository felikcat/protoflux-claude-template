# Component:UserRoot

> Source: https://wiki.resonite.com/Component:UserRoot

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:UserRoot&diff=98212) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/5d/UserRootComponent.png/510px-UserRootComponent.png)](https://wiki.resonite.com/File:UserRootComponent.png) **User Root** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UserRoot** component can be found on the top [slot](https://wiki.resonite.com/Slot "Slot") of a [user](https://wiki.resonite.com/User "User"), this component references the user's [AvatarRenderSettings](https://wiki.resonite.com/Component:AvatarRenderSettings "Component:AvatarRenderSettings"), [ScreenController](https://wiki.resonite.com/Component:ScreenController "Component:ScreenController") and any current [AvatarUserRootOverrideAssigners](https://wiki.resonite.com/Component:AvatarUserRootOverrideAssigner "Component:AvatarUserRootOverrideAssigner").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `RenderSettings` | **[IRenderSettingsSource](https://wiki.resonite.com/index.php?title=Type:IRenderSettingsSource&action=edit&redlink=1 "Type:IRenderSettingsSource (page does not exist)")** | The user's render settings. Usually part of an avatar. |
| `ScreenController` | **[ScreenController](https://wiki.resonite.com/Component:ScreenController "Component:ScreenController")** | The screen controller that the user is using to control the game. |
| `OverrideRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot currently overriding the user's root position locally for rendering. |
| `OverrideView` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot currently overriding the user's view position locally for rendering. |
| `OverrideEars` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot currently overriding the user's ears position locally for rendering audio. |

Fields
Collapse

## UserNode

| Name | Value | Description |
| --- | --- | --- |
| `None` | 0 | Do operations based off of no user node. |
| `Root` | 1 | Do operations based off of the user root slot. |
| `GroundProjectedHead` | 2 | Do operations based off of the user's head projected to the ground and use the hit normal too. |
| `Head` | 3 | Do operations based off of user head. |
| `Hips` | 4 | Do operations based off of user hips. |
| `Feet` | 5 | Do operations based off of between user feet. |
| `View` | 6 | Do operations based off of user view. |

Values

## Usage

Usually users find the slot containing this component by using the [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") node [User Root Slot](https://wiki.resonite.com/ProtoFlux:User_Root_Slot "ProtoFlux:User Root Slot").

## Examples

Found in the user root slot of users in the [world](https://wiki.resonite.com/World "World").

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UserRoot&oldid=98212](https://wiki.resonite.com/index.php?title=Component:UserRoot&oldid=98212)"

Contents