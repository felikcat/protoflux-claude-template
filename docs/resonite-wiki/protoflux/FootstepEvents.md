# ProtoFlux:FootstepEvents

> Source: https://wiki.resonite.com/ProtoFlux:FootstepEvents

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
  * [English](https://wiki.resonite.com/ProtoFlux:FootstepEvents)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AFootstepEvents "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AFootstepEvents "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:FootstepEvents
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:FootstepEvents#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:FootstepEvents)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FootstepEvents&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FootstepEvents&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:FootstepEvents "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:FootstepEvents&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:FootstepEvents "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:FootstepEvents "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FootstepEvents&oldid=109811 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FootstepEvents&action=info "More information about this page")


Footstep Events
Footstep
Side
Position
Rotation
ImpactVelocity
HasLanded
HitCollider
HitTriangleIndex
Source
null
∅
Locomotion
The **Footstep Events** node takes in the global source of a [FootstepEventRelay](https://wiki.resonite.com/Component:FootstepEventRelay "Component:FootstepEventRelay") or [SelfFootstepEventRelay](https://wiki.resonite.com/Component:SelfFootstepEventRelay "Component:SelfFootstepEventRelay") component, and returns the values from this [user's](https://wiki.resonite.com/User "User") footstep. The footstep event counts when any proxy on a [slot](https://wiki.resonite.com/Slot "Slot") detects the collision and raycast from a user's feet onto that [ICollider](https://wiki.resonite.com/Type:ICollider "Type:ICollider"), as long as that collider does **not** have the `No Collision` setting on, and also does **not** have the `Ignore Raycasts` setting on. 
## Outputs
### Footstep ([Call](https://wiki.resonite.com/Impulses "Impulses"))
Fires when a footstep event happens from a [FootstepEventRelay](https://wiki.resonite.com/Component:FootstepEventRelay "Component:FootstepEventRelay") or [SelfFootstepEventRelay](https://wiki.resonite.com/Component:SelfFootstepEventRelay "Component:SelfFootstepEventRelay") component. 
### Side ([Chirality](https://wiki.resonite.com/Type:Chirality "Type:Chirality"))
Returns the side of that footstep. 
### Position ([float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))
Returns the position of that footstep. 
### Rotation ([floatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ"))
Returns the rotation of that footstep. 
### ImpactVelocity ([float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))
Returns the impact velocity of that footstep. 
### HasLanded ([bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))
Returns if this footstep has landed. 
### HitCollider ([ICollider](https://wiki.resonite.com/Type:ICollider "Type:ICollider"))
Returns the collider that this footstep has collided with. 
### HitTriangleIndex ([int](https://wiki.resonite.com/Type:Int "Type:Int"))
Returns the particular triangle of where this footstep has collided with. 
## Globals
### Source ([IFootstepEventRelay](https://wiki.resonite.com/index.php?title=Type:IFootstepEventRelay&action=edit&redlink=1 "Type:IFootstepEventRelay \(page does not exist\)"))
The [FootstepEventRelay](https://wiki.resonite.com/Component:FootstepEventRelay "Component:FootstepEventRelay") or [SelfFootstepEventRelay](https://wiki.resonite.com/Component:SelfFootstepEventRelay "Component:SelfFootstepEventRelay") component required to make this node work. 
Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:FootstepEvents&oldid=109811](https://wiki.resonite.com/index.php?title=ProtoFlux:FootstepEvents&oldid=109811)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:FootstepEvents#top "Back to top \[home\]")
Contents
  * [ 1 Outputs ](https://wiki.resonite.com/ProtoFlux:FootstepEvents#Outputs)
    * [ 1.1 Footstep (Call) ](https://wiki.resonite.com/ProtoFlux:FootstepEvents#Footstep_\(Call\))
    * [ 1.2 Side (Chirality) ](https://wiki.resonite.com/ProtoFlux:FootstepEvents#Side_\(Chirality\))
    * [ 1.3 Position (float3) ](https://wiki.resonite.com/ProtoFlux:FootstepEvents#Position_\(float3\))
    * [ 1.4 Rotation (floatQ) ](https://wiki.resonite.com/ProtoFlux:FootstepEvents#Rotation_\(floatQ\))
    * [ 1.5 ImpactVelocity (float3) ](https://wiki.resonite.com/ProtoFlux:FootstepEvents#ImpactVelocity_\(float3\))
    * [ 1.6 HasLanded (bool) ](https://wiki.resonite.com/ProtoFlux:FootstepEvents#HasLanded_\(bool\))
    * [ 1.7 HitCollider (ICollider) ](https://wiki.resonite.com/ProtoFlux:FootstepEvents#HitCollider_\(ICollider\))
    * [ 1.8 HitTriangleIndex (int) ](https://wiki.resonite.com/ProtoFlux:FootstepEvents#HitTriangleIndex_\(int\))
  * [ 2 Globals ](https://wiki.resonite.com/ProtoFlux:FootstepEvents#Globals)
    * [ 2.1 Source (IFootstepEventRelay) ](https://wiki.resonite.com/ProtoFlux:FootstepEvents#Source_\(IFootstepEventRelay\))


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Locomotion](https://wiki.resonite.com/Category:ProtoFlux:Locomotion "Category:ProtoFlux:Locomotion")


Last modified
This page was last edited on 21 August 2025, at 00:16.
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


