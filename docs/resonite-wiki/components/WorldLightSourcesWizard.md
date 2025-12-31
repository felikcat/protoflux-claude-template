# Component:WorldLightSourcesWizard

> Source: https://wiki.resonite.com/Component:WorldLightSourcesWizard

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/18/WorldLightSourcesWizardComponent.png/510px-WorldLightSourcesWizardComponent.png)](https://wiki.resonite.com/File:WorldLightSourcesWizardComponent.png) **World Light Sources Wizard** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [World Light Sources Wizard](https://wiki.resonite.com/index.php?title=World_Light_Sources_Wizard&action=edit&redlink=1 "World Light Sources Wizard (page does not exist)").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Root` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root directory in which all lights underneath it will be affected. |
| `ProcessPointLights` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to process point lights. |
| `ProcessSpotLights` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to process spot lights. |
| `ProcessDirectionalLights` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to process directional lights. |
| `ProcessDisabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to process lights that are not part of an active hiearchy or the component itself is disabled. |
| `TargetShadowType` | **[ShadowType](https://wiki.resonite.com/Type:ShadowType "Type:ShadowType")** | The shadow type to set all lights to. |
| `_tag` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | The slot tag that lights have to have under `Root` to be affected. |
| `_intensityField` | **[FloatTextEditorParser](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser")** | The intensity to set all lights under `Root` to. |
| `_rangeField` | **[FloatTextEditorParser](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser")** | The distance range to set all lights under `Root` to. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `SetShadowType:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the shadow type is set in the dialog. |
| `ChangeIntensity:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the intensity is changed in the dialog. |
| `ChangeRange:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the range is changed in the dialog. |
| `Remove:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the dialog asks to remove lights. |
| `Disable:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the dialog asks to disable lights. |
| `Enable:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Handles when the dialog asks to enable lights. |

Triggers
Collapse

## Usage

See [World Light Sources Wizard](https://wiki.resonite.com/index.php?title=World_Light_Sources_Wizard&action=edit&redlink=1 "World Light Sources Wizard (page does not exist)").

## Examples

See [World Light Sources Wizard](https://wiki.resonite.com/index.php?title=World_Light_Sources_Wizard&action=edit&redlink=1 "World Light Sources Wizard (page does not exist)").

## See Also

- [World Light Sources Wizard](https://wiki.resonite.com/index.php?title=World_Light_Sources_Wizard&action=edit&redlink=1 "World Light Sources Wizard (page does not exist)")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:WorldLightSourcesWizard&oldid=100814](https://wiki.resonite.com/index.php?title=Component:WorldLightSourcesWizard&oldid=100814)"

Contents