# Component:FootstepSoundPlayer

> Source: https://wiki.resonite.com/Component:FootstepSoundPlayer

Collapse **Component image**

[File:FootstepSoundPlayerComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=FootstepSoundPlayerComponent.png "File:FootstepSoundPlayerComponent.png") **Footstep Sound Player** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **FootstepSoundPlayer** component triggers a list of [IFootstepSoundMaterials](https://wiki.resonite.com/Type:IFootstepSoundMaterial "Type:IFootstepSoundMaterial") when a player walks on a collider on the same slot.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `SoundMaterials` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[IFootstepSoundMaterial](https://wiki.resonite.com/Type:IFootstepSoundMaterial "Type:IFootstepSoundMaterial")** | usually a list of [FootstepSoundDefinitions](https://wiki.resonite.com/Component:FootstepSoundDefinition "Component:FootstepSoundDefinition"). |

Fields
Collapse

## Usage

Used to make an entire collider like a tile floor play sounds when a player walks on it.

## Examples

Can be used for tile floors or grid spaces.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:FootstepSoundPlayer&oldid=94757](https://wiki.resonite.com/index.php?title=Component:FootstepSoundPlayer&oldid=94757)"

Contents