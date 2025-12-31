# ProtoFlux:FingerPose

> Source: https://wiki.resonite.com/ProtoFlux:FingerPose

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
  * [English](https://wiki.resonite.com/ProtoFlux:FingerPose)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AFingerPose "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AFingerPose "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:FingerPose
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:FingerPose#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:FingerPose)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FingerPose&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FingerPose&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:FingerPose "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:FingerPose&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:FingerPose "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:FingerPose "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FingerPose&oldid=109785 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FingerPose&action=info "More information about this page")


Finger Pose
PoseSource
Position
FingerNode
Rotation
Avatars
Finger Pose is a ProtoFlux node that takes a Pose source and a body node corresponding to a finger on a user's avatar and returns it's rotation and position. 
## Inputs
### PoseSource ([IFingerPoseSource](https://wiki.resonite.com/Type:IFingerPoseSource "Type:IFingerPoseSource"))
A pose source usually obtained using a [User Finger Pose Source](https://wiki.resonite.com/ProtoFlux:User_Finger_Pose_Source "ProtoFlux:User Finger Pose Source") Node. 
### FingerNode ([BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode"))
A finger node as a body node, providing a non finger body node will make the output a default 0. 
## Outputs
### Position ([Float3](https://wiki.resonite.com/Type:Float3 "Type:Float3"))
The position of the finger node if PoseSource ([IFingerPoseSource](https://wiki.resonite.com/Type:IFingerPoseSource "Type:IFingerPoseSource")) is not null and FingerNode ([BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode")) is a body node that points to a finger. 
### Rotation ([FloatQ](https://wiki.resonite.com/Type:FloatQ "Type:FloatQ"))
The rotation of the finger if PoseSource ([IFingerPoseSource](https://wiki.resonite.com/Type:IFingerPoseSource "Type:IFingerPoseSource")) is not null and FingerNode ([BodyNode](https://wiki.resonite.com/Type:BodyNode "Type:BodyNode")) is a body node that points to a finger. 
## Examples
  * [An example of finger pose being used with a Index Controller or camera tracking to be used for finger gestures for making magic spells/actions.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Finger_Pose.webp "File:Protoflux example Finger Pose.webp")
An example of finger pose being used with a Index Controller or camera tracking to be used for finger gestures for making magic spells/actions.


Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:FingerPose&oldid=109785](https://wiki.resonite.com/index.php?title=ProtoFlux:FingerPose&oldid=109785)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:FingerPose#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:FingerPose#Inputs)
    * [ 1.1 PoseSource (IFingerPoseSource) ](https://wiki.resonite.com/ProtoFlux:FingerPose#PoseSource_\(IFingerPoseSource\))
    * [ 1.2 FingerNode (BodyNode) ](https://wiki.resonite.com/ProtoFlux:FingerPose#FingerNode_\(BodyNode\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:FingerPose#Outputs)
    * [ 2.1 Position (Float3) ](https://wiki.resonite.com/ProtoFlux:FingerPose#Position_\(Float3\))
    * [ 2.2 Rotation (FloatQ) ](https://wiki.resonite.com/ProtoFlux:FingerPose#Rotation_\(FloatQ\))
  * [ 3 Examples ](https://wiki.resonite.com/ProtoFlux:FingerPose#Examples)


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [Pages with broken file links](https://wiki.resonite.com/Category:Pages_with_broken_file_links "Category:Pages with broken file links")
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Avatars](https://wiki.resonite.com/Category:ProtoFlux:Avatars "Category:ProtoFlux:Avatars")
  * [ContinuouslyChanging nodes](https://wiki.resonite.com/Category:ContinuouslyChanging_nodes "Category:ContinuouslyChanging nodes")


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


