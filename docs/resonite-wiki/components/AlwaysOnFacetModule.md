# Component:AlwaysOnFacetModule

> Source: https://wiki.resonite.com/Component:AlwaysOnFacetModule

Collapse **Component image**

[![](https://wiki.resonite.com/images/thumb/d/d7/AlwaysOnFacetModule.png/510px-AlwaysOnFacetModule.png)](https://wiki.resonite.com/File:AlwaysOnFacetModule.png) **Always On Facet Module** component as seen in the [Scene Inspector](https://wiki.resonite.com/Scene_Inspector "Scene Inspector")

The AlwaysOnFacetModule component allows apart of a [facet](https://wiki.resonite.com/Facets "Facets") to remain active while the [dashboard](https://wiki.resonite.com/Dash_Menu "Dash Menu") is closed.

## Fields

| Name | Type | Description |
| --- | --- | --- |
| `persistent` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Determines whether or not this item will be saved to the server. |
| `UpdateOrder` | **[Int](https://wiki.resonite.com/Type:Int "Type:Int")** | Controls the order in which this component is updated. |
| `Enabled` | **[Bool](https://wiki.resonite.com/Type:Bool "Type:Bool")** | Controls whether or not this component is enabled. Some components stop their functionality when this field is disabled, but some don't. |
| `_targets` | _[list](https://wiki.resonite.com/Type:SyncRefList%601 "Type:SyncRefList`1")_ of **[Slot](https://wiki.resonite.com/Type:Slot "Type:Slot")** | A list of Slots that should remain active when the dash is closed. |

Fields
Collapse

## Behavior

This component only applies to [Facets](https://wiki.resonite.com/Facets "Facets").

When a [Facets](https://wiki.resonite.com/Facets "Facets") is installed in a [dashboard](https://wiki.resonite.com/Dash_Menu "Dash Menu"), all of the children of a slot containing a AlwaysOnFacetModule are reparented to a [Slot](https://wiki.resonite.com/Slot "Slot") outside of the dashboard. This slot is active when the [dashboard](https://wiki.resonite.com/Dash_Menu "Dash Menu") is closed, otherwise the facet is inactive due to being under an inactive [Slot](https://wiki.resonite.com/Slot "Slot").

Do not manually modify the \_targets list, as it is managed during the normal lifetime of the component. Manually modifying the list may cause unexpected behavior.

This will change the hierarchy of the [Facets](https://wiki.resonite.com/Facets "Facets"), if you rely on your facet using [dynamic variables](https://wiki.resonite.com/Dynamic_Variables "Dynamic Variables") they may disconnect due to reparenting (many parts of facets are re-parented, be warned).

Avoid putting this above the [UIX elements](https://wiki.resonite.com/UIX "UIX") of the [Facets](https://wiki.resonite.com/Facets "Facets"), as it will reparent them and they will no longer show up or may break the canvas.

## Examples

For creating a taco facet that reports live taco statistics from a [WebSockets](https://wiki.resonite.com/WebSocket "WebSocket"), and plays an audio clip when a new taco deal is available.
In this example the [WebSockets](https://wiki.resonite.com/WebSocket "WebSocket") and audio output are active sensitive, and will not work when the dashboard is closed without an AlwaysOnFacetModule.

```
 Taco Facet
   Canvas - (Having the same name helps when debugging)
     Background and Taco pictures
   Logic - (with AlwaysOnFacetModule)
     Taco Facet Logic - (Having the same name helps when debugging)
       ProtoFlux, WebSockets, audio, and other active sensitive content
```

When installed, the facet is pulled apart into the following, the exact hierarchy is prone to change but this is the general structure.

```
 Dashboard Root
   AlwaysOnFacetRoot
     Taco Facet Logic
   DashOffset
     ...Many other slots, some of which go inactive when the dashboard is closed...
       Facets
         Taco Facet
           Canvas
             Background and Taco pictures
```

## See Also

Retrieved from " [https://wiki.resonite.com/index.php?title=Component:AlwaysOnFacetModule&oldid=96216](https://wiki.resonite.com/index.php?title=Component:AlwaysOnFacetModule&oldid=96216)"

Contents