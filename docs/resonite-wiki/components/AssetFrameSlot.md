# Component:AssetFrameSlot

> Source: https://wiki.resonite.com/Component:AssetFrameSlot

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:AssetFrameSlot&diff=78856) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/2/21/AssetFrameSlot%601Component.png/510px-AssetFrameSlot%601Component.png)](https://wiki.resonite.com/File:AssetFrameSlot%601Component.png) **Asset Frame Slot\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

An asset frame slot is a component that takes any [Asset Type](https://wiki.resonite.com/Type:IAsset%601 "Type:IAsset`1") as an attach component type argument, and allows for snapping assets to a frame. The asset in the frame can be used as a source to drive a list of asset fields which is defined in Targets.
Optionally it calls a sync delegate that takes an argument of the chosen asset type for this component.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `FrameSize` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how thick the frame should be. |
| `FrameAnimSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | how fast the frame should fit to the asset's bounding box in seconds |
| `SnapAnimTime` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How long the animation should be for the asset going into the frame when snapped in seconds. |
| `Targets` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") < [SyncRef\`1](https://wiki.resonite.com/Type:SyncRef%601 "Type:SyncRef`1") < [IAssetProvider\`1](https://wiki.resonite.com/Type:IAssetProvider%601 "Type:IAssetProvider`1") <A>>>** | The items to drive with the snapped object's asset. |
| `Callback` | _[delegate of identity](https://wiki.resonite.com/Type:SyncDelegate%601 "Type:SyncDelegate`1")_ **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [IAssetProvider\`1](https://wiki.resonite.com/Type:IAssetProvider%601 "Type:IAssetProvider`1") <A>>** | A sync delegate that takes an argument of the chosen asset type for this component. The sync delegate is called when the asset is snapped. |
| `_current` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot of the asset item inside of the frame. |
| `_currentRatio` | **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The ratio of the asset's bounding box held in the frame |
| `_frameSize` | _[field drive](https://wiki.resonite.com/Type:FieldDrive%601 "Type:FieldDrive`1")_ of **[Float2](https://wiki.resonite.com/Type:Float2 "Type:Float2")** | The field to drive with what the size of the frame should be for the held asset's bounding box. |
| `_collider` | **[BoxCollider](https://wiki.resonite.com/Component:BoxCollider "Component:BoxCollider")** | The collider to drive the values of the size of the held asset's bounding box. |

Fields
Collapse

## Usage

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Examples

_This article or section is a stub. You can help the Resonite wiki by expanding it._

## Related Components

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AssetFrameSlot&oldid=78856](https://wiki.resonite.com/index.php?title=Component:AssetFrameSlot&oldid=78856)"

Contents