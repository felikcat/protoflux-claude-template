# Component:CharacterColliderWorldLink

> Source: https://wiki.resonite.com/Component:CharacterColliderWorldLink

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:CharacterColliderWorldLink&diff=91413) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/e/e5/CharacterColliderWorldLinkComponent.png/510px-CharacterColliderWorldLinkComponent.png)](https://wiki.resonite.com/File:CharacterColliderWorldLinkComponent.png) **CharacterColliderWorldLink** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

Character collider world link is a component that allows for having a user trigger a world link when they collide against a collider or go into a trigger zone.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TriggersOnly` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to only allow collision events from trigger type colliders on this slot to trigger or all types of colliders to trigger this world link. |
| `OpenOnContactStart` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Use world link on contact start. |
| `OpenOnContactStay` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Use world link on contact stay. |
| `OpenOnContactEnd` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Use world link on contact end. |
| `WorldLink` | **[WorldLink](https://wiki.resonite.com/Component:WorldLink "Component:WorldLink")** | The world to open and optionally go to to on contact. |
| `LastOpened` | _direct_ **[SyncTime](https://wiki.resonite.com/Type:SyncTime "Type:SyncTime")** | Last time this world link was used. |

Fields
Collapse

## Behavior

## Examples

Useful for portals, or "teleporters".

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:CharacterColliderWorldLink&oldid=91413](https://wiki.resonite.com/index.php?title=Component:CharacterColliderWorldLink&oldid=91413)"

Contents