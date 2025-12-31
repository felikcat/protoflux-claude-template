# Component:ModelImportDialog

> Source: https://wiki.resonite.com/Component:ModelImportDialog

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/1/18/ModelImportDialogComponent.png/510px-ModelImportDialogComponent.png)](https://wiki.resonite.com/File:ModelImportDialogComponent.png) **Model Import Dialog** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **ModelImportDialog** component is better explained at [Importing](https://wiki.resonite.com/Importing "Importing").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `path` | _[list](https://wiki.resonite.com/Type:SyncDelegateList%601 "Type:SyncDelegateList`1")_ of **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [UIBuilder](https://wiki.resonite.com/index.php?title=Type:UIBuilder&action=edit&redlink=1 "Type:UIBuilder (page does not exist)") >** | A list of sync delegates used to generate the UI when at particular paths in the importer. |
| `_contentRoot` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The slot to put ui elements for import options in. |
| `_scale` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | The scale of the model being imported. |
| `_autoScale` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to use auto scale to humanoid height |
| `_material` | **[ModelImportDialog.MaterialType](https://wiki.resonite.com/Component:ModelImportDialog#MaterialType)** | What kind of material to import the materials for the model as. |
| `_preferSpecular` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the importer should prefer to use specular materials. |
| `_rig` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the model has a rig or not. |
| `_setupIK` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether IK should be set up. |
| `_debugRig` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to debug the rig bones after import. |
| `_colliders` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to add auto generated colliders. |
| `_animations` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to import animations. |
| `_snappable` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to import the model as separate snappable pieces |
| `_timelapse` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to import animations as timelapses |
| `_externalTextures` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to look for external textures when importing |
| `_grabbable` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to import the model as grabbable |
| `_scalable` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to import the model as scalable. |
| `_importAtOrigin` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to import the model centered at the world origin |
| `_forceTpose` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to enforce a t-pose on an IK model when importing |
| `_assetsOnObject` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to place the asset components on the avatar itself under a list of slots, or place them under the world assets and have them be optimized automatically. |
| `_asPointCloud` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to import as a point cloud. |
| `_importImagesByName` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to import images by name. |
| `_importImageAlignment` | **[ModelImportDialog.AlignmentAxis](https://wiki.resonite.com/Component:ModelImportDialog#AlignmentAxis)** | Which axis import the image objects along. |
| `_calculateNormals` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to calculate new normals on import. |
| `_calculateTangents` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to calculate new tangents on import. |
| `_calculateTextureAlpha` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to calculate new texture alpha/transparency on import. |
| `_importVertexColors` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to import vertex color data for the model. |
| `_importAlbedoColor` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to import material solid albedo color data on import |
| `_importEmissive` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to import material solid emissive color data on import. |
| `_importBones` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to import model rig bones on import. |
| `_importLights` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to import model light objects on import. |
| `_makeDualSided` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to import the model as dual sided geometry. |
| `_makeFlatShaded` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to import the model geometry as flat shaded rather than smooth shaded. |
| `_deduplicateInstances` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to deduplicate duplicate data on the mesh like cubes or models in the same place and size. |
| `_optimizeModel` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to do some small optimizations to the model or not. |
| `_splitSubmeshes` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to split the model by material or not. |
| `_generateRandomColors` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to generate random colors per material for identification or not. |
| `_spawnMaterialOrbs` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to spawn material orb objects per material for easy access. |
| `_maxTextureSize` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The max texture size to restrict textures to on the model during import. |
| `_textureConversion` | **[TextureConversion](https://wiki.resonite.com/Type:TextureConversion "Type:TextureConversion")** | What kind of texture format to convert imported textures to. |
| `_forcePointFiltering` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to force point filtering on textures (Pixel art) |
| `_forceNoMipMaps` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to disable texture resolution reduction by distance optimization. |
| `_forceUncompressed` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to disable compression on assets and textures or not. |
| `ForceAsPointCloud` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to enforce importing the model as a point cloud or not. |
| `PotentialGaussianSplat` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to interpret the data as a gaussian splat. |
| `_flipY` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to flip the gaussian splat on the Y axis. |
| `_encodeSPZ` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the gaussian splat is an SPZ format. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| ``OpenRoot:Action`1<UIBuilder>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [UIBuilder](https://wiki.resonite.com/index.php?title=Type:UIBuilder&action=edit&redlink=1 "Type:UIBuilder (page does not exist)") >** | ✓ | Called when the root menu needs generating. |
| `Preset_3DModel:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the 3d model preset button is touched. |
| `Preset_VertexColorModel:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the vertex color model preset button is touched. |
| ``Menu3DModel:Action`1<UIBuilder>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [UIBuilder](https://wiki.resonite.com/index.php?title=Type:UIBuilder&action=edit&redlink=1 "Type:UIBuilder (page does not exist)") >** | ✓ | called when the 3d model menu needs generating. |
| ``MenuFinishImport:Action`1<UIBuilder>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [UIBuilder](https://wiki.resonite.com/index.php?title=Type:UIBuilder&action=edit&redlink=1 "Type:UIBuilder (page does not exist)") >** | ✓ | Is called when the finish import menu needs generating. |
| `OpenAdvancedSettings:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the advanced settings button is touched. |
| `Preset_Regular3DModel:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the regular model preset button is touched. |
| `Preset_Separable3DModel:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the separate snappable pieces preset button is touched. |
| `Preset_3DScan:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the 3d scan preset button is touched. |
| `Preset_CADModel:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the CAD preset button is touched. |
| `Preset_PointCloud:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the point cloud preset button is touched. |
| `Preset_GaussianSplat:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the gaussian splat preset button is touched. |
| ``MenuGaussianSplatVertical:Action`1<UIBuilder>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [UIBuilder](https://wiki.resonite.com/index.php?title=Type:UIBuilder&action=edit&redlink=1 "Type:UIBuilder (page does not exist)") >** | ✓ | Called when the vertical gaussian splat menu needs generating |
| ``MenuGaussianSplatEncoding:Action`1<UIBuilder>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [UIBuilder](https://wiki.resonite.com/index.php?title=Type:UIBuilder&action=edit&redlink=1 "Type:UIBuilder (page does not exist)") >** | ✓ | called when the gaussian splat encoding menu needs generating. |
| ``MenuScale:Action`1<UIBuilder>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [UIBuilder](https://wiki.resonite.com/index.php?title=Type:UIBuilder&action=edit&redlink=1 "Type:UIBuilder (page does not exist)") >** | ✓ | called when the scaling menu needs generating. |
| `ScaleAuto:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the Scale auto button is touched. |
| `ScaleHumanoid:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the Scale humanoid button is touched. |
| `ScaleMeters:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the scale meters button is touched. |
| `ScaleMillimeters:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the scale millimeters button is touched. |
| `ScaleCentimeters:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the scale centimeters button is touched. |
| `ScaleInches:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the scale inches button is touched. |
| `OpenCustom:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the custom import settings button is touched. |
| ``MenuCustom:Action`1<UIBuilder>`` | **[Action\`1](https://wiki.resonite.com/Type:Action%601 "Type:Action`1") < [UIBuilder](https://wiki.resonite.com/index.php?title=Type:UIBuilder&action=edit&redlink=1 "Type:UIBuilder (page does not exist)") >** | ✓ | Called when the custom import settings menu needs generating. |
| `MulScale:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the multiply scale by 10X button is touched. |
| `DivScale:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the div scale by 10X button is touched. |
| `RunImport:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the run import button is touched. |
| `Import_RegularVerticalSplat:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the import regular vertical splat button is touched. |
| `Import_FlipVerticalSplat:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the import flipped vertical splat button is touched. |
| `Import_SplatLossless:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the import splat lossless button is touched. |
| `Import_SplatSPZ:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the import splat SPZ button is touched. |
| `AsRawFile:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the import as raw file button is touched. |
| `Return:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the return to previous button is touched. |

Triggers
Collapse

## AlignmentAxis

| Name | Value | Description |
| --- | --- | --- |
| `PosX` | 0 | Import items along the Positive X axis. |
| `PosY` | 1 | Import items along the Positive Y axis. |
| `PosZ` | 2 | Import items along the Positive Z axis. |
| `NegX` | 3 | Import items along the Negative X axis. |
| `NegY` | 4 | Import items along the Negative Y axis. |
| `NegZ` | 5 | Import items along the Negative Z axis. |

Values

## MaterialType

| Name | Value | Description |
| --- | --- | --- |
| `PBS` | 0 | Materials should be imported as PBS metallic or specular. |
| `PBS_DualSided` | 1 | Materials should be imported as PBS dual sided metallic or specular. |
| `PBS_Triplanar` | 2 | Materials should be imported as PBS triplanar metallic or specular. |
| `PBS_Emissive` | 3 | Materials should be imported as PBS emissive metallic or specular. |
| `Unlit` | 4 | Materials should be imported as unlit. |
| `UnlitDualSided` | 5 | Materials should be imported as Unlit dual sided. |
| `UnlitBillboard` | 6 | Materials should be imported as Unlit per vertex billboard. |
| `XiexeToon` | 7 | Materials should be imported as Xiexe Toon. |
| `XiexeToonOutline` | 8 | Materials should be imported as Xiexe Toon with an outline. |
| `Wireframe` | 9 | Materials should be imported as wireframe. |

Values

Called when the button is touched.

## Usage

See [Importing](https://wiki.resonite.com/Importing "Importing").

## Examples

See [Importing](https://wiki.resonite.com/Importing "Importing").

## See Also

- [Importing](https://wiki.resonite.com/Importing "Importing")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:ModelImportDialog&oldid=99080](https://wiki.resonite.com/index.php?title=Component:ModelImportDialog&oldid=99080)"

Contents