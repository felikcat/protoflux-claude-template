# Component:AssetOptimizationWizard

> Source: https://wiki.resonite.com/Component:AssetOptimizationWizard

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/6b/AssetOptimizationWizardComponent.png/510px-AssetOptimizationWizardComponent.png)](https://wiki.resonite.com/File:AssetOptimizationWizardComponent.png) **Asset Optimization Wizard** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

_This article or section is a stub. You can help the Resonite wiki by expanding it._

The component that drives the [Asset Optimization Wizard](https://wiki.resonite.com/Asset_Optimization_Wizard "Asset Optimization Wizard").

## Usage

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Root` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot specified in the generated UI for the wizard. If this is null, the wizard will use the [Root](https://wiki.resonite.com/Root "Root") slot. |
| `IgnoreNonpersistentUsers` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Ignore the contents of the slots of users in the session or not. |
| `_maxResolution` | **[IntTextEditorParser](https://wiki.resonite.com/Component:IntTextEditorParser "Component:IntTextEditorParser")** | The max resolution field that's part of the generated UI. |
| `_message` | **[Text](https://wiki.resonite.com/Component:Text "Component:Text")** | The message for the current progress and statuses of this wizard's work. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `CleanupUnusedAssets:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | see [Asset Optimization Wizard](https://wiki.resonite.com/Asset_Optimization_Wizard "Asset Optimization Wizard"). |
| `CleanupEmptySlots:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | see [Asset Optimization Wizard](https://wiki.resonite.com/Asset_Optimization_Wizard "Asset Optimization Wizard"). |
| `CleanupDisabledMeshRenderers:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | see [Asset Optimization Wizard](https://wiki.resonite.com/Asset_Optimization_Wizard "Asset Optimization Wizard"). |
| `DeduplicateMaterials:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | see [Asset Optimization Wizard](https://wiki.resonite.com/Asset_Optimization_Wizard "Asset Optimization Wizard"). |
| `OnSetMaxTextureResolution:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | see [Asset Optimization Wizard](https://wiki.resonite.com/Asset_Optimization_Wizard "Asset Optimization Wizard"). |
| `CleanupFileItems:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | see [Asset Optimization Wizard](https://wiki.resonite.com/Asset_Optimization_Wizard "Asset Optimization Wizard"). |
| `OnRecompressTextures:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | see [Asset Optimization Wizard](https://wiki.resonite.com/Asset_Optimization_Wizard "Asset Optimization Wizard"). |
| `OnRecalculateAllMikktspace:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | see [Asset Optimization Wizard](https://wiki.resonite.com/Asset_Optimization_Wizard "Asset Optimization Wizard"). |
| `OnRecalculateAllNormals:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | see [Asset Optimization Wizard](https://wiki.resonite.com/Asset_Optimization_Wizard "Asset Optimization Wizard"). |
| `OnRecalculateAllNormalsMerged:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | see [Asset Optimization Wizard](https://wiki.resonite.com/Asset_Optimization_Wizard "Asset Optimization Wizard"). |

Triggers
Collapse

## Behavior

## Examples

## See Also

- [Asset Optimization Wizard](https://wiki.resonite.com/Asset_Optimization_Wizard "Asset Optimization Wizard")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AssetOptimizationWizard&oldid=98326](https://wiki.resonite.com/index.php?title=Component:AssetOptimizationWizard&oldid=98326)"

Contents