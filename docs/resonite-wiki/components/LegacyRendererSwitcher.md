# Component:LegacyRendererSwitcher

> Source: https://wiki.resonite.com/Component:LegacyRendererSwitcher

Collapse **Component image**

[File:LegacyRendererSwitcherComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=LegacyRendererSwitcherComponent.png "File:LegacyRendererSwitcherComponent.png") **Legacy Renderer Switcher** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LegacyRendererSwitcher** component is used to switch between different rendering types depending on meshes.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `ParticleMesh` | _direct_ **[RelayRef\`1](https://wiki.resonite.com/Type:RelayRef%601 "Type:RelayRef`1") < [AssetRef\`1](https://wiki.resonite.com/index.php?title=Type:AssetRef%601&action=edit&redlink=1 "Type:AssetRef`1 (page does not exist)") < [Mesh](https://wiki.resonite.com/Type:Mesh "Type:Mesh") >>** | The particle mesh object when not null will use `MeshRenderer` for the renderer. |
| `BillboardRenderer` | **[BillboardParticleRenderer](https://wiki.resonite.com/Component:BillboardParticleRenderer "Component:BillboardParticleRenderer")** | Can be switched to in order to render the particles as squares. |
| `MeshRenderer` | **[MeshParticleRenderer](https://wiki.resonite.com/Component:MeshParticleRenderer "Component:MeshParticleRenderer")** | Can be switched to in order to render the particles as meshes. |
| `RendererDrive` | _direct_ **[RefDrive\`1](https://wiki.resonite.com/index.php?title=Type:RefDrive%601&action=edit&redlink=1 "Type:RefDrive`1 (page does not exist)") < [IParticleRenderer](https://wiki.resonite.com/Type:IParticleRenderer "Type:IParticleRenderer") >** | Drives the target field with `BillboardRenderer` or `MeshRenderer` depending on if `ParticleMesh` is null. |

Fields
Collapse

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LegacyRendererSwitcher&oldid=99178](https://wiki.resonite.com/index.php?title=Component:LegacyRendererSwitcher&oldid=99178)"

Contents