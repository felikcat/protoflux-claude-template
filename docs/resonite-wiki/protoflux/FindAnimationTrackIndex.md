# ProtoFlux:FindAnimationTrackIndex

> Source: https://wiki.resonite.com/ProtoFlux:FindAnimationTrackIndex

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
  * [English](https://wiki.resonite.com/ProtoFlux:FindAnimationTrackIndex)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AFindAnimationTrackIndex "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AFindAnimationTrackIndex "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:FindAnimationTrackIndex
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:FindAnimationTrackIndex#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:FindAnimationTrackIndex)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FindAnimationTrackIndex&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FindAnimationTrackIndex&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:FindAnimationTrackIndex "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:FindAnimationTrackIndex&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:FindAnimationTrackIndex "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:FindAnimationTrackIndex "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FindAnimationTrackIndex&oldid=109769 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FindAnimationTrackIndex&action=info "More information about this page")


Find Animation Track Index
Animation
*
Node
Property
Assets
  
This node when provided an [Animation Asset](https://wiki.resonite.com/Type:Animation "Type:Animation") will search the animation's [AnimJ](https://wiki.resonite.com/AnimJ "AnimJ") data for a field on an object 
## Inputs
### Animation ([Animation Asset](https://wiki.resonite.com/Type:Animation "Type:Animation"))
The [Animation Asset](https://wiki.resonite.com/Type:Animation "Type:Animation") provided by an [IAssetProvider<Animation>](https://wiki.resonite.com/Type:IAssetProvider%601 "Type:IAssetProvider`1"). 
### Node ([String](https://wiki.resonite.com/Type:String "Type:String"))
A [String](https://wiki.resonite.com/Type:String "Type:String") that is usually the name of the slot which has it's property animated. This can vary though, and [AnimJ](https://wiki.resonite.com/AnimJ "AnimJ") explains this. 
### Property ([String](https://wiki.resonite.com/Type:String "Type:String"))
A [String](https://wiki.resonite.com/Type:String "Type:String") that is usually the human name of a field. So a [floatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ") would be Rotation for a Property. This can vary though, and [AnimJ](https://wiki.resonite.com/AnimJ "AnimJ") explains this. 
## Outputs
### * ([Int](https://wiki.resonite.com/Types:Int "Types:Int"))
The index in a list of drivers a [Animator](https://wiki.resonite.com/Component:Animator "Component:Animator") would have when using the Animation ([Animation Asset](https://wiki.resonite.com/Type:IAsset%601 "Type:IAsset`1")) provided to this node. The animation would be put into the `Clip` Field. 
## Examples
  * [![Example of a find track index being used with a sample track index.](https://wiki.resonite.com/images/thumb/9/93/Animation_Track_Index_Example1.png/480px-Animation_Track_Index_Example1.png)](https://wiki.resonite.com/File:Animation_Track_Index_Example1.png "Example of a find track index being used with a sample track index.")
Example of a find track index being used with a sample track index.


Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:FindAnimationTrackIndex&oldid=109769](https://wiki.resonite.com/index.php?title=ProtoFlux:FindAnimationTrackIndex&oldid=109769)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:FindAnimationTrackIndex#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:FindAnimationTrackIndex#Inputs)
    * [ 1.1 Animation (Animation Asset) ](https://wiki.resonite.com/ProtoFlux:FindAnimationTrackIndex#Animation_\(Animation_Asset\))
    * [ 1.2 Node (String) ](https://wiki.resonite.com/ProtoFlux:FindAnimationTrackIndex#Node_\(String\))
    * [ 1.3 Property (String) ](https://wiki.resonite.com/ProtoFlux:FindAnimationTrackIndex#Property_\(String\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:FindAnimationTrackIndex#Outputs)
    * [ 2.1 * (Int) ](https://wiki.resonite.com/ProtoFlux:FindAnimationTrackIndex#*_\(Int\))
  * [ 3 Examples ](https://wiki.resonite.com/ProtoFlux:FindAnimationTrackIndex#Examples)


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Assets](https://wiki.resonite.com/Category:ProtoFlux:Assets "Category:ProtoFlux:Assets")


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


