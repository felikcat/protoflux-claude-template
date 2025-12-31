# ProtoFlux:LocalImpulseTimeout

> Source: https://wiki.resonite.com/ProtoFlux:LocalImpulseTimeout

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
  * [English](https://wiki.resonite.com/ProtoFlux:LocalImpulseTimeout)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3ALocalImpulseTimeout "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3ALocalImpulseTimeout "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:LocalImpulseTimeout
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:LocalImpulseTimeout#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:LocalImpulseTimeout)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:LocalImpulseTimeout&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:LocalImpulseTimeout&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:LocalImpulseTimeout "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:LocalImpulseTimeout&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:LocalImpulseTimeout "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:LocalImpulseTimeout "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:LocalImpulseTimeout&oldid=110223 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:LocalImpulseTimeout&action=info "More information about this page")


Local Impulse Timeout
Trigger
Next
Reset
Timeout
Flow
Local Impulse Timeout is a ProtoFlux node that when recieving impulses from a specific user in the Trigger ([Call](https://wiki.resonite.com/Impulses "Impulses")) Slot, it will send an impulse out of Next ([Continuation](https://wiki.resonite.com/Impulses "Impulses")). Afterwards, that user will not be able to send more impulses through the node until either Reset ([Call](https://wiki.resonite.com/Impulses "Impulses")) is called or Timeout (Pseudo-generic) time has passed. 
This is extremely useful to prevent button spam abuse. 
## Inputs
### Trigger ([Call](https://wiki.resonite.com/Impulses "Impulses"))
Trigger the node to attempt to send an impulse out of Next ([Continuation](https://wiki.resonite.com/Impulses "Impulses")). 
### Reset ([Call](https://wiki.resonite.com/Impulses "Impulses"))
Reset the Timeout (Pseudo-generic) so more impulses from the local user can go out to Next again. 
### Timeout (Pseudo-generic)
How long to prevent the local user from sending impulses through after the first in seconds as a [float](https://wiki.resonite.com/Type:Float "Type:Float") or as a [TimeSpan](https://wiki.resonite.com/Type:TimeSpan "Type:TimeSpan")
Examples (all): [float](https://wiki.resonite.com/Type:Float "Type:Float"), [TimeSpan](https://wiki.resonite.com/Type:TimeSpan "Type:TimeSpan")
## Outputs
### Next ([Continuation](https://wiki.resonite.com/Impulses "Impulses"))
Will send an impulse immediately after Trigger ([Call](https://wiki.resonite.com/Impulses "Impulses")) has been impulsed and Timeout (Pseudo-generic) time has passed since the last impulse from the local user. 
## Examples
  * [Local Impulse Timeout being used to stop someone from spamming a door.](https://wiki.resonite.com/index.php?title=Special:Upload&wpDestFile=Protoflux_example_Local_Impulse_Timeout_door.webp "File:Protoflux example Local Impulse Timeout door.webp")
Local Impulse Timeout being used to stop someone from spamming a door.
  * [![Local Impulse Timeout being used to stop someone from spamming a booper on someone's face.](https://wiki.resonite.com/images/thumb/f/fc/Protoflux_example_Local_Impulse_Timeout_booper.webp/480px-Protoflux_example_Local_Impulse_Timeout_booper.webp.png)](https://wiki.resonite.com/File:Protoflux_example_Local_Impulse_Timeout_booper.webp "Local Impulse Timeout being used to stop someone from spamming a booper on someone's face.")
Local Impulse Timeout being used to stop someone from spamming a booper on someone's face.


Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:LocalImpulseTimeout&oldid=110223](https://wiki.resonite.com/index.php?title=ProtoFlux:LocalImpulseTimeout&oldid=110223)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:LocalImpulseTimeout#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:LocalImpulseTimeout#Inputs)
    * [ 1.1 Trigger (Call) ](https://wiki.resonite.com/ProtoFlux:LocalImpulseTimeout#Trigger_\(Call\))
    * [ 1.2 Reset (Call) ](https://wiki.resonite.com/ProtoFlux:LocalImpulseTimeout#Reset_\(Call\))
    * [ 1.3 Timeout (Pseudo-generic) ](https://wiki.resonite.com/ProtoFlux:LocalImpulseTimeout#Timeout_\(Pseudo-generic\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:LocalImpulseTimeout#Outputs)
    * [ 2.1 Next (Continuation) ](https://wiki.resonite.com/ProtoFlux:LocalImpulseTimeout#Next_\(Continuation\))
  * [ 3 Examples ](https://wiki.resonite.com/ProtoFlux:LocalImpulseTimeout#Examples)


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [Pages with broken file links](https://wiki.resonite.com/Category:Pages_with_broken_file_links "Category:Pages with broken file links")
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Flow](https://wiki.resonite.com/Category:ProtoFlux:Flow "Category:ProtoFlux:Flow")


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


