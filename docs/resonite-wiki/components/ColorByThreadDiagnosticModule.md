# Component:ColorByThreadDiagnosticModule

> Source: https://wiki.resonite.com/Component:ColorByThreadDiagnosticModule

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/6c/ColorByThreadDiagnosticModuleComponent.png/510px-ColorByThreadDiagnosticModuleComponent.png)](https://wiki.resonite.com/File:ColorByThreadDiagnosticModuleComponent.png) **Color By Thread Diagnostic Module** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ColorByThreadDiagnosticModule** component makes particles colored based on what the thread is doing and/or what thread they are a part of as part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") Simulation.

This component is part of the [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust") system made by [Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |

Fields
Collapse

## Usage

Attach to a slot, add to the list of modules in a [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem"), and adjust the values to make the desired effect from this component.

## Examples

Used to debug particles and what threads they are a part of or what their thread is doing.

## See Also

- [Component:ParticleSystem](https://wiki.resonite.com/Component:ParticleSystem "Component:ParticleSystem")
- [Photon Dust](https://wiki.resonite.com/Photon_Dust "Photon Dust")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ColorByThreadDiagnosticModule&oldid=96030](https://wiki.resonite.com/index.php?title=Component:ColorByThreadDiagnosticModule&oldid=96030)"

Contents