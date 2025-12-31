# ProtoFlux:RenderToTextureAsset

> Source: https://wiki.resonite.com/ProtoFlux:RenderToTextureAsset

Render To Texture Asset

\*

OnRenderStarted

Camera

OnRendered

Resolution

OnFailed

Format

RenderedAssetURL

Quality

Rendering

The `Render To Texture Asset` node takes in a provided [Camera](https://wiki.resonite.com/Camera_(Component) "Camera (Component)"), resolution, file format, and quality for the texture. Then this node will attempt to render it into a texture, and returns the asset URL for the world to use.

## Inputs

### \\* ( [AsyncCall](https://wiki.resonite.com/Impulses "Impulses"))

Calls an impulse to render a texture.

### Camera ( [Camera](https://wiki.resonite.com/index.php?title=Type:Camera&action=edit&redlink=1 "Type:Camera (page does not exist)"))

The camera used to render the texture.

### Resolution ( [int2](https://wiki.resonite.com/Type:Int2 "Type:Int2"))

The resolution for the texture.

### Format ( [string](https://wiki.resonite.com/Type:String "Type:String"))

The texture asset file format (defaults to `webp`).

### Quality ( [int](https://wiki.resonite.com/Type:Int "Type:Int"))

The quality of the texture asset (default to `200`).

## Outputs

### OnRenderStarted ( [AsyncCall](https://wiki.resonite.com/Impulses "Impulses"))

Fires when this rendering task has started.

### OnRendered ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when this rendering task has finished rendering.

### OnFailed ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires when this rendering task has failed.

### RenderedAssetURL ( [Uri](https://wiki.resonite.com/Type:Uri "Type:Uri"))

The Uri asset of the texture.

Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:RenderToTextureAsset&oldid=110593](https://wiki.resonite.com/index.php?title=ProtoFlux:RenderToTextureAsset&oldid=110593)"

Contents