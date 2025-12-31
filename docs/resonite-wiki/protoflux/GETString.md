# ProtoFlux:GETString

> Source: https://wiki.resonite.com/ProtoFlux:GETString

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
  * [English](https://wiki.resonite.com/ProtoFlux:GETString)


Personal tools 
  * [](https://wiki.resonite.com/Special:MyTalk "Discussion about edits from this IP address \[n\]")
  * [](https://wiki.resonite.com/Special:MyContributions "A list of edits made from this IP address \[y\]")
  * [](https://wiki.resonite.com/index.php?title=Special:CreateAccount&returnto=ProtoFlux%3AGETString "You are encouraged to create an account and log in; however, it is not mandatory")
  * [](https://wiki.resonite.com/index.php?title=Special:UserLogin&returnto=ProtoFlux%3AGETString "You are encouraged to log in; however, it is not mandatory \[o\]")


#  ProtoFlux:GETString
From Resonite Wiki
[](https://wiki.resonite.com/ProtoFlux:GETString#top "Back to top \[home\]")
Views 
  * [](https://wiki.resonite.com/ProtoFlux:GETString)
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GETString&action=edit "This page is protected.
You can view its source \[e\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GETString&action=history "Past revisions of this page \[h\]")


associated-pages 
  * [ProtoFlux](https://wiki.resonite.com/ProtoFlux:GETString "View the subject page \[c\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux_talk:GETString&action=edit&redlink=1 "Discussion about the content page \(page does not exist\) \[t\]")


More actions
More 
Tools 
  * [](https://wiki.resonite.com/Special:WhatLinksHere/ProtoFlux:GETString "A list of all wiki pages that link here \[j\]")
  * [](https://wiki.resonite.com/Special:RecentChangesLinked/ProtoFlux:GETString "Recent changes in pages linked from this page \[k\]")
  * [](javascript:print\(\); "Printable version of this page \[p\]")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GETString&oldid=109847 "Permanent link to this revision of this page")
  * [](https://wiki.resonite.com/index.php?title=ProtoFlux:GETString&action=info "More information about this page")


GET String
*
OnSent
URL
OnResponse
OnError
OnDenied
StatusCode
Content
Network
GET String sends a HTTP request with GET method on call and decode its content with given charset in the `Content-Type` header (See [MDN](https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Type) to obtain more info about the header). Defaults to UTF-8 if charset is not present in the header, or the header itself does not exist. 
Authorization - i.e. via BasicAuth - is currently _not_ supported. 
![](https://wiki.resonite.com/images/d/dd/InformationIcon.svg)
This is not suitable for binary-transmission, as this node decodes the whole response as a human-readable string. Consider using one of the [Asset Providers](https://wiki.resonite.com/Category:Components:Assets "Category:Components:Assets") if your intention is fetching remote assets such as [Texture2D](https://wiki.resonite.com/Component:StaticTexture2D "Component:StaticTexture2D"). 
![](https://wiki.resonite.com/images/d/dd/InformationIcon.svg)
This node is best used with an impulse from the client actually wanting to fulfill the data transfer task. See [Security/Consent and surrounding info.](https://wiki.resonite.com/Connecting_Resonite_to_Other_Applications#Security_/_Consent "Connecting Resonite to Other Applications")
## Inputs
### * ([AsyncCall](https://wiki.resonite.com/Impulses "Impulses"))
Trigger to send a get request to the URL ([Uri](https://wiki.resonite.com/Type:Uri "Type:Uri")) server location 
### URL ([Uri](https://wiki.resonite.com/Type:Uri "Type:Uri"))
The server location to send the get request to. 
## Outputs
### OnSent ([AsyncCall](https://wiki.resonite.com/Impulses "Impulses"))
Fires immediately after the request is sent, so multiple async functions can happen in parallel. 
### OnResponse ([Continuation](https://wiki.resonite.com/Impulses "Impulses"))
Fires after the server has responded with either (TODO: Which responses are valid?) HTTP code and sent a string based response. The node will output these to their respective outputs during this pulse. 
### OnError ([Continuation](https://wiki.resonite.com/Impulses "Impulses"))
Fires after the HTTP client concludes that the request failed due to an underlying issue such as network connectivity, DNS failure, server certificate validation or timeout. 
### OnDenied ([Continuation](https://wiki.resonite.com/Impulses "Impulses"))
Fires after the user processing the request denied access request prompt to the Uri host, or denied by their setting. Please see [external connection page](https://wiki.resonite.com/Connecting_Resonite_to_Other_Applications#Security_/_Consent "Connecting Resonite to Other Applications") for more information. 
### StatusCode ([HTTP Status Code](https://wiki.resonite.com/Type:HttpStatusCode "Type:HttpStatusCode"))
The code that the server responded with, no matter if it failed, was denied, succeeded at a response, or returned an error. This only exists during the OnResponse ([Continuation](https://wiki.resonite.com/Impulses "Impulses")), OnError ([Continuation](https://wiki.resonite.com/Impulses "Impulses")), and OnDenied ([Continuation](https://wiki.resonite.com/Impulses "Impulses")) impulses. Default to 0 if request has not been sent, or terminaed by an error described in OnError section. 
### Content ([String](https://wiki.resonite.com/Type:String "Type:String"))
The response that the server gave, or message of the thrown exception during HTTP request. This only exists during the OnResponse ([Continuation](https://wiki.resonite.com/Impulses "Impulses")) impulse. 
Retrieved from "[https://wiki.resonite.com/index.php?title=ProtoFlux:GETString&oldid=109847](https://wiki.resonite.com/index.php?title=ProtoFlux:GETString&oldid=109847)"
Contents [ Back to top ](https://wiki.resonite.com/ProtoFlux:GETString#top "Back to top \[home\]")
Contents
  * [ 1 Inputs ](https://wiki.resonite.com/ProtoFlux:GETString#Inputs)
    * [ 1.1 * (AsyncCall) ](https://wiki.resonite.com/ProtoFlux:GETString#*_\(AsyncCall\))
    * [ 1.2 URL (Uri) ](https://wiki.resonite.com/ProtoFlux:GETString#URL_\(Uri\))
  * [ 2 Outputs ](https://wiki.resonite.com/ProtoFlux:GETString#Outputs)
    * [ 2.1 OnSent (AsyncCall) ](https://wiki.resonite.com/ProtoFlux:GETString#OnSent_\(AsyncCall\))
    * [ 2.2 OnResponse (Continuation) ](https://wiki.resonite.com/ProtoFlux:GETString#OnResponse_\(Continuation\))
    * [ 2.3 OnError (Continuation) ](https://wiki.resonite.com/ProtoFlux:GETString#OnError_\(Continuation\))
    * [ 2.4 OnDenied (Continuation) ](https://wiki.resonite.com/ProtoFlux:GETString#OnDenied_\(Continuation\))
    * [ 2.5 StatusCode (HTTP Status Code) ](https://wiki.resonite.com/ProtoFlux:GETString#StatusCode_\(HTTP_Status_Code\))
    * [ 2.6 Content (String) ](https://wiki.resonite.com/ProtoFlux:GETString#Content_\(String\))


[Categories](https://wiki.resonite.com/Special:Categories "Special:Categories"): 
  * [ProtoFlux:All](https://wiki.resonite.com/Category:ProtoFlux:All "Category:ProtoFlux:All")
  * [ProtoFlux:Network](https://wiki.resonite.com/Category:ProtoFlux:Network "Category:ProtoFlux:Network")


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


