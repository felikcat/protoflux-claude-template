# ProtoFlux:FireOnChange

> Source: https://wiki.resonite.com/ProtoFlux:FireOnChange

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
  * [English](https://wiki.resonite.com/ProtoFlux:FireOnChange)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AFireOnChange "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AFireOnChange "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:FireOnChange
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:FireOnChange#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:FireOnChange)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FireOnChange&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FireOnChange&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:FireOnChange "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:FireOnChange&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:FireOnChange "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:FireOnChange "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FireOnChange&oldid=113123 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:FireOnChange&action=info "More information about this page")


Fire On Change
OnlyForUser
OnChanged
Value
Flow
The **FireOnChange** node will [listen](https://wiki.resonite.com/Type:IExecutionChangeListener%601 "Type:IExecutionChangeListener`1") for changes on its input and fire an [impulse](https://wiki.resonite.com/Impulses "Impulses") for the specified [user](https://wiki.resonite.com/User "User") whenever there is a change in value across [updates](https://wiki.resonite.com/Update "Update"). 
This can be useful for providing complex behavior for a specific user whenever a value changes that existing components do not provide. 
## Inputs
### OnlyForUser ([User](https://wiki.resonite.com/Type:User "Type:User"))
The user that will listen to changes and fire the impulse. 
For best practice, this should never be left `null` or evaluated differently based on the user (e.g. via [LocalUser](https://wiki.resonite.com/ProtoFlux:LocalUser "ProtoFlux:LocalUser")). If this input is `null` and the node is parented under a user, then the impulse will be fired for said user. If this input is `null` and not parented under a user, or if this input evaluates differently for different users, then the impulse will _tend to_ be fired for the first user that sees the change in value. This is usually the one who caused the change in the first place. This could cause inconsistent behavior unless carefully managed. If the desired behavior is for an impulse to fire by every user that detects a change for them locally, then use the local version of this node, which is linked at the bottom of the page. 
### Value (Generic)
The value or object that should be listened to for changes. 
## Outputs
### OnChanged ([impulse](https://wiki.resonite.com/Impulses "Impulses"))
Fires a single [impulse](https://wiki.resonite.com/Impulses "Impulses") from the specified user whenever the provided input changes value across updates. 
## See also
  * [ProtoFlux:FireOnLocalChange](https://wiki.resonite.com/ProtoFlux:FireOnLocalChange "ProtoFlux:FireOnLocalChange") will fire an impulse for _every_ user that detects a change rather than a specific user.
  * [ProtoFlux:FireOnTrue](https://wiki.resonite.com/ProtoFlux:FireOnTrue "ProtoFlux:FireOnTrue")
  * [ProtoFlux:FireOnFalse](https://wiki.resonite.com/ProtoFlux:FireOnFalse "ProtoFlux:FireOnFalse")


Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:FireOnChange&oldid=113123](https://wiki.resonite.com/index.php?title=ProtoFlux:FireOnChange&oldid=113123)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:FireOnChange#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:FireOnChange#Inputs)
    * [ 1.1 OnlyForUser (User) ](https://wiki.resonite.com/ProtoFlux:FireOnChange#OnlyForUser_\(User\))
    * [ 1.2 Value (Generic) ](https://wiki.resonite.com/ProtoFlux:FireOnChange#Value_\(Generic\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:FireOnChange#Outputs)
    * [ 2.1 OnChanged (impulse) ](https://wiki.resonite.com/ProtoFlux:FireOnChange#OnChanged_\(impulse\))
  * [ 3 See also ](https://wiki.resonite.com/ProtoFlux:FireOnChange#See_also)


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Flow](https://wiki.resonite.com/Category:ProtoFlux:Flow "Category:ProtoFlux:Flow")
  * [Listener nodes](https://wiki.resonite.com/Category:Listener_nodes "Category:Listener nodes")


Last modified
This page was last edited on 19 September 2025, at 08:48.
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


