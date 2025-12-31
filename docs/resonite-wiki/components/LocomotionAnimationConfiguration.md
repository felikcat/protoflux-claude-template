# Component:LocomotionAnimationConfiguration

> Source: https://wiki.resonite.com/Component:LocomotionAnimationConfiguration

Collapse **Component image**

[File:LocomotionAnimationConfigurationComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=LocomotionAnimationConfigurationComponent.png "File:LocomotionAnimationConfigurationComponent.png") **Locomotion Animation Configuration** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The **LocomotionAnimationConfiguration** component is used to customize the user's locomotion animations using a list of gaits and a global settings menu as well.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `GlobalParameters` | _direct_ **[LocomotionAnimationGlobalParameters](https://wiki.resonite.com/Type:LocomotionAnimationGlobalParameters "Type:LocomotionAnimationGlobalParameters")** | The settings to use for all gaits regardless of user speed. |
| `Gaits` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[LocomotionAnimationGaitParameters](https://wiki.resonite.com/Type:LocomotionAnimationGaitParameters "Type:LocomotionAnimationGaitParameters")** | The list of gaits to use at different speeds of user movement. |

Fields
Collapse

## Usage

Can be used to customize the user's procedural animations when walking.

## Examples

### Videos

[Frooxius](https://wiki.resonite.com/User:Frooxius "User:Frooxius") goes over how the **LocomotionAnimationConfiguration** component can be customized (featuring [Cyro](https://wiki.resonite.com/index.php?title=User:Cyro&action=edit&redlink=1 "User:Cyro (page does not exist)")).

![](https://i.ytimg.com/vi/wHeBGDoK0BA/hqdefault.jpg)

[Locomotion animation system crash course](https://www.youtube-nocookie.com/embed/wHeBGDoK0BA?autoplay=1)

Load video

YouTube

YouTube might collect personal data. [Privacy Policy](https://www.youtube.com/howyoutubeworks/user-settings/privacy/)

ContinueDismiss

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:LocomotionAnimationConfiguration&oldid=96684](https://wiki.resonite.com/index.php?title=Component:LocomotionAnimationConfiguration&oldid=96684)"

Contents