# ProtoFlux:LineCircleIntersections

> Source: https://wiki.resonite.com/ProtoFlux:LineCircleIntersections

[ ![](https://wiki.resonite.com/images/1/11/Resonite_Wiki-Icon.png) ](https://wiki.resonite.com/Main_Page "Visit the main page")
Toggle search
Search [ ](https://wiki.resonite.com/Special:Random "Random page")
Toggle menu
[ ![](https://wiki.resonite.com/images/1/11/Resonite_Wiki-Icon.png) ](https://wiki.resonite.com/Main_Page "Visit the main page")
Resonite Wiki
Navigation 
  * [](https://wiki.resonite.com/Special:MyLanguage/Main_Page "Visit the main page \[z\]")
  * [](https://wiki.resonite.com/Special:RecentChanges "A list of recent changes in the wiki \[r\]")
  * [](https://wiki.resonite.com/Special:Random "Load a random page \[x\]")
  * [](https://www.mediawiki.org/wiki/Special:MyLanguage/Help:Contents)
  * [Contributing to the Wiki](https://wiki.resonite.com/Special:MyLanguage/Wiki_Contributions_%26_Translations)
  * [](https://wiki.resonite.com/Special:SpecialPages "A list of all special pages \[q\]")
  * [](https://wiki.resonite.com/Special:Upload "Upload files \[u\]")


Team 
  * [Resonite Team](https://wiki.resonite.com/Special:MyLanguage/Resonite_Team)
  * [Moderation](https://wiki.resonite.com/Special:MyLanguage/Moderation)
  * [Office Hours](https://wiki.resonite.com/Special:MyLanguage/Office_Hours)
  * [Contact Us](https://wiki.resonite.com/Special:MyLanguage/Contact_Us)


Key Information 
  * [Guidelines and Rules](https://wiki.resonite.com/Special:MyLanguage/Guidelines)
  * [FAQ](https://wiki.resonite.com/Special:MyLanguage/Frequently_Asked_Questions)
  * [How to Help](https://wiki.resonite.com/Special:MyLanguage/How_to_Help)
  * [Branding Information](https://wiki.resonite.com/Special:MyLanguage/Branding)
  * [Roadmap](https://wiki.resonite.com/Special:MyLanguage/Roadmap)
  * [Get your Patreon Rewards](https://wiki.resonite.com/Special:MyLanguage/Patreon_Linking)


notifications 
Toggle personal menu
  * Not logged in


user-interface-preferences 
  * [English](https://wiki.resonite.com/ProtoFlux:LineCircleIntersections)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3ALineCircleIntersections "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3ALineCircleIntersections "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:LineCircleIntersections
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:LineCircleIntersections#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:LineCircleIntersections)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:LineCircleIntersections&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:LineCircleIntersections&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:LineCircleIntersections "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:LineCircleIntersections&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:LineCircleIntersections "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:LineCircleIntersections "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:LineCircleIntersections&oldid=110217 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:LineCircleIntersections&action=info "More information about this page")


Line Circle Intersections
Center
IntersectionCount
Radius
Intersection0
LinePoint0
Intersection1
LinePoint1
Geometry 2D
The **Line Circle Intersections** node determines how many times a line defined by two points intersects a circle and where said intersections occur. 
## Inputs
### Center ([float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))
Center of the circle. 
### Radius ([float](https://wiki.resonite.com/Type:Float "Type:Float"))
Radius of the circle. 
### LinePoint0 ([float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))
First point of the line. 
### LinePoint1 ([float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))
Second point of the line. 
## Outputs
### IntersectionCount ([int](https://wiki.resonite.com/Type:Int "Type:Int"))
The amount of intersections of the defined line and circle. This is at most two. 
### Intersection0 ([float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))
The first point of intersection between the line and circle. This is the point that occurs "later" in the intersection when tracing the line from `LinePoint0` to `LinePoint1`. If there does not exist any intersection, this value is `[NaN; NaN]`. 
### Intersection1 ([float2](https://wiki.resonite.com/Type:Float2 "Type:Float2"))
The second point of intersection between the line and circle. This is the point that occurs "earlier" in the intersection when tracing the line from `LinePoint0` to `LinePoint1`. If there are fewer than two intersections, this value is `[NaN; NaN]`. 
## Examples
  * [![Center=0,0 Radius=1 LinePoint0=0,2 LinePoint1=0,0; Outputs: IntersectionCount=2 Intersection0=0,1 Intersection1=0,1](https://wiki.resonite.com/images/thumb/6/66/ProtoFlux_Example_Line_Circle_Intersections.webp/400px-ProtoFlux_Example_Line_Circle_Intersections.webp.png)](https://wiki.resonite.com/File:ProtoFlux_Example_Line_Circle_Intersections.webp "An example of the Line Circle Intersections node, where a circle centered at \(0,0\) and radius 1 intersects with a line defined by the points \(0,2\) and \(0,0\) at the points \(0,-1\) and \(0,1\).")
An example of the Line Circle Intersections node, where a circle centered at `(0,0)` and radius `1` intersects with a line defined by the points `(0,2)` and `(0,0)` at the points `(0,-1)` and `(0,1)`.


Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:LineCircleIntersections&oldid=110217](https://wiki.resonite.com/index.php?title=ProtoFlux:LineCircleIntersections&oldid=110217)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:LineCircleIntersections#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:LineCircleIntersections#Inputs)
    * [ 1.1 Center (float2) ](https://wiki.resonite.com/ProtoFlux:LineCircleIntersections#Center_\(float2\))
    * [ 1.2 Radius (float) ](https://wiki.resonite.com/ProtoFlux:LineCircleIntersections#Radius_\(float\))
    * [ 1.3 LinePoint0 (float2) ](https://wiki.resonite.com/ProtoFlux:LineCircleIntersections#LinePoint0_\(float2\))
    * [ 1.4 LinePoint1 (float2) ](https://wiki.resonite.com/ProtoFlux:LineCircleIntersections#LinePoint1_\(float2\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:LineCircleIntersections#Outputs)
    * [ 2.1 IntersectionCount (int) ](https://wiki.resonite.com/ProtoFlux:LineCircleIntersections#IntersectionCount_\(int\))
    * [ 2.2 Intersection0 (float2) ](https://wiki.resonite.com/ProtoFlux:LineCircleIntersections#Intersection0_\(float2\))
    * [ 2.3 Intersection1 (float2) ](https://wiki.resonite.com/ProtoFlux:LineCircleIntersections#Intersection1_\(float2\))
  * [ 3 Examples ](https://wiki.resonite.com/ProtoFlux:LineCircleIntersections#Examples)


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Math:Geometry2D](https://wiki.resonite.com/Category:ProtoFlux:Math:Geometry2D "Category:ProtoFlux:Math:Geometry2D")


Last modified
This page was last edited on 21 August 2025, at 00:26.
Resonite Wiki
[Resonite Website](https://resonite.com)
[Resonite Policies](https://resonite.com/policies)
[Resonite on Steam](https://store.steampowered.com/app/2519830/Resonite/)
  * [Privacy policy](https://wiki.resonite.com/Resonite_Wiki:Privacy_policy)
  * [About Resonite Wiki](https://wiki.resonite.com/Resonite_Wiki:About)
  * [Disclaimers](https://wiki.resonite.com/Resonite_Wiki:General_disclaimer)


Content is available under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/deed.en), unless otherwise specified. 
Resonite is Copyright © Yellow Dog Man Studios s.r.o. 
  * [![Powered by MediaWiki](https://wiki.resonite.com/resources/assets/poweredby_mediawiki_88x31.png)](https://www.mediawiki.org/)


