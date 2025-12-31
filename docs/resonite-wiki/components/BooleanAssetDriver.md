# Component:BooleanAssetDriver

> Source: https://wiki.resonite.com/Component:BooleanAssetDriver

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/3d/BooleanAssetDriver%601Component.png/510px-BooleanAssetDriver%601Component.png)](https://wiki.resonite.com/File:BooleanAssetDriver%601Component.png) **Boolean Asset Driver\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

This component is functionally identical to [Boolean Reference Driver](https://wiki.resonite.com/Component:BooleanReferenceDriver "Component:BooleanReferenceDriver"). Except it only accepts [IAssets](https://wiki.resonite.com/Type:IAsset%601 "Type:IAsset`1") and acts as a user for assets in `FalseTarget` and `TrueTarget` meaning assets assigned to this component won't get cleaned up by the asset optimizer world processes.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `State` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to drive `Target` to `TrueTarget` or `FalseTarget` |
| `Target` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[AssetRef\`1](https://wiki.resonite.com/index.php?title=Type:AssetRef%601&action=edit&redlink=1 "Type:AssetRef`1 (page does not exist)") <A>** | The field to drive the value of. |
| `FalseTarget` | **A** | The asset to drive `Target` to when `State` is false. |
| `TrueTarget` | **A** | The asset to drive `Target` to when `State` is true. |

Fields
Collapse

## Usage

Attach this component to a slot, and (optionally) put an asset into the False and/or True target fields. Then, put a field which you want to change the asset of into `Target`. now, switching `State` will allow switching between the values of `FalseTarget` and `TrueTarget`.

## Examples

This can be used to switch textures, materials, documents, and many other [IAssets](https://wiki.resonite.com/Type:IAsset%601 "Type:IAsset`1") between two different values. This can be used to allow flip flopping eye textures, or having an evil/good texture.

## See Also

[Asset Multiplexer](https://wiki.resonite.com/Component:AssetMultiplexer "Component:AssetMultiplexer") for switching between more than 2 assets.

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:BooleanAssetDriver&oldid=91258](https://wiki.resonite.com/index.php?title=Component:BooleanAssetDriver&oldid=91258)"

Contents