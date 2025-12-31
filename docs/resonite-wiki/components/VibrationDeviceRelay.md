# Component:VibrationDeviceRelay

> Source: https://wiki.resonite.com/Component:VibrationDeviceRelay

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/3/3d/VibrationDeviceRelayComponent.png/510px-VibrationDeviceRelayComponent.png)](https://wiki.resonite.com/File:VibrationDeviceRelayComponent.png) **Vibration Device Relay** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **VibrationDeviceRelay** component recieves haptics events and relays them to other vibration recievers.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `TargetComponent` | **[IVibrationDeviceComponent](https://wiki.resonite.com/index.php?title=Type:IVibrationDeviceComponent&action=edit&redlink=1 "Type:IVibrationDeviceComponent (page does not exist)")** | The component to relay the vibration event to. |
| `DynamicLookupTarget` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to look for components in to send the vibration event to. |

Fields
Collapse

## Usage

Attach to a slot like the hands or other slots that can recieve haptics, then specify a target or component that the vibrations should be relayed to.

## Examples

Could be used for a user haptics share system.

## See Also

- [Haptics](https://wiki.resonite.com/Haptics "Haptics")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:VibrationDeviceRelay&oldid=100830](https://wiki.resonite.com/index.php?title=Component:VibrationDeviceRelay&oldid=100830)"

Contents