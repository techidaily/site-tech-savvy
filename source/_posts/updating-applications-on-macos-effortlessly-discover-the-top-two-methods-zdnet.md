---
title: "Updating Applications on macOS Effortlessly: Discover the Top Two Methods | ZDNet"
date: 2024-12-25T20:02:23.777Z
updated: 2024-12-27T20:52:47.655Z
tags:
  - apple
categories:
  - tech
thumbnail: https://thmb.techidaily.com/d35e798d7cf8d00e558373e4952ec0178aa0674db22d4cc9c0a2fcdcf78387c6.jpg
---

## Two Simple Methods for Updating Applications on Your Mac OS - Insights

![fullscreen-1-4-24-7-23pm](https://www.zdnet.com/a/img/resize/4d0754ca50eca284946b9049b2a02512354bb4c1/2024/01/05/f413ba01-74e1-4edb-8d1e-41b8aa539d45/fullscreen-1-4-24-7-23pm.jpg?auto=webp&width=1280)

Screen Sharing on MacOS Sonoma

Jason Perlow/ZDNET

Any time I see updates available for my MacOS machines, I immediately apply them. Why? Because those updates often contain security patches that keep my computers safe. Those updates might also contain new features for apps or performance and reliability improvements. Either way, I find these updates to be an essential part of [maintaining the security of my devices](https://www.zdnet.com/article/how-to-update-every-apple-device/) and keeping my mind at ease.

**Also: [How I purged over 175GB of files from my Mac in under a minute (and you can too)](https://www.zdnet.com/article/how-i-purged-over-175gb-of-files-from-my-mac-in-under-a-minute/)**

When I go to update a MacOS device, I know there's more than one way to approach the task -- from the App Store (via the MacOS GUI) or from the command line. Because I've spent decades [working with Linux](https://www.zdnet.com/article/thinking-about-switching-to-linux-things-you-need-to-know/), I'm 100% comfortable using the command line, so I will sometimes open the terminal app, check for upgrades, and then run them when they're available. Or, if I'm feeling a bit lazy, I'll just go the App Store route.

Let me show you both approaches.

>  Disclaimer: This post includes affiliate links
>
>  If you click on a link and make a purchase, I may receive a commission at no extra cost to you.
>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/2Iv3DjT2Fyw?si=pR_z8ZDDVGF2MvKJ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## How to update MacOS apps from the App Store

**What you'll need:** The only things you'll need are an Apple device (a MacBook or iMac) and a valid user account on the machine. That's it. Let's get to the updates.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/_SbYznUy_zY?si=ThBkP934r3mizi48" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## 1\. Open the App Store

The fastest way to check and see if there are any updates available is by clicking the Apple button in the upper-left corner, where you might see something like _2 updates_ listed (indicating you have two apps that have updates available). Click that entry to open the App Store.

I have two available updates on my MacBook Pro.

Screenshot by Jack Wallen/ZDNET

#### Newsletters

ZDNET Tech Today

ZDNET's Tech Today newsletter is a daily briefing of the newest, most talked about stories, five days a week.

 Subscribe

[See all](https://www.zdnet.com/newsletters/)

## 2\. Update your apps

When the App Store opens, you can either update the apps individually (by clicking the Update button associated with the app in question) or update them all at once (by clicking Update All). During the update process, you might be prompted to close an app (or even a related app) if it's blocking the update from continuing. Should that be the case, close the app in question, return to the App Store, and click Continue from the pop-up warning.

These two apps on my MacBook Pro have pending updates.

Screenshot by Jack Wallen/ZDNET

Once the update is completed, close the App Store and you're done.

## How to update MacOS apps from the command line

This is a bit more complicated, for two reasons: first, you have to find out what apps are available for updating, and, second -- as with Linux -- the app names are case-sensitive.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/UcplMvRBulA?si=iBonbwDS1v7RAlHK" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## 1\. Open the Terminal app

To run commands, you must first open the terminal app, which can be done from the Launchpad. Click the Launchpad icon in your Dock and then type _terminal_. Click the launcher to open the Terminal app.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/T-ssCD10v2M?si=WVWGNayUiCAkMZzZ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## 2\. Check for available updates

Next, you need to run the command to check for updates. The command in question is _softwareupdate_ and is used for both checking and running the updates. To check for available updates, issue the command:

sudo softwareupdate -l

You will be prompted for your sudo password (which is your MacOS user password). 

**Also: [How to update every Apple device (iPhone, iPad, Apple Watch, Mac, more)](https://www.zdnet.com/article/how-to-update-every-apple-device/)**

The -l option stands for _list_. This will print out any available app updates and, if required, it will inform you if a restart is needed to complete any recent OS updates. If you see such a warning, make sure to do the reboot to complete the process.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/ZblaBc-v2vs?si=CKW1gJwXQT2vZJYo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## 3\. Update the apps

Let's say the command lists that Apple Mail has an update available, which should be listed as _Mail_ (remember, case sensitivity). Before you update the app, make sure to close it first. Once closed, update the app with a command like this:

sudo softwareupdate -i Mail

After successfully typing your sudo password, the update will proceed. When the update completes, you may or may not have to restart the machine. (You will be informed if a reboot is necessary.) You can then re-open the app you just updated and enjoy whatever fresh features or security patches the update applied.

**Also: [The Apple products you shouldn't buy this month](https://www.zdnet.com/article/the-apple-products-you-shouldnt-buy-this-month/)** 

This is about as simple a method as you'll find to help keep your MacOS machines running smoothly and securely. Never leave an app update lingering because it often contains security patches, which are required for the health and well-being of your operating system.

#### Apple

[iPhone 16 Pro upgrade: If you have a 3 year-old iPhone, here are all the new features you'll get](https://www.zdnet.com/article/iphone-16-pro-and-pro-max-hands-on/ "iPhone 16 Pro upgrade: If you have a 3 year-old iPhone, here are all the new features you'll get")

[My biggest regret with upgrading my iPhone to iOS 18 (and I'm not alone)](https://www.zdnet.com/article/my-biggest-regret-with-upgrading-my-iphone-to-ios-18-and-im-not-alone/ "My biggest regret with upgrading my iPhone to iOS 18 (and I'm not alone)")

[We've used every iPhone 16 model and here's our best buying advice for 2024](https://www.zdnet.com/article/iphone-16-pro-max-buying-advice-2024/ "We've used every iPhone 16 model and here's our best buying advice for 2024")

[6 iOS 18 settings I changed immediately - and why you should too](https://www.zdnet.com/article/6-ios-18-settings-i-changed-immediately-and-why-you-should-too/ "6 iOS 18 settings I changed immediately - and why you should too")

* [iPhone 16 Pro upgrade: If you have a 3 year-old iPhone, here are all the new features you'll get](https://www.zdnet.com/article/iphone-16-pro-and-pro-max-hands-on/ "iPhone 16 Pro upgrade: If you have a 3 year-old iPhone, here are all the new features you'll get")
* [My biggest regret with upgrading my iPhone to iOS 18 (and I'm not alone)](https://www.zdnet.com/article/my-biggest-regret-with-upgrading-my-iphone-to-ios-18-and-im-not-alone/ "My biggest regret with upgrading my iPhone to iOS 18 (and I'm not alone)")
* [We've used every iPhone 16 model and here's our best buying advice for 2024](https://www.zdnet.com/article/iphone-16-pro-max-buying-advice-2024/ "We've used every iPhone 16 model and here's our best buying advice for 2024")
* [6 iOS 18 settings I changed immediately - and why you should too](https://www.zdnet.com/article/6-ios-18-settings-i-changed-immediately-and-why-you-should-too/ "6 iOS 18 settings I changed immediately - and why you should too")

<ins class="adsbygoogle"
     style="display:block"
     data-ad-format="autorelaxed"
     data-ad-client="ca-pub-7571918770474297"
     data-ad-slot="1223367746"></ins>

<ins class="adsbygoogle"
     style="display:block"
     data-ad-client="ca-pub-7571918770474297"
     data-ad-slot="8358498916"
     data-ad-format="auto"
     data-full-width-responsive="true"></ins>

<span class="atpl-alsoreadstyle">Also read:</span>
<div><ul>
<li><a href="https://fox-cloud.techidaily.com/new-cutting-edge-cameras-top-15-picks-innovation/"><u>[New] Cutting-Edge Cameras Top 15 Picks Innovation</u></a></li>
<li><a href="https://fox-glue.techidaily.com/new-discovering-the-basics-of-digital-pixel-landscapes-for-2024/"><u>[New] Discovering the Basics of Digital Pixel Landscapes for 2024</u></a></li>
<li><a href="https://instagram-clips.techidaily.com/updated-2024-approved-how-to-change-your-voice-on-instagram/"><u>[Updated] 2024 Approved How to Change Your Voice on Instagram?</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/updated-building-brands-earning-dollars-a-comprehensive-guide-to-insta-sponsorships/"><u>[Updated] Building Brands, Earning Dollars A Comprehensive Guide to Insta-Sponsorships</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/updated-securely-distributing-exclusive-youtube-videos-through-gmail/"><u>[Updated] Securely Distributing Exclusive YouTube Videos Through Gmail</u></a></li>
<li><a href="https://extra-tips.techidaily.com/2024-approved-boosting-video-content-with-effective-srt-file-management/"><u>2024 Approved Boosting Video Content with Effective SRT File Management</u></a></li>
<li><a href="https://youtube-sure.techidaily.com/approved-fix-confirmed-shorts-are-showing-up/"><u>2024 Approved Fix Confirmed Shorts Are Showing Up</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/can-chatgpt-transform-healthcare/"><u>Can ChatGPT Transform Healthcare?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatbots-rising-the-transformation-of-digital-storytelling/"><u>Chatbots Rising: The Transformation of Digital Storytelling</u></a></li>
<li><a href="https://tech-hub.techidaily.com/1723809009078-comprehensive-insights-into-enterprise-level-search-systems-discover-your-best-option-today/"><u>Comprehensive Insights Into Enterprise-Level Search Systems - Discover Your Best Option Today</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/creating-nutritionally-sound-menus-with-chatgpt/"><u>Creating Nutritionally Sound Menus with ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/disabling-recording-privacy-focused-tips-for-chatgpt-users/"><u>Disabling Recording: Privacy-Focused Tips for ChatGPT Users</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/distinguishing-diverse-ai-usage-scenarios/"><u>Distinguishing Diverse AI Usage Scenarios</u></a></li>
<li><a href="https://fake-location.techidaily.com/fake-the-location-to-get-around-the-mlb-blackouts-on-itel-a70-drfone-by-drfone-virtual-android/"><u>Fake the Location to Get Around the MLB Blackouts on Itel A70 | Dr.fone</u></a></li>
<li><a href="https://change-location.techidaily.com/in-2024-4-methods-to-turn-off-life-360-on-infinix-smart-7-without-anyone-knowing-drfone-by-drfone-virtual-android/"><u>In 2024, 4 Methods to Turn off Life 360 On Infinix Smart 7 without Anyone Knowing | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/streamline-tasks-with-7-chatgpt-tips-for-optimal-output/"><u>Streamline Tasks with 7 ChatGPT Tips for Optimal Output</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-art-of-conversation-five-ways-to-steer-chatgpt/"><u>The Art of Conversation: Five Ways to Steer ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unlocking-potential-web-designs-using-ai-chatgpt-guide/"><u>Unlocking Potential Web Designs Using AI: ChatGPT Guide</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-top-5-non-commercial-art-influencers/"><u>Unveiling Top 5 Non-Commercial Art Influencers</u></a></li>
</ul></div>

