# Component:AssetMetadata

> Source: https://wiki.resonite.com/Component:AssetMetadata

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/8/8c/AssetMetadataComponent.png/510px-AssetMetadataComponent.png)](https://wiki.resonite.com/File:AssetMetadataComponent.png) **Asset Metadata** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `LocationName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | Name of the world the photo was taken in. |
| `LocationURL` | **[Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")** | The url of the world the photo was taken in. |
| `LocationHost` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The host user of the session the photo was taken in. |
| `LocationAccessLevel` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [SessionAccessLevel](https://wiki.resonite.com/Type:SessionAccessLevel "Type:SessionAccessLevel") >** | The access level of the world the photo was taken in. |
| `LocationHiddenFromListing` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Bool](https://wiki.resonite.com/Type:Bool "Type:Bool") >** | whether the photo was taken in a hidden world or not. |
| `TimeTaken` | **[DateTime](https://wiki.resonite.com/Type:DateTime "Type:DateTime")** | The time the photo was taken. |
| `TakenBy` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | the user who took the photo. |
| `TakenGlobalPosition` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The Position the Asset was generated in global space. |
| `TakenGlobalRotation` | **[FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ")** | The rotation the Asset was generated in global space. |
| `TakenGlobalScale` | **[Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3")** | The scale of the point this Asset was generated in global space. |
| `AppVersion` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The [Version](https://wiki.resonite.com/Category:Versions "Category:Versions") of the game the photo was taken in. |
| `UserInfos` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[AssetMetadata.UserInfo](https://wiki.resonite.com/Component:AssetMetadata#UserInfo)** | A list of users present in the session when the photo was taken. |
| `__legacyPresentUsers` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | A list of users present in the session when the photo was taken. This is internal legacy data. |

Fields
Collapse

## Sync Delegates

| Method Name | Method type and Arguments. | Is the method hidden? | Description |
| --- | --- | --- | --- |
| `SetFromCurrentWorld:Action` | **[Action](https://wiki.resonite.com/Type:Action "Type:Action")** | X | fills in all the fields using the current session data and the local user (the user running this method) |

Triggers
Collapse

## UserInfo

See [UserInfo](https://wiki.resonite.com/Type:UserInfo "Type:UserInfo").

## Usage

This component is used as a base component for other components like [PhotoMetadata](https://wiki.resonite.com/Component:PhotoMetadata "Component:PhotoMetadata")

## Examples

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AssetMetadata&oldid=97852](https://wiki.resonite.com/index.php?title=Component:AssetMetadata&oldid=97852)"

Contents