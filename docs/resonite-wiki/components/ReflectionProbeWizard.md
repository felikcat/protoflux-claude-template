# Component:ReflectionProbeWizard

> Source: https://wiki.resonite.com/Component:ReflectionProbeWizard

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/5/5d/ReflectionProbeWizardComponent.png/510px-ReflectionProbeWizardComponent.png)](https://wiki.resonite.com/File:ReflectionProbeWizardComponent.png) **Reflection Probe Wizard** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

See [Reflection Probe Wizard](https://wiki.resonite.com/index.php?title=Reflection_Probe_Wizard&action=edit&redlink=1 "Reflection Probe Wizard (page does not exist)") for more up to date info

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Root` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root slot in which all probes in it's hierarchy should be baked. |
| `ProcessDisabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to bake probes in disabled hierarchies. |
| `TeleportUserToProbe` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to teleport the user to the probe before baking. |
| `_tag` | **[TextField](https://wiki.resonite.com/Component:TextField "Component:TextField")** | Probes only with this tag will be baked. |
| `_delayBetweenProbes` | **[FloatTextEditorParser](https://wiki.resonite.com/Component:FloatTextEditorParser "Component:FloatTextEditorParser")** | How long to wait between baking probes. |
| `_bakeCount` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The number of probes baked |
| `_bakeIndex` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The current probe being baked. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnShowDebugVisuals:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the show debug visuals button is touched. |
| `OnHideDebugVisuals:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the hide debug visuals button is touched. |
| `OnBakeAll:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the bake all button is touched. |

Triggers
Collapse

## Usage

See [Reflection Probe Wizard](https://wiki.resonite.com/index.php?title=Reflection_Probe_Wizard&action=edit&redlink=1 "Reflection Probe Wizard (page does not exist)").

## Examples

See [Reflection Probe Wizard](https://wiki.resonite.com/index.php?title=Reflection_Probe_Wizard&action=edit&redlink=1 "Reflection Probe Wizard (page does not exist)").

## See Also

- [Reflection Probe Wizard](https://wiki.resonite.com/index.php?title=Reflection_Probe_Wizard&action=edit&redlink=1 "Reflection Probe Wizard (page does not exist)")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ReflectionProbeWizard&oldid=99147](https://wiki.resonite.com/index.php?title=Component:ReflectionProbeWizard&oldid=99147)"

Contents