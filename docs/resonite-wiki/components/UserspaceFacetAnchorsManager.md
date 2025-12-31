# Component:UserspaceFacetAnchorsManager

> Source: https://wiki.resonite.com/Component:UserspaceFacetAnchorsManager

![](https://wiki.resonite.com/images/f/fe/WarningIcon.svg)

This is a **[userspace](https://wiki.resonite.com/Userspace "Userspace") component** — you cannot attach it anywhere but the userspace. Messing with the userspace can be fun, but it is **not recommended** as you risk messing your dash up if you don't know what you're doing.


Collapse **Component image**

[File:UserspaceFacetAnchorsManagerComponent.png](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=UserspaceFacetAnchorsManagerComponent.png "File:UserspaceFacetAnchorsManagerComponent.png") **Userspace Facet Anchors Manager** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

To know what this controls, see [Facet Anchors](https://wiki.resonite.com/Facets#Facet_Anchors "Facets").

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `Open` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether the facet anchors are open or closed. |
| `UseFacetAnchors` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Whether to allow the use of facet anchors. |
| `Toggle` | **[Chirality](https://wiki.resonite.com/Type:Chirality "Type:Chirality")** | What controller toggles facet anchors when opening dash. |
| `AnimSpeed` | **[Float](https://wiki.resonite.com/Type:Float "Type:Float")** | How fast the facet anchors should open or close. |
| `Dash` | **[UserspaceRadiantDash](https://wiki.resonite.com/Component:UserspaceRadiantDash "Component:UserspaceRadiantDash")** | The dash that is in the world this component is managing facet anchors for. |
| `ProfileName` | **[String](https://wiki.resonite.com/Type:String "Type:String")** | The name of the profile to use when loading the facet anchors. |
| `Anchors` | _[list](https://wiki.resonite.com/Type:SyncList%601 "Type:SyncList`1")_ of **[UserspaceFacetAnchorsManager.Data](https://wiki.resonite.com/Component:UserspaceFacetAnchorsManager#Data)** | A list of facet anchors and their data. |

Fields
Collapse

## Data

| Name | Type | Description |
| --- | --- | --- |
| `Point` | **[FacetAnchorPoint](https://wiki.resonite.com/Type:FacetAnchorPoint "Type:FacetAnchorPoint")** | Where this facet should be. |
| `Root` | **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | The root of this facet anchor element. |
| `Workspace` | **[Workspace](https://wiki.resonite.com/Component:Workspace "Component:Workspace")** | The workspace component that controls saving and loading of this facet's data. |

Fields

## Usage

## Examples

## See Also

- [Facet Anchors](https://wiki.resonite.com/Facets#Facet_Anchors "Facets")

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:UserspaceFacetAnchorsManager&oldid=106612](https://wiki.resonite.com/index.php?title=Component:UserspaceFacetAnchorsManager&oldid=106612)"

Contents