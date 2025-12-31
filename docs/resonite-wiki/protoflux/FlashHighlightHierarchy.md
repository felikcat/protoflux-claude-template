# ProtoFlux:FlashHighlightHierarchy

> Source: https://wiki.resonite.com/ProtoFlux:FlashHighlightHierarchy

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
  * [English](https://wiki.resonite.com/ProtoFlux:FlashHighlightHierarchy)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AFlashHighlightHierarchy "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AFlashHighlightHierarchy "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:FlashHighlightHierarchy
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:FlashHighlightHierarchy#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:FlashHighlightHierarchy)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FlashHighlightHierarchy&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FlashHighlightHierarchy&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:FlashHighlightHierarchy "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:FlashHighlightHierarchy&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:FlashHighlightHierarchy "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:FlashHighlightHierarchy "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FlashHighlightHierarchy&oldid=109801 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FlashHighlightHierarchy&action=info "More information about this page")


Flash Highlight Hierarchy
*
Next
HierarchyRoot
FlashRoot
ExcludeColliders
ExcludeMeshes
ExcludeDisabled
TrackPosition
Duration
Color
Rendering
The `Flash Highlight Hierarchy` node takes in the target slot hierarchy, what to exclude, if this flash should track the position, how long the flash should be, and what color it should be. Then this node will make that hierarchy flash, also providing the slot of the flash itself. 
![](https://wiki.resonite.com/images/b/b7/DangerIcon.svg)
It is really easy to lag or even crash a world if this node is abused, try to avoid doing the following: 
  * Setting the color to invisible
  * Having a long duration
  * Calling this node every frame
  * Selecting a heavy slot, like root


This could be disastrous if you are not careful! 
## Inputs
### * ([Call](https://wiki.resonite.com/Impulses "Impulses"))
Calls an impulse to flash the hierarchy. 
### HierarchyRoot ([Slot](https://wiki.resonite.com/Slot "Slot"))
The target hierarchy to flash 
### ExcludeColliders ([bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))
Should exclude any colliders for this flash. 
### ExcludeMeshes ([bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))
Should exclude meshes for this flash. 
### ExcludeDisabled ([bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))
Should exclude any slots that are not active. 
### TrackPosition ([bool](https://wiki.resonite.com/Type:Bool "Type:Bool"))
Should this flash be tracking the provided hierarchy. 
### Duration ([float](https://wiki.resonite.com/Type:Float "Type:Float"))
How long this flash should last for. 
### Color ([colorX](https://wiki.resonite.com/Type:ColorX "Type:ColorX"))
The flash color. 
## Outputs
### Next ([Continuation](https://wiki.resonite.com/Impulses "Impulses"))
Continues the code from here. 
### FlashRoot ([Slot](https://wiki.resonite.com/Slot "Slot"))
The slot that is the flash itself. 
Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:FlashHighlightHierarchy&oldid=109801](https://wiki.resonite.com/index.php?title=ProtoFlux:FlashHighlightHierarchy&oldid=109801)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:FlashHighlightHierarchy#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:FlashHighlightHierarchy#Inputs)
    * [ 1.1 * (Call) ](https://wiki.resonite.com/ProtoFlux:FlashHighlightHierarchy#*_\(Call\))
    * [ 1.2 HierarchyRoot (Slot) ](https://wiki.resonite.com/ProtoFlux:FlashHighlightHierarchy#HierarchyRoot_\(Slot\))
    * [ 1.3 ExcludeColliders (bool) ](https://wiki.resonite.com/ProtoFlux:FlashHighlightHierarchy#ExcludeColliders_\(bool\))
    * [ 1.4 ExcludeMeshes (bool) ](https://wiki.resonite.com/ProtoFlux:FlashHighlightHierarchy#ExcludeMeshes_\(bool\))
    * [ 1.5 ExcludeDisabled (bool) ](https://wiki.resonite.com/ProtoFlux:FlashHighlightHierarchy#ExcludeDisabled_\(bool\))
    * [ 1.6 TrackPosition (bool) ](https://wiki.resonite.com/ProtoFlux:FlashHighlightHierarchy#TrackPosition_\(bool\))
    * [ 1.7 Duration (float) ](https://wiki.resonite.com/ProtoFlux:FlashHighlightHierarchy#Duration_\(float\))
    * [ 1.8 Color (colorX) ](https://wiki.resonite.com/ProtoFlux:FlashHighlightHierarchy#Color_\(colorX\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:FlashHighlightHierarchy#Outputs)
    * [ 2.1 Next (Continuation) ](https://wiki.resonite.com/ProtoFlux:FlashHighlightHierarchy#Next_\(Continuation\))
    * [ 2.2 FlashRoot (Slot) ](https://wiki.resonite.com/ProtoFlux:FlashHighlightHierarchy#FlashRoot_\(Slot\))


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Rendering](https://wiki.resonite.com/Category:ProtoFlux:Rendering "Category:ProtoFlux:Rendering")


Last modified
This page was last edited on 21 August 2025, at 00:15.
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


