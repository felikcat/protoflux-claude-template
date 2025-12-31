# ProtoFlux:AssetLoadProgress

> Source: https://wiki.resonite.com/ProtoFlux:AssetLoadProgress

AssetLoadProgress

Tracker

Download Progress

User

LoadState

Assets

Asset Load Progress is a node that allows for the reading on weither or not a user has loaded an asset. This node takes a [UsersAssetLoadProgress\`1](https://wiki.resonite.com/Component:UsersAssetLoadProgress "Component:UsersAssetLoadProgress") component and allows for the extraction of the load progress of a certain [User](https://wiki.resonite.com/Type:User "Type:User").

This can be highly useful in controlling the execution or visibility of content in a world or item. You can use this to control if a user is allowed to continue with something, interact with something, or see something.

The provided Tracker ( [UsersAssetLoadProgress\`1](https://wiki.resonite.com/Component:UsersAssetLoadProgress "Component:UsersAssetLoadProgress")) component is where the asset is referenced.

## Inputs

### Tracker ( [UsersAssetLoadProgress\`1](https://wiki.resonite.com/Component:UsersAssetLoadProgress "Component:UsersAssetLoadProgress"))

The [UsersAssetLoadProgress\`1](https://wiki.resonite.com/Component:UsersAssetLoadProgress "Component:UsersAssetLoadProgress") component to use for tracking an asset's load progress

### User ( [User](https://wiki.resonite.com/Type:User "Type:User"))

The [User](https://wiki.resonite.com/Type:User "Type:User") to check loading progress and status on for the provided Tracker ( [UsersAssetLoadProgress\`1](https://wiki.resonite.com/Component:UsersAssetLoadProgress "Component:UsersAssetLoadProgress")).

## Outputs

### DownloadProgress ( [Float? (Nullable\`1)](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1"))

The download progress a User ( [User](https://wiki.resonite.com/Type:User "Type:User")) has on the Tracker ( [UsersAssetLoadProgress\`1](https://wiki.resonite.com/Component:UsersAssetLoadProgress "Component:UsersAssetLoadProgress")), or null if they don't exist or they haven't started downloading yet.

### LoadState ( [Asset Load State](https://wiki.resonite.com/Type:AssetLoadState "Type:AssetLoadState"))

The load state of the Tracker ( [UsersAssetLoadProgress\`1](https://wiki.resonite.com/Component:UsersAssetLoadProgress "Component:UsersAssetLoadProgress")) for the provided User ( [User](https://wiki.resonite.com/Type:User "Type:User"))

## Examples

- [An example of an Asset Load Progress making a shield around an avatar with a loading bar until it has loaded the body mesh.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ProtoFlux_examples_Asset_Load_Progress_Avatar.webp "File:ProtoFlux examples Asset Load Progress Avatar.webp")

An example of an Asset Load Progress making a shield around an avatar with a loading bar until it has loaded the body mesh.

- [The code used in the example for an avatar loading bar](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=ProtoFlux_examples_Asset_Load_Progress_Code.webp "File:ProtoFlux examples Asset Load Progress Code.webp")

The code used in the example for an avatar loading bar


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:AssetLoadProgress&oldid=113013](https://wiki.resonite.com/index.php?title=ProtoFlux:AssetLoadProgress&oldid=113013)"

Contents