# Component:DataPreset

> Source: https://wiki.resonite.com/Component:DataPreset

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:DataPreset&diff=98418) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/b/b9/DataPresetComponent.png)](https://wiki.resonite.com/File:DataPresetComponent.png) **Data Preset** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **DataPreset** is a component that is useful for switching a list of values to a predetermined set.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `IsActive` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Indicates that all the presets in Entries have been applied. Cannot be driven. |
| `Entries` | _direct_ **[SyncRelayList\`1](https://wiki.resonite.com/index.php?title=Type:SyncRelayList%601&action=edit&redlink=1 "Type:SyncRelayList`1 (page does not exist)") < [IDataPresetEntry](https://wiki.resonite.com/Type:IDataPresetEntry "Type:IDataPresetEntry") >** | A list of data preset references and values. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `SetActive:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Set all target values targeted by `Entries` to their preset values. |
| `SetValues:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Set all preset values in `Entries` to their target values. |
| `OnSetValues:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use `SetValues` instead. |
| `OnSetActive:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Use `SetActive` instead. |
| `OnAddAllChildren:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Adds all the children preset components under this slot's hierarchy. |

Triggers
Collapse

## Usage

Each entry in the list of Entries is a [DataPresetReference](https://wiki.resonite.com/index.php?title=Componenr:DataPresetReference&action=edit&redlink=1 "Componenr:DataPresetReference (page does not exist)") <T> or a [DataPresetValue](https://wiki.resonite.com/Component:DataPresetValue "Component:DataPresetValue") <T>. These may be added manually, or, if the DataPresetReferences and DataPresetValues are components in this slot or child slots, the Add All Children button will add them for you (replacing any existing list).

Each entry consists of the value or reference, plus a target field.

The Set Active button applies all values and references to their respective target fields.

The only way to programmatically apply the preset is to use a [ProtoFlux Tool](https://wiki.resonite.com/ProtoFlux_Tool "ProtoFlux Tool"), grab the `SetActive()` [Delegate](https://wiki.resonite.com/index.php?title=Delegate&action=edit&redlink=1 "Delegate (page does not exist)"), and press the "Proxy" button in your [Context Menu](https://wiki.resonite.com/Context_menu "Context menu"), then feed a [Call](https://wiki.resonite.com/Impulses "Impulses") into the node.

## Examples

Using with clothes to make presets of clothing toggle combinations.

using it with [Dynamic Blendshape Driver Component](https://wiki.resonite.com/index.php?title=Component:DynamicBlendshapeDriver&action=edit&redlink=1 "Component:DynamicBlendshapeDriver (page does not exist)") to clear invalid blendshapes in the list.

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:DataPreset&oldid=98418](https://wiki.resonite.com/index.php?title=Component:DataPreset&oldid=98418)"

Contents