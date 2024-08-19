---
title: How To Fix the 'Printer Cannot Be Removed' Error in Windows (Complete Solution)
date: 2024-08-18T09:50:03.384Z
updated: 2024-08-19T09:50:03.384Z
tags:
  - win11
  - win10
  - win7
categories:
  - driver
description: This Article Describes How To Fix the 'Printer Cannot Be Removed' Error in Windows (Complete Solution)
excerpt: This Article Describes How To Fix the 'Printer Cannot Be Removed' Error in Windows (Complete Solution)
thumbnail: https://thmb.techidaily.com/7cdccda0c1b455cde02be352d145a5b4b55f977ca27570cd9c8cff441c6409c8.jpg
---

## Error Code 80240020: Comprehensive Troubleshooting Steps for Windows 10 Installation Issues Resolved

The**80240020** error happens usually when the Windows 10 files that you downloaded was not complete and the setup process still tried to do the upgrade to Windows 10\. Or it could be that your Windows 10 installation folder is unfinished or corrupted.

![](https://images.drivereasy.com/wp-content/uploads/2016/08/error-code-80240020.jpg)

Luckily, this is an easy question to solve. Please follow the steps below to get this problem fixed. **Step One**1) Navigate to**C:\\$Windows.\~BT**folder. If you cannot see this folder, please make sure that you have checked the hidden items.

![](https://images.drivereasy.com/wp-content/uploads/2016/08/windows-bt-600x427.jpg)

Delete as many files in this folder as you can. You might not be able to delete all the files due to permission issues. 2) Navigate to**C:\\Windows\\SoftwareDistribution\\Download** and delete all the files in this folder. Please note that you don’t have to delete**Download**folder, but rather, you need to delete the content in it.

![](https://images.drivereasy.com/wp-content/uploads/2016/08/softwaredistributiondownload.jpg)

3) Type**cmd.exe**in the search box in**Start**panel and right click the option**cmd**and choose**Run as administrator**. ![](https://images.drivereasy.com/wp-content/uploads/2016/08/run-as-administrator.jpg)Click**Yes**at this prompt.

![](https://images.drivereasy.com/wp-content/uploads/2016/08/uac-command-processor.jpg)

4) Type**wuauclt.exe/updatenow**and hit**Enter**key. ![](https://images.drivereasy.com/wp-content/uploads/2016/08/img_57b5394edbd33.png) **Step Two** **Warning**: Before you proceed with this step, please make sure that you have back up your registry first just in case any irreversible errors happen. Refer to this post to see[**how to backup and restore your registry**](https://tools.techidaily.com/drivereasy/download/). 1) Press**Windows key**and**R**at the same time, then type in**regedit**and hit**Enter**. When prompted for administrator permission, click**Yes** to continue.

![](https://images.drivereasy.com/wp-content/uploads/2016/10/regedit.png)

2) Then follow the path:   **HKEY\_LOCAL\_MACHINE\\SOFTWARE\\Microsoft\\Windows\\CurrentVersion\\WindowsUpdate\\OSUpgrade**

![](https://images.drivereasy.com/wp-content/uploads/2016/10/hkey_local_machinesoftwaremicrosoftwindowscurrentversionwindowsupdateosupgrade-600x394.jpg)

3) On the right side of the pane, right click on the blank spot and select**New > DWORD (32-bit) Value**.

![](https://images.drivereasy.com/wp-content/uploads/2016/10/new-dword-32-bit-value-600x396.jpg)

4) Rename the value to**AllowOSUpgrade**. Then double click the value and set the**Value data**to**1**. Then click**OK**to save the change.

![](https://images.drivereasy.com/wp-content/uploads/2016/10/img_58140207aba43-600x394.jpg)

 Your**Windows Update** panel should come out in a couple of seconds. If it won’t open automatically, you can open this panel from Control Panel manually. Then, you should be able to download your Windows 10 from scratch.

The steps above also work if you are having a**80080080** or **8024600A**  error code. Usually the error is common with Windows 8.1 users, but for those who are using Windows 7, this solution applies as well. If the problem still persists, please be patient, Windows update takes time to download the upgrades in the background. If you still could not get this problem fixed, your Windows update tool might be corrupted so the security settings and background process is now malfunctioned. In this case, it is suggested that you burn the DVD or CD or USB flash drive with Windows 10 ISO files in to do the clean install from scratch. If you want to know how to do it, please refer to[this post here](https://tools.techidaily.com/drivereasy/download/) for more information.

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
<li><a href="https://fox-blue.techidaily.com/new-guide-to-using-eraser-tool-in-photoshop/"><u>[New] Guide to Using Eraser Tool In Photoshop</u></a></li>
<li><a href="https://facebook-videos.techidaily.com/new-unleash-the-skys-potential-with-drone-livestreaming-on-fb-for-2024/"><u>[New] Unleash the Sky's Potential with Drone Livestreaming on FB for 2024</u></a></li>
<li><a href="https://tiktok-video-recordings.techidaily.com/updated-creating-popular-jujutsu-kaisen-tiktok-content/"><u>[Updated] Creating Popular Jujutsu Kaisen TikTok Content</u></a></li>
<li><a href="https://screen-activity-recording.techidaily.com/updated-in-2024-guide-to-excellent-voice-recorders-for-macs/"><u>[Updated] In 2024, Guide to Excellent Voice Recorders for Macs</u></a></li>
<li><a href="https://fox-access.techidaily.com/2024-approved-15-innovative-cost-free-photo-manipulation-software/"><u>2024 Approved  15 Innovative, Cost-Free Photo Manipulation Software</u></a></li>
<li><a href="https://fox-links.techidaily.com/2024-approved-premium-fonts-with-dynamic-movement/"><u>2024 Approved  Premium Fonts with Dynamic Movement</u></a></li>
<li><a href="https://some-guidance.techidaily.com/2024-approved-unraveling-photoshops-magic-with-image-curving/"><u>2024 Approved  Unraveling Photoshop’s Magic with Image Curving</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-in-action-future-of-website-content-discovery/"><u>AI in Action: Future of Website Content Discovery</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-mediator-conquering-lifes-stresses/"><u>AI Mediator: Conquering Life's Stresses</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ais-creative-domain-who-holds-the-title/"><u>AI's Creative Domain: Who Holds The Title?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/assessing-intelligence-progressive-approaches-post-turing/"><u>Assessing Intelligence: Progressive Approaches Post-Turing</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/become-an-expert-in-chatgpt-with-this-chrome-extension/"><u>Become an Expert in ChatGPT with This Chrome Extension</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/bert-vs-gpt-the-evolution-of-nlp-technology/"><u>BERT vs GPT: The Evolution of NLP Technology</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/best-affordable-openai-image-modifiers/"><u>Best Affordable OpenAI Image Modifiers</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/beyond-human-conversation-googles-gemini-vs-chatgpts-standards/"><u>Beyond Human Conversation? Google's Gemini Vs. ChatGPT’s Standards</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/carve-out-your-chatai-masterpiece/"><u>Carve Out Your ChatAI Masterpiece</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/contrasting-ais-gpt-versus-bings-dialogue-assistant/"><u>Contrasting AIs: GPT versus Bing's Dialogue Assistant</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/convenient-bavarder-implementation-in-linux/"><u>Convenient Bavarder Implementation in Linux</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/creating-interactive-web-platforms-with-gpt-3-integration/"><u>Creating Interactive Web Platforms with GPT-3 Integration</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/decoding-the-enigma-of-chatgpt-logout-problems/"><u>Decoding the Enigma of ChatGPT Logout Problems</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/disconnect-for-peace-how-to-drop-off-gpts-radar/"><u>Disconnect for Peace: How to Drop Off GPT's Radar</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/do-real-world-dialogues-enhance-chatgpts-knowledge-base/"><u>Do Real-World Dialogues Enhance ChatGPT’s Knowledge Base?</u></a></li>
<li><a href="https://location-social.techidaily.com/does-find-my-friends-work-on-vivo-y100-drfone-by-drfone-virtual-android/"><u>Does find my friends work on Vivo Y100 | Dr.fone</u></a></li>
<li><a href="https://driver-install.techidaily.com/enhance-samsung-monojet-output-on-windows-11/"><u>Enhance Samsung MonoJet Output on Windows 11</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/from-concept-to-commercial-chatgpts-story/"><u>From Concept to Commercial: ChatGPT's Story</u></a></li>
<li><a href="https://extra-tips.techidaily.com/in-2024-comprehensive-scrutiny-gear-360s-virtual-reality-capability/"><u>In 2024, Comprehensive Scrutiny  Gear 360'S Virtual Reality Capability</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/in-2024-sim-unlock-xiaomi-13t-pro-phones-without-code-2-ways-to-remove-android-sim-lock-by-drfone-android/"><u>In 2024, Sim Unlock Xiaomi 13T Pro Phones without Code 2 Ways to Remove Android Sim Lock</u></a></li>
<li><a href="https://driver-install.techidaily.com/install-latest-sound-driver-in-windows-7/"><u>Install Latest Sound Driver in Windows 7</u></a></li>
<li><a href="https://extra-resources.techidaily.com/link-films-for-organized-youtube-display/"><u>Link Films for Organized YouTube Display</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/narrative-design-aided-by-gpt-3-insights/"><u>Narrative Design Aided by GPT-3 Insights</u></a></li>
<li><a href="https://extra-resources.techidaily.com/quick-start-utilizing-zoom-in-windows-10-systems/"><u>Quick Start  Utilizing Zoom in Windows 10 Systems</u></a></li>
<li><a href="https://common-error.techidaily.com/resolving-hdmi-connectivity-issues-windows-10-wont-recognize-your-tv/"><u>Resolving HDMI Connectivity Issues: Windows 10 Won't Recognize Your TV</u></a></li>
<li><a href="https://buynow-marvelous.techidaily.com/sky-dominance-why-professionals-prefer-the-dji-mavic-2/"><u>Sky Dominance: Why Professionals Prefer the DJI Mavic 지 2 프로</u></a></li>
<li><a href="https://video-screen-grab.techidaily.com/step-by-step-guide-to-iphone-screen-capturing/"><u>Step-by-Step Guide to Iphone Screen Capturing</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-future-of-friendly-faces-snapchat-ai-vs-gpt-powered-convo/"><u>The Future of Friendly Faces: Snapchat AI vs GPT-Powered Convo</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-future-of-storytelling-chatais-potential/"><u>The Future of Storytelling: ChatAI's Potential</u></a></li>
<li><a href="https://android-location-track.techidaily.com/top-6-appsservices-to-trace-any-xiaomi-civi-3-disney-100th-anniversary-edition-location-by-mobile-number-drfone-by-drfone-virtual-android/"><u>Top 6 Apps/Services to Trace Any Xiaomi Civi 3 Disney 100th Anniversary Edition Location By Mobile Number | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/voice-for-algorithms-chatgpts-new-command-respondive-capability/"><u>Voice for Algorithms: ChatGPT's New Command-Respondive Capability</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://25home.pxf.io/c/5597632/2090698/16836" target="_top" id="2090698"><img src="//a.impactradius-go.com/display-ad/16836-2090698" border="0" alt="" width="720" height="300"/></a>
<!-- affiliate ads end -->