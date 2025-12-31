# Component:ViolentAprilFoolsExplosion

> Source: https://wiki.resonite.com/Component:ViolentAprilFoolsExplosion

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:ViolentAprilFoolsExplosion&diff=79024) which are not marked for translation.

_This article or section is a stub. You can help the Resonite wiki by expanding it._

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/a/a7/ViolentAprilFoolsExplosionComponent.png/510px-ViolentAprilFoolsExplosionComponent.png)](https://wiki.resonite.com/File:ViolentAprilFoolsExplosionComponent.png) **ViolentAprilFoolsExplosion** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ViolentAprilFoolsExplosion** component, when deleted, causes an explosion animation to be played on any mesh below it in the hierarchy.

This component was added as an [April Fool's Day](https://en.wikipedia.org/wiki/April_Fools%27_Day) joke on April 1st, 2019.

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `BloatMagnitude` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | Intensity of the bloat, prior to explosion |
| `_bloatingClip` | **[AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip")** | _Automatically Assigned_ |
| `_explosionClip` | **[AudioClip](https://wiki.resonite.com/Type:AudioClip "Type:AudioClip")** | _Automatically Assigned_ |

Fields
Collapse

## Behavior

This component causes all [MeshRenderers](https://wiki.resonite.com/MeshRenderer_(Component) "MeshRenderer (Component)") under it in the hierarchy to expand outwards based on the `BloatMagnitude` while playing the audio in `_bloatingClip`, followed by an explosion particle effect, the playing of the audio in `_explosionClip`, and the deletion of the slot it's attached to.

## Examples

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ViolentAprilFoolsExplosion&oldid=79024](https://wiki.resonite.com/index.php?title=Component:ViolentAprilFoolsExplosion&oldid=79024)"

Contents