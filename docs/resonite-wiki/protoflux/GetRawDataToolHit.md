# ProtoFlux:GetRawDataToolHit

> Source: https://wiki.resonite.com/ProtoFlux:GetRawDataToolHit

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
  * [English](https://wiki.resonite.com/ProtoFlux:GetRawDataToolHit)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AGetRawDataToolHit "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AGetRawDataToolHit "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:GetRawDataToolHit
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:GetRawDataToolHit#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:GetRawDataToolHit)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GetRawDataToolHit&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GetRawDataToolHit&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:GetRawDataToolHit "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:GetRawDataToolHit&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:GetRawDataToolHit "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:GetRawDataToolHit "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GetRawDataToolHit&oldid=109889 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GetRawDataToolHit&action=info "More information about this page")


Get Raw Data Tool Hit
Tool
HitCollider
HitPoint
HitNormal
HitDistance
HitTriangleIndex
Tools
The `Get Raw Data Tool Hit` node creates a raycast from the origin (tip reference slot position and direction?) looking and retrieving for valid hits. This node acts similarly to the [Raycaster](https://wiki.resonite.com/ProtoFlux:Raycaster "ProtoFlux:Raycaster") and [Raycast One](https://wiki.resonite.com/ProtoFlux:Raycast_One "ProtoFlux:Raycast One") nodes in functionality. 
This node returns data per frame, and is very useful for debugging and testing hit detection due to its constant updates. 
This node can be combined with the [Hit UV Coordinate](https://wiki.resonite.com/ProtoFlux:Hit_UV_Coordinate "ProtoFlux:Hit UV Coordinate") node to get further data from this hit, such as a 2D location point on the collider for example. 
## Inputs
### * ([RawDataTool](https://wiki.resonite.com/index.php?title=Type:RawDataTool&action=edit&redlink=1 "Type:RawDataTool \(page does not exist\)"))
The raw data tool to point with using raycasts. 
## Outputs
### HitColider ([ICollider](https://wiki.resonite.com/Type:ICollider "Type:ICollider"))
The collider we hit. 
### HitPoint ([float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))
The point in 3D space of where we hit. 
### HitNormal ([float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))
The normal of the collider facing direction. 
### HitDistance ([float](https://wiki.resonite.com/Type:Float "Type:Float"))
The distance of how far this hit was from the origin of this raycast. 
### HitTriangleIndex ([int](https://wiki.resonite.com/Type:Int "Type:Int"))
The mesh data number of our hit. 
Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:GetRawDataToolHit&oldid=109889](https://wiki.resonite.com/index.php?title=ProtoFlux:GetRawDataToolHit&oldid=109889)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:GetRawDataToolHit#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:GetRawDataToolHit#Inputs)
    * [ 1.1 * (RawDataTool) ](https://wiki.resonite.com/ProtoFlux:GetRawDataToolHit#*_\(RawDataTool\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:GetRawDataToolHit#Outputs)
    * [ 2.1 HitColider (ICollider) ](https://wiki.resonite.com/ProtoFlux:GetRawDataToolHit#HitColider_\(ICollider\))
    * [ 2.2 HitPoint (float3) ](https://wiki.resonite.com/ProtoFlux:GetRawDataToolHit#HitPoint_\(float3\))
    * [ 2.3 HitNormal (float3) ](https://wiki.resonite.com/ProtoFlux:GetRawDataToolHit#HitNormal_\(float3\))
    * [ 2.4 HitDistance (float) ](https://wiki.resonite.com/ProtoFlux:GetRawDataToolHit#HitDistance_\(float\))
    * [ 2.5 HitTriangleIndex (int) ](https://wiki.resonite.com/ProtoFlux:GetRawDataToolHit#HitTriangleIndex_\(int\))


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Tools](https://wiki.resonite.com/Category:ProtoFlux:Tools "Category:ProtoFlux:Tools")
  * [ContinuouslyChanging nodes](https://wiki.resonite.com/Category:ContinuouslyChanging_nodes "Category:ContinuouslyChanging nodes")


Last modified
This page was last edited on 21 August 2025, at 00:20.
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


