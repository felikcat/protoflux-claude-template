# Component:RenderTransformOverride

> Source: https://wiki.resonite.com/Component:RenderTransformOverride

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/c/c3/RenderTransformOverrideComponent.png/510px-RenderTransformOverrideComponent.png)](https://wiki.resonite.com/File:RenderTransformOverrideComponent.png) **Render Material Override** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The RenderTransformOverride component is used to transform, rotate or scale a [Slot](https://wiki.resonite.com/Slot "Slot") following a specific [rendering context](https://wiki.resonite.com/Type:RenderingContext "Type:RenderingContext").

It can be used, for instance, to scale a player's head to zero locally to effectively hide it from the user's view while it still being visible in mirrors, cameras and by other players.

This component is automatically added to all [Avatars](https://wiki.resonite.com/Avatar "Avatar") on the Head [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode") by the [AvatarUserViewHeadOverride](https://wiki.resonite.com/Component:AvatarUserViewHeadOverride "Component:AvatarUserViewHeadOverride") component. It will also setup drives for Enabled, PositionOverride, and RotationOverride.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Context` | **[RenderingContext](https://wiki.resonite.com/Type:RenderingContext "Type:RenderingContext")** | The Context when rendering from to apply this override. |
| `PositionOverride` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | If not null, will override the position of the slot this component is on. |
| `RotationOverride` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ") >** | If not null, will override the rotation of the slot this component is on. |
| `ScaleOverride` | **[Nullable\`1](https://wiki.resonite.com/Type:Nullable%601 "Type:Nullable`1") < [Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3") >** | If not null, will override the scale of the slot this component is on. |
| `SkinnedMeshRenderers` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[SkinnedMeshRenderer](https://wiki.resonite.com/Component:SkinnedMeshRenderer "Component:SkinnedMeshRenderer")** | List of SkinnedMeshRenderers that need to be recalculated and overridden. |

Fields
Collapse

## Examples

[![](https://wiki.resonite.com/images/thumb/5/5b/ModifiedRTO.png/400px-ModifiedRTO.png)](https://wiki.resonite.com/File:ModifiedRTO.png) A modified default

A RenderTransformOverride is automatically added to avatars and is located on the head bodynode slot. You can expand what gets automatically included to also hide the head from your viewpoint by enabling the Scale option with the values all set to 0. Do note that this will affect the shadow of your avatar from your own viewpoint while in first person.

## Bugs

- This component has a very small chance to increase the frequency of crashes.[\[1\]](https://wiki.resonite.com/Component:RenderTransformOverride#cite_note-1)
- This component might not function correctly if there are any Null fields in the SkinnedMeshRenderers list.[\[2\]](https://wiki.resonite.com/Component:RenderTransformOverride#cite_note-2)
- This component currently has an imprecise understanding of the UserView context and will be active while an item is grabbed or when saving a thumbnail to the inventory.[\[3\]](https://wiki.resonite.com/Component:RenderTransformOverride#cite_note-3)
- This component will cause motion blur to be very visible on object when looking through a cameras or in a mirror.[\[4\]](https://wiki.resonite.com/Component:RenderTransformOverride#cite_note-4)

## Notes

1. [↑](https://wiki.resonite.com/Component:RenderTransformOverride#cite_ref-1 "Jump up")[https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/269](https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/269)
2. [↑](https://wiki.resonite.com/Component:RenderTransformOverride#cite_ref-2 "Jump up")[https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/2474](https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/2474)
3. [↑](https://wiki.resonite.com/Component:RenderTransformOverride#cite_ref-3 "Jump up")[https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/3732](https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/3732)
4. [↑](https://wiki.resonite.com/Component:RenderTransformOverride#cite_ref-4 "Jump up")[https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/1654](https://github.com/Yellow-Dog-Man/Resonite-Issues/issues/1654)

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:RenderTransformOverride&oldid=97708](https://wiki.resonite.com/index.php?title=Component:RenderTransformOverride&oldid=97708)"

Contents