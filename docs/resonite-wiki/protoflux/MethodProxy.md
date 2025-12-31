# ProtoFlux:MethodProxy

> Source: https://wiki.resonite.com/ProtoFlux:MethodProxy

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
  * [English](https://wiki.resonite.com/ProtoFlux:MethodProxy)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AMethodProxy "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AMethodProxy "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:MethodProxy
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:MethodProxy#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:MethodProxy)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:MethodProxy&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:MethodProxy&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:MethodProxy "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:MethodProxy&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:MethodProxy "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:MethodProxy "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:MethodProxy&oldid=110269 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:MethodProxy&action=info "More information about this page")


Method Proxy
*
Next
This could be anything
This could be anything
This could be anything
This could be anything
This could be anything
Method
null
∅
CoreNodes
#### What are Method Proxies
The `Method Proxy` node is used to call a method from a component. Some components expose these methods by default such as [StaticTexture2D](https://wiki.resonite.com/Component:StaticTexture2D "Component:StaticTexture2D"). More hidden methods can be exposed when using the mod "[Show Delegates](https://github.com/art0007i/ShowDelegates)" from [Arti](https://wiki.resonite.com/User:Arti "User:Arti"), to do so, go into the inspector of any slot and you should see "---- SYNC METHODS HERE ----", clicking on that should reveal the extra methods. Using your flux tool, grab the method you want, then open your [context menu](https://wiki.resonite.com/Context_menu "Context menu") and select the option "Proxy". This will spawn out a node with any number of arguments depending on the method call you choose. 
The arguments on the Method Proxy node will be depending on the type it wants and also can depend on how many inputs it wants. This makes it very difficult to document the thousands of variants of this node (and is unwise to list them here unless there is a good explanation for the individual listing). 
Some common methods known to use Method Proxies are System.Action methods (actions that the engine will enact upon when called). Common inputs from Method Proxies are IButton, and ButtonEventData, both are not needed to still work. 
#### What you can do with Method Proxies
You can use Method Proxies when you want to call an internal method from the engine that is exposed and usable (presumed to be public method and not private method in the code) from a defined input from a user (i.e. a button press). This is also an alternative way to do the same call compared to using the node version of it (i.e. Using the Play function instead of the Play Flux node). However there is not really an advantage to doing it this way unless you have a good reason for it. 
One common use for this node is to help with [Cloud Spawning](https://wiki.resonite.com/Cloud_Spawning "Cloud Spawning"), utilizing the method "OnImportFile" within the component "FileMetadata". 
![](https://wiki.resonite.com/images/d/dd/InformationIcon.svg)
There is another node similar to this but returns data as well, called a [Function Proxy](https://wiki.resonite.com/ProtoFlux:Function_Proxy "ProtoFlux:Function Proxy"). 
Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:MethodProxy&oldid=110269](https://wiki.resonite.com/index.php?title=ProtoFlux:MethodProxy&oldid=110269)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:MethodProxy#top "Back to top \[home\]")
Contents
  * [ 1 What are Method Proxies ](https://wiki.resonite.com/ProtoFlux:MethodProxy#What_are_Method_Proxies)
  * [ 2 What you can do with Method Proxies ](https://wiki.resonite.com/ProtoFlux:MethodProxy#What_you_can_do_with_Method_Proxies)


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux](https://wiki.resonite.com/Category:ProtoFlux "Category:ProtoFlux")


Last modified
This page was last edited on 21 August 2025, at 00:27.
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


