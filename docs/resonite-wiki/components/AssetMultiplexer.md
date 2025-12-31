# Component:AssetMultiplexer

> Source: https://wiki.resonite.com/Component:AssetMultiplexer

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AssetMultiplexer&diff=108369) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/30/AssetMultiplexer%601Component.png/510px-AssetMultiplexer%601Component.png)](https://wiki.resonite.com/File:AssetMultiplexer%601Component.png) **Asset Multiplexer\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **AssetMultiplexer** component is used to drive an asset field from a list of assets and an index within the list.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Target` | _[reference drive](https://wiki.resonite.com/Type:DriveRef%601 "Type:DriveRef`1")_ of **[AssetRef\`1](https://wiki.resonite.com/index.php?title=Type:AssetRef%601&action=edit&redlink=1 "Type:AssetRef`1 (page does not exist)") <A>** | The field to drive. |
| `Index` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Which element in `Assets` to drive to `Target` |
| `Assets` | _[list](https://wiki.resonite.com/Type:SyncAssetList%601 "Type:SyncAssetList`1")_ of **A** | The list of assets to multiplex between. |

Fields
Collapse

## Usage

Add the list of assets you want to use through the SyncAssetList<IAsset\`1> area, then add in your assets into the items. Then you can specify the field through the Target you wanna switch between different assets for. Changing the Index will change which asset the Target has in it.

Ensure you can set the Target field on this component before making any other components reference the Index field on this component if you don't wanna waste your time.

![](https://wiki.resonite.com/images/d/dd/InformationIcon.svg)

This component directly drives a value, not a reference. Therefore, trying to combine it with other components using an [IAssetProvider](https://wiki.resonite.com/Type:IAssetProvider "Type:IAssetProvider") <T> type, such as a [ReferenceMultiDriver](https://wiki.resonite.com/Component:ReferenceMultiDriver "Component:ReferenceMultiDriver"), will not work. To drive by reference and thus interop this component, use a [ReferenceMultiDriver](https://wiki.resonite.com/Component:ReferenceMultiDriver "Component:ReferenceMultiDriver") <IAssetProvider<T>>


## Examples

Using an asset multiplexer to allow your avatar to switch shirts via changing the texture, a pattern changer for a music visualizer.

To do texture swapping, use AssetMultiplexer< [Type:ITexture2D](https://wiki.resonite.com/Type:ITexture2D "Type:ITexture2D") >, not to be confused with AssetMultiplexer< [Type:Texture2D](https://wiki.resonite.com/Type:Texture2D "Type:Texture2D") >

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AssetMultiplexer&oldid=108369](https://wiki.resonite.com/index.php?title=Component:AssetMultiplexer&oldid=108369)"

Contents