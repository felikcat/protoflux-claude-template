# ProtoFlux:AttachAudioClip

> Source: https://wiki.resonite.com/ProtoFlux:AttachAudioClip

Attach Audio Clip

\*

Next

URL

AttachedProvider

Target

GetExisting

Characters

Attach Audio Clip is a ProtoFlux node that allows you to attach a provided [uri](https://wiki.resonite.com/Type:Uri "Type:Uri") as a new [StaticAudioClip](https://wiki.resonite.com/Component:StaticAudioClip "Component:StaticAudioClip") component and return the StaticAudioClip raw [IAsset\`1](https://wiki.resonite.com/Type:IAsset%601 "Type:IAsset`1") itself.

## Inputs

### \\* ( [Call](https://wiki.resonite.com/Impulses "Impulses"))

Call to attach the asset.

### URL ( [uri](https://wiki.resonite.com/Type:Uri "Type:Uri"))

The URI of the asset you want to attach. Can be a resdb or a local or a website hosted asset.

### Target ( [Slot](https://wiki.resonite.com/Slot "Slot"))

The slot to attach the asset to.

### GetExisting ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))

Get an existing asset on Target ( [Slot](https://wiki.resonite.com/Slot "Slot")) of the same URL ( [uri](https://wiki.resonite.com/Type:Uri "Type:Uri")) or attach a new one.

## Outputs

### Next ( [Continuation](https://wiki.resonite.com/Impulses "Impulses"))

Fires after \* ( [Call](https://wiki.resonite.com/Impulses "Impulses")) is called and the asset was successfully attached.

### AttachedProvider ( [IAsset\`1](https://wiki.resonite.com/Type:IAsset%601 "Type:IAsset`1") <Audio>)

The attached provider or an existing one on Target ( [Slot](https://wiki.resonite.com/Slot "Slot")) if GetExisting ( [bool](https://wiki.resonite.com/Type:Bool "Type:Bool")) is true.

## Examples

- [An example of Attach Audio Clip being used to keep an asset on an item that someone made in session.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Attach_Audio_Clip.webp "File:Protoflux example Attach Audio Clip.webp")

An example of Attach Audio Clip being used to keep an asset on an item that someone made in session.


Retrieved from " [https://wiki.resonite.com/index.php?title=ProtoFlux:AttachAudioClip&oldid=109297](https://wiki.resonite.com/index.php?title=ProtoFlux:AttachAudioClip&oldid=109297)"

Contents