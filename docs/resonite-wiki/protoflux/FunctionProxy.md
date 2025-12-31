# ProtoFlux:FunctionProxy

> Source: https://wiki.resonite.com/ProtoFlux:FunctionProxy

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
  * [English](https://wiki.resonite.com/ProtoFlux:FunctionProxy)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AFunctionProxy "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AFunctionProxy "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:FunctionProxy
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:FunctionProxy#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:FunctionProxy)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FunctionProxy&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FunctionProxy&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:FunctionProxy "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:FunctionProxy&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:FunctionProxy "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:FunctionProxy "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FunctionProxy&oldid=109845 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FunctionProxy&action=info "More information about this page")


Function Proxy
*
Next
This could be anything
This could be anything
This could be anything
This could be anything
This could be anything
This could be anything
Method
null
∅
CoreNodes
#### What are Function Proxies
The `Function Proxy` node is used to call a function from a component. Some components expose these functions by default such as [ProtoFluxTool](https://wiki.resonite.com/Component:ProtoFluxTool "Component:ProtoFluxTool"). More hidden functions can be exposed when using the mod "[Show Delegates](https://github.com/art0007i/ShowDelegates)" from [Arti](https://wiki.resonite.com/User:Arti "User:Arti"), to do so, go into the inspector of any slot and you should see "---- SYNC METHODS HERE ----", clicking on that should reveal the extra functions. Using your flux tool, grab the function you want, then open your [context menu](https://wiki.resonite.com/Context_menu "Context menu") and select the option "Proxy". This will spawn out a node with any number of input arguments depending on the function call you choose, including the outputs it will provide. 
The arguments on the Function Proxy node will be depending on the type it wants and also can depend on how many inputs it wants. This makes it very difficult to document the thousands of variants of this node (and is unwise to list them here unless there is a good explanation for the individual listing). 
Some common functions known to use Function Proxies are System.Action types (actions that the engine will enact upon when called). Common inputs from Function Proxies are System.Type arguments, which may be needed to make these nodes work. 
#### What you can do with Function Proxies
You can use Function Proxies when you want to call an internal function from the engine that is exposed and usable (presumed to be public functions and not private functions in the code) from a defined input from a user (i.e. a button press). This is also an alternative way to do the same call compared to using the node version of it. However there is not really an advantage to doing it this way unless you have a good reason for it. 
One common use for this node is to use [tools](https://wiki.resonite.com/Tools "Tools") and the functions within them to do things in a special way. 
![](https://wiki.resonite.com/images/d/dd/InformationIcon.svg)
There is another node similar to this but does not return anything, called a [Method Proxy](https://wiki.resonite.com/ProtoFlux:Method_Proxy "ProtoFlux:Method Proxy"). 
Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:FunctionProxy&oldid=109845](https://wiki.resonite.com/index.php?title=ProtoFlux:FunctionProxy&oldid=109845)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:FunctionProxy#top "Back to top \[home\]")
Contents
  * [ 1 What are Function Proxies ](https://wiki.resonite.com/ProtoFlux:FunctionProxy#What_are_Function_Proxies)
  * [ 2 What you can do with Function Proxies ](https://wiki.resonite.com/ProtoFlux:FunctionProxy#What_you_can_do_with_Function_Proxies)


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux](https://wiki.resonite.com/Category:ProtoFlux "Category:ProtoFlux")


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


