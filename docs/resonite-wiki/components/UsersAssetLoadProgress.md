# Component:UsersAssetLoadProgress

> Source: https://wiki.resonite.com/Component:UsersAssetLoadProgress

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/6/67/UsersAssetLoadProgress%601Component.png/510px-UsersAssetLoadProgress%601Component.png)](https://wiki.resonite.com/File:UsersAssetLoadProgress%601Component.png) **Users Asset Load Progress\`1** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **UsersAssetLoadProgress** component is commonly used with [ProtoFlux](https://wiki.resonite.com/ProtoFlux "ProtoFlux") to tell if a particular User has loaded an asset. The node in particular is the [Asset Load Progress](https://wiki.resonite.com/ProtoFlux:Asset_Load_Progress "ProtoFlux:Asset Load Progress") ProtoFlux node. This component takes any [IAsset](https://wiki.resonite.com/Type:IAsset "Type:IAsset") as the generic argument for the component.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Asset` | **A** | The Asset to monitor loading progress for. |
| `ProgressInfo` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[UsersAssetLoadProgress\`1.LoadProgress](https://wiki.resonite.com/Component:UsersAssetLoadProgress#LoadProgress) <A>** | A list of users in the session and their status on loading the specified `Asset`. |
| `TotalUsers` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | The total users in the session that see `Asset` exists? |
| `UsersNotLoaded` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many users haven't fully loaded `Asset`? |
| `UsersLoading` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many users are trying to load `Asset` currently? |
| `UsersPartiallyLoaded` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many users are currently in the process of downloading `Asset`? |
| `UsersFullyLoaded` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many users have finished loading `Asset`? |
| `UsersFailedToLoad` | _[raw output](https://wiki.resonite.com/Type:RawOutput%601 "Type:RawOutput`1")_ of **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | How many users failed to load `Asset` due to an error? |

Fields
Collapse

## LoadProgress

| Name | Type | Description |
| --- | --- | --- |
| `User` | _direct_ **[UserRef](https://wiki.resonite.com/Type:UserRef "Type:UserRef")** | The user this Load Progress is tracking loading for. |
| `DownloadProgress` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float](https://wiki.resonite.com/Type:Float "Type:Float") >** | If the user had begun downloading, how much have they downloaded from 0<->1? |
| `State` | **[AssetLoadState](https://wiki.resonite.com/Type:AssetLoadState "Type:AssetLoadState")** | What stage of getting the Asset `User` is at, or if they failed to get it. |

Fields

## Usage

Attach to a slot and provide an asset to `Asset` for this component to start working.

## Examples

Can be used with ProtoFlux [Asset Load Progress](https://wiki.resonite.com/ProtoFlux:Asset_Load_Progress "ProtoFlux:Asset Load Progress") node to get the loading progress of `Asset` for a particular User.

## See Also

- [Component:MeshRendererLoadStatus](https://wiki.resonite.com/Component:MeshRendererLoadStatus "Component:MeshRendererLoadStatus")
- [ProtoFlux:Asset Load Progress](https://wiki.resonite.com/ProtoFlux:Asset_Load_Progress "ProtoFlux:Asset Load Progress")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UsersAssetLoadProgress&oldid=97810](https://wiki.resonite.com/index.php?title=Component:UsersAssetLoadProgress&oldid=97810)"

Contents