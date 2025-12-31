# Component:GiggleTechSettings

> Source: https://wiki.resonite.com/Component:GiggleTechSettings

Collapse **Component image**

[File:GiggleTechSettingsComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=GiggleTechSettingsComponent.png "File:GiggleTechSettingsComponent.png") **Giggle Tech Settings** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **GiggleTechSettings** Component is used to control different aspects of [giggle pucks](https://giggletech.io/products/giggle_puck) for use in Resonite.

See [Settings](https://wiki.resonite.com/Settings "Settings") for information.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Devices` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[GiggleTechSettings.Device](https://wiki.resonite.com/Component:GiggleTechSettings#Device)** | A list of giggle pucks with settings for them. |
| `GigglePuckIP` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | the IP address of the giggle puck. |
| `IsGigglePuckValid` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the giggle puck is valid and tracking. |

Fields
Collapse

## Device

| Name | Type | Description |
| --- | --- | --- |
| `IP` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The IP address of this device. |
| `IsConnected` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this device is connected. |
| `UseDevice` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow use and registration of this device. |
| `AlwaysTreatAsConnected` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether this puck should always be treated as connected even if it looses connection. |
| `CustomName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | A user defined name for this giggle puck. |
| `IntensityScale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The scaling for intensity. |
| `MinimumIntensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The minimum intensity needed to activate this. |
| `InitialActivationIntensity` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How strong the inital activation will be. |
| `HapticPointMapping` | _direct_ **[HapticPointMapping](https://wiki.resonite.com/index.php?title=Type:HapticPointMapping&action=edit&redlink=1 "Type:HapticPointMapping (page does not exist)")** | How this is mapped. |
| `HapticPointIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The index of this device in the list of haptic devices. |

Fields

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `RegisterGigglePuck:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | Register a gigglepuck to the list |
| `GetDeviceForSubsetting:SubsettingGetter` | **[SubsettingGetter](https://wiki.resonite.com/Type:SubsettingGetter "Type:SubsettingGetter")** | X | Get one of the `Devices` by key. |

Triggers
Collapse

## Usage

See [Settings](https://wiki.resonite.com/Settings "Settings") for information.

## Examples

See [Settings](https://wiki.resonite.com/Settings "Settings") for information.

## See Also

- [Component:SettingsFacetPreset](https://wiki.resonite.com/Component:SettingsFacetPreset "Component:SettingsFacetPreset")
- [Settings](https://wiki.resonite.com/Settings "Settings")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:GiggleTechSettings&oldid=99155](https://wiki.resonite.com/index.php?title=Component:GiggleTechSettings&oldid=99155)"

Contents