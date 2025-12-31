# ProtoFlux:FingerNodeIndex

> Source: https://wiki.resonite.com/ProtoFlux:FingerNodeIndex

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
  * [English](https://wiki.resonite.com/ProtoFlux:FingerNodeIndex)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AFingerNodeIndex "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AFingerNodeIndex "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:FingerNodeIndex
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:FingerNodeIndex#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:FingerNodeIndex)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FingerNodeIndex&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FingerNodeIndex&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:FingerNodeIndex "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:FingerNodeIndex&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:FingerNodeIndex "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:FingerNodeIndex "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FingerNodeIndex&oldid=109783 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FingerNodeIndex&action=info "More information about this page")


Finger Node Index
Node
*
Body Nodes
Finger Node Index is a node that returns the finger index a [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode") has, or -1 if it isn't a body node that is part of a finger. 
## Inputs
### Node ([BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"))
The node to check for a finger node index for 
## Outputs
### * ([int](https://wiki.resonite.com/Type:Int "Type:Int"))
The finger segment index of the given Node ([BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode")) or -1 if Node ([BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode")) is not a finger segment. It will return a value from 0 to 23, counting in the order the finger nodes appear on the [BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode") page for the fingers. 
## Examples
  * [Example of the finger node index being used in some ProtoFlux code.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Finger_Node_Index.webp "File:Protoflux example Finger Node Index.webp")
Example of the finger node index being used in some ProtoFlux code.


Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:FingerNodeIndex&oldid=109783](https://wiki.resonite.com/index.php?title=ProtoFlux:FingerNodeIndex&oldid=109783)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:FingerNodeIndex#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:FingerNodeIndex#Inputs)
    * [ 1.1 Node (BodyNode) ](https://wiki.resonite.com/ProtoFlux:FingerNodeIndex#Node_\(BodyNode\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:FingerNodeIndex#Outputs)
    * [ 2.1 * (int) ](https://wiki.resonite.com/ProtoFlux:FingerNodeIndex#*_\(int\))
  * [ 3 Examples ](https://wiki.resonite.com/ProtoFlux:FingerNodeIndex#Examples)


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [Pages with broken file links](https://wiki.resonite.com/Category:Pages_with_broken_file_links "Category:Pages with broken file links")
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Avatars:BodyNodes](https://wiki.resonite.com/Category:ProtoFlux:Avatars:BodyNodes "Category:ProtoFlux:Avatars:BodyNodes")


Last modified
This page was last edited on 20 August 2025, at 23:52.
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


