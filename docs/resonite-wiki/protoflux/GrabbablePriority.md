# ProtoFlux:GrabbablePriority

> Source: https://wiki.resonite.com/ProtoFlux:GrabbablePriority

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
  * [English](https://wiki.resonite.com/ProtoFlux:GrabbablePriority)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AGrabbablePriority "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AGrabbablePriority "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:GrabbablePriority
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:GrabbablePriority#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:GrabbablePriority)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GrabbablePriority&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GrabbablePriority&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:GrabbablePriority "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:GrabbablePriority&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:GrabbablePriority "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:GrabbablePriority "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GrabbablePriority&oldid=109947 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GrabbablePriority&action=info "More information about this page")


Grabbable Priority
Grabbable
*
Grabbable
Grabbable Priority is a ProtoFlux node that gets the priority of an [IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable"). 
Grab Priority Determines what gets grabbed if several grabbable objects are touching someone's grab sphere. The [IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable") with the highest priority will be grabbed first. If the highest priority ties with another [IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable"), it will grab both of those and ignore any lower priority [IGrabbables](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable"). 
## Inputs
### Grabbable ([IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable"))
The grabbable that should be checked for a grabber that is grabbing it. 
## Outputs
### * ([Grabber](https://wiki.resonite.com/Type:Grabber "Type:Grabber"))
The grab priority of the provided Grabbable ([IGrabbable](https://wiki.resonite.com/Type:IGrabbable "Type:IGrabbable")). 
## Examples
  * [An example of using Grabbable Priority to get the grab priority of a DynamicBoneChain component.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Grabbable_Priority.webp "File:Protoflux example Grabbable Priority.webp")
An example of using Grabbable Priority to get the grab priority of a [DynamicBoneChain component](https://wiki.resonite.com/Component:DynamicBoneChain "Component:DynamicBoneChain").


Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:GrabbablePriority&oldid=109947](https://wiki.resonite.com/index.php?title=ProtoFlux:GrabbablePriority&oldid=109947)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:GrabbablePriority#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:GrabbablePriority#Inputs)
    * [ 1.1 Grabbable (IGrabbable) ](https://wiki.resonite.com/ProtoFlux:GrabbablePriority#Grabbable_\(IGrabbable\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:GrabbablePriority#Outputs)
    * [ 2.1 * (Grabber) ](https://wiki.resonite.com/ProtoFlux:GrabbablePriority#*_\(Grabber\))
  * [ 3 Examples ](https://wiki.resonite.com/ProtoFlux:GrabbablePriority#Examples)


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [Pages with broken file links](https://wiki.resonite.com/Category:Pages_with_broken_file_links "Category:Pages with broken file links")
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Interaction:Grabbable](https://wiki.resonite.com/Category:ProtoFlux:Interaction:Grabbable "Category:ProtoFlux:Interaction:Grabbable")
  * [ContinuouslyChanging nodes](https://wiki.resonite.com/Category:ContinuouslyChanging_nodes "Category:ContinuouslyChanging nodes")


Last modified
This page was last edited on 21 August 2025, at 00:21.
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


