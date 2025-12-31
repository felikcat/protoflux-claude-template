# Component:PhotoMetadata

> Source: https://wiki.resonite.com/Component:PhotoMetadata

This page contains [changes](https://wiki.resonite.com/index.php?title=Component:PhotoMetadata&diff=99086) which are not marked for translation.

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d9/PhotoMetadataComponent.png/510px-PhotoMetadataComponent.png)](https://wiki.resonite.com/File:PhotoMetadataComponent.png) **Photo Metadata** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **PhotoMetadata** component is used to contain the information on a photo usually taken within Resonite. It is automatically attached to every screenshot taken using the finger photo gesture. This component can also be attached to a photo imported with the "import as screenshot" option when importing an image.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `LocationName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Name of the session the screenshot was taken in. |
| `LocationURL` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The URI of the session's world that the photo was taken in. (basically a world link) |
| `LocationHost` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | Host of the session the screenshot was taken in. |
| `LocationAccessLevel` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [SessionAccessLevel](https://wiki.resonite.com/Type:SessionAccessLevel "Type:SessionAccessLevel") >** | Access level of the session. |
| `LocationHiddenFromListing` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | Whether the location was marked as hidden. |
| `TimeTaken` | **[DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime")** | Exact timestamp that the screenshot was taken. |
| `TakenBy` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | User who took the screenshot. |
| `TakenGlobalPosition` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The position in [global space](https://wiki.resonite.com/Coordinate_spaces "Coordinate spaces") the camera had when the photo was taken. |
| `TakenGlobalRotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation in [global space](https://wiki.resonite.com/Coordinate_spaces "Coordinate spaces") the camera had when the photo was taken. |
| `TakenGlobalScale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The scale in [global space](https://wiki.resonite.com/Coordinate_spaces "Coordinate spaces") the camera had when the photo was taken. |
| `AppVersion` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Resonite version number of the photographer. |
| `UserInfos` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[AssetMetadata.UserInfo](https://wiki.resonite.com/Component:AssetMetadata#UserInfo "Component:AssetMetadata")** | See [UserInfo](https://wiki.resonite.com/Type:UserInfo "Type:UserInfo") |
| `__legacyPresentUsers` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | Internal. no longer used. |
| `CameraManufacturer` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Manufacturer of the camera. |
| `CameraModel` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Model of the camera. |
| `CameraFOV` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | FOV of the camera at picture time. |
| `Is360` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the image is a 360 degree image or not. |
| `StereoLayout` | **[StereoLayout](https://wiki.resonite.com/Type:StereoLayout "Type:StereoLayout")** | The layout of the image's left and right sections if it is a stereoscopic image, also known as a 3D image. |
| `_exportedUsers` | _[unordered list](https://wiki.resonite.com/Type:SyncBag%601 "Type:SyncBag`1")_ of **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | This is a list of users that exported the screenshot. If this component is part of a saved item, this is the list of users that exported the screenshot before the item was saved to the cloud. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `OnSavePhoto:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the save photo button is touched. |
| `OnExportPhoto:ButtonEventHandler` | **[ButtonEventHandler](https://wiki.resonite.com/index.php?title=Type:ButtonEventHandler&action=edit&redlink=1 "Type:ButtonEventHandler (page does not exist)")** | ✓ | Called when the export photo button is touched. |
| `SetFromCurrentWorld:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | fills in all the fields using the current session data and the local user (the user running this method) |

Triggers
Collapse

## Examples

- [![The PhotoMetadata component on a screenshot.](https://wiki.resonite.com/images/thumb/a/a8/Component_AssetMetadata_Example_1.webp/480px-Component_AssetMetadata_Example_1.webp.png)](https://wiki.resonite.com/File:Component_AssetMetadata_Example_1.webp "The PhotoMetadata component on a screenshot.")

The PhotoMetadata component on a screenshot.


## See Also

- [Component:FileMetadata](https://wiki.resonite.com/Component:FileMetadata "Component:FileMetadata")
- [Component:AssetMetadata](https://wiki.resonite.com/Component:AssetMetadata "Component:AssetMetadata")
- [Component:AudioMetadata](https://wiki.resonite.com/Component:AudioMetadata "Component:AudioMetadata")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:PhotoMetadata&oldid=99086](https://wiki.resonite.com/index.php?title=Component:PhotoMetadata&oldid=99086)"

Contents