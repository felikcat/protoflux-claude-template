# Component:ProceduralAssetMetadata

> Source: https://wiki.resonite.com/Component:ProceduralAssetMetadata

Collapse **Component image**

[File:ProceduralAssetMetadataComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ProceduralAssetMetadataComponent.png "File:ProceduralAssetMetadataComponent.png") **Procedural Asset Metadata** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The ProceduralAssetMetadata component is shown in the inspector for procedural meshes and textures.[\[1\]](https://wiki.resonite.com/Component:ProceduralAssetMetadata#cite_note-1)

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Asset` | **[ProceduralAssetProvider\`1](https://wiki.resonite.com/index.php?title=Type:ProceduralAssetProvider%601&action=edit&redlink=1 "Type:ProceduralAssetProvider`1 (page does not exist)") <A>** | The procedural asset to get data on. |
| `UpdateCount` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many times `Asset` has been updated since generation. |
| `Error` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether `Asset` ran into an error when generating. |

Fields
Collapse

1. [↑](https://wiki.resonite.com/Component:ProceduralAssetMetadata#cite_ref-1 "Jump up")Component was given this functionality in [Beta 2024.1.12.1336](https://wiki.resonite.com/Beta_2024.1.12.1336 "Beta 2024.1.12.1336")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ProceduralAssetMetadata&oldid=94839](https://wiki.resonite.com/index.php?title=Component:ProceduralAssetMetadata&oldid=94839)"

Contents