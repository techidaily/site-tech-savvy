---
title: Resolving Windows 11 or 11S Lagging Initial Launch Issues
date: 2024-08-18T09:45:35.521Z
updated: 2024-08-19T09:45:35.521Z
tags:
  - win11
  - win10
  - win7
categories:
  - driver
description: This Article Describes Resolving Windows 11 or 11S Lagging Initial Launch Issues
excerpt: This Article Describes Resolving Windows 11 or 11S Lagging Initial Launch Issues
thumbnail: https://thmb.techidaily.com/900dc848292f751f63b27f646fc76a619bc7384a4aedd9106177497020dbae72.jpg
---

## Resolving Windows 10 Installation Issue - Fix Error Code 80 #

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
<li><a href="https://vimeo-videos.techidaily.com/new-vimeos-revenue-revolution-strategies-for-sustainable-earnings/"><u>[New] Vimeo's Revenue Revolution  Strategies for Sustainable Earnings</u></a></li>
<li><a href="https://instagram-clips.techidaily.com/updated-instagram-icons-unveiled-elevate-your-fame-and-followers-in-record-time-heres-how/"><u>[Updated] Instagram Icons Unveiled  Elevate Your Fame & Followers in Record Time – Here's How</u></a></li>
<li><a href="https://video-capture.techidaily.com/updated-ultimate-quicktime-lapse-setup-for-5/"><u>[Updated] Ultimate Quicktime-Lapse Setup for #5</u></a></li>
<li><a href="https://fox-friendly.techidaily.com/10-cost-free-multi-os-video-player-releases-for-2024/"><u>10 Cost-Free, Multi-OS Video Player Releases for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-in-action-future-of-website-content-discovery/"><u>AI in Action: Future of Website Content Discovery</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-mediator-conquering-lifes-stresses/"><u>AI Mediator: Conquering Life's Stresses</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ais-creative-domain-who-holds-the-title/"><u>AI's Creative Domain: Who Holds The Title?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/are-real-time-interactions-crucial-for-chatgpt-learning/"><u>Are Real-Time Interactions Crucial for ChatGPT Learning?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/artificial-emotionality-can-machines-provide-solace-or-stress/"><u>Artificial Emotionality: Can Machines Provide Solace or Stress?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/assessing-intelligence-progressive-approaches-post-turing/"><u>Assessing Intelligence: Progressive Approaches Post-Turing</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/authentification-assistant-openais-anti-fake-tech-for-gpt/"><u>Authentification Assistant: OpenAI’s Anti-Fake Tech for GPT</u></a></li>
<li><a href="https://graphic-issues.techidaily.com/banishing-blinking-light-from-asus-devices-simply/"><u>Banishing Blinking Light From ASUS Devices Simply</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/become-an-expert-in-chatgpt-with-this-chrome-extension/"><u>Become an Expert in ChatGPT with This Chrome Extension</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/bert-vs-gpt-the-evolution-of-nlp-technology/"><u>BERT vs GPT: The Evolution of NLP Technology</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/best-affordable-openai-image-modifiers/"><u>Best Affordable OpenAI Image Modifiers</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/beyond-human-conversation-googles-gemini-vs-chatgpts-standards/"><u>Beyond Human Conversation? Google's Gemini Vs. ChatGPT’s Standards</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/breaking-down-failed-attempts-at-gpt-alteration/"><u>Breaking Down Failed Attempts at GPT Alteration</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/carve-out-your-chatai-masterpiece/"><u>Carve Out Your ChatAI Masterpiece</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/cha-tting-with-ai-androids-voice-controlled-gpt-explained/"><u>Cha [T]ting with AI? Android's Voice Controlled GPT Explained</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-4-explored-the-pinnacle-of-social-verification/"><u>ChatGPT-4 Explored: The Pinnacle of Social Verification</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/contrasting-ais-gpt-versus-bings-dialogue-assistant/"><u>Contrasting AIs: GPT versus Bing's Dialogue Assistant</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/convenient-bavarder-implementation-in-linux/"><u>Convenient Bavarder Implementation in Linux</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/creating-interactive-web-platforms-with-gpt-3-integration/"><u>Creating Interactive Web Platforms with GPT-3 Integration</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/decoding-chatgpts-shared-link-ecosystem/"><u>Decoding ChatGPT's Shared Link Ecosystem</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/decoding-the-enigma-of-chatgpt-logout-problems/"><u>Decoding the Enigma of ChatGPT Logout Problems</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/disconnect-for-peace-how-to-drop-off-gpts-radar/"><u>Disconnect for Peace: How to Drop Off GPT's Radar</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/do-real-world-dialogues-enhance-chatgpts-knowledge-base/"><u>Do Real-World Dialogues Enhance ChatGPT’s Knowledge Base?</u></a></li>
<li><a href="https://facebook-clips.techidaily.com/elevate-your-digital-footprint-strategies-for-effective-fb-video-marketing/"><u>Elevate Your Digital Footprint  Strategies for Effective FB Video Marketing</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/from-concept-to-commercial-chatgpts-story/"><u>From Concept to Commercial: ChatGPT's Story</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/guard-your-data-from-malware-disguised-as-ai-helpers/"><u>Guard Your Data From Malware Disguised as AI Helpers</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/hugging-face-unveiling-its-role-in-modern-machine-learning/"><u>Hugging Face: Unveiling Its Role in Modern Machine Learning</u></a></li>
<li><a href="https://android-location.techidaily.com/in-2024-9-best-free-android-monitoring-apps-to-monitor-phone-remotely-for-your-motorola-edge-40-neo-drfone-by-drfone-virtual/"><u>In 2024, 9 Best Free Android Monitoring Apps to Monitor Phone Remotely For your Motorola Edge 40 Neo | Dr.fone</u></a></li>
<li><a href="https://twitter-videos.techidaily.com/in-2024-comedy-cornucopia-twitters-best/"><u>In 2024, Comedy Cornucopia  Twitter's Best</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/in-2024-easily-unlock-your-oppo-a58-4g-device-sim-by-drfone-android/"><u>In 2024, Easily Unlock Your Oppo A58 4G Device SIM</u></a></li>
<li><a href="https://ios-unlock.techidaily.com/in-2024-how-to-make-the-most-of-your-apple-iphone-13-pro-max-lock-screen-with-notifications-by-drfone-ios/"><u>In 2024, How to Make the Most of Your Apple iPhone 13 Pro Max Lock Screen with Notifications?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/integrating-chatgpt-into-the-crypto-realm/"><u>Integrating ChatGPT Into the Crypto Realm</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/introduction-to-ai-in-laymans-terms/"><u>Introduction to AI in Layman's Terms</u></a></li>
<li><a href="https://android-frp.techidaily.com/is-gsm-flasher-adb-legit-full-review-to-bypass-your-samsung-galaxy-s24-ultrafrp-lock-by-drfone-android/"><u>Is GSM Flasher ADB Legit? Full Review To Bypass Your Samsung Galaxy S24 UltraFRP Lock</u></a></li>
<li><a href="https://data-wizards.techidaily.com/mirage-gpt-modifier-exfiltrates-fb-accounts/"><u>Mirage GPT Modifier: Exfiltrates FB Accounts</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/narrative-design-aided-by-gpt-3-insights/"><u>Narrative Design Aided by GPT-3 Insights</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/reaching-new-heights-with-chatgpts-token-limit/"><u>Reaching New Heights with ChatGPT's Token Limit</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/securely-transporting-your-chatgpt-interactions/"><u>Securely Transporting Your ChatGPT Interactions</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/strategies-for-effective-communication-with-chatgpt-clients/"><u>Strategies for Effective Communication with ChatGPT Clients</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/tailoring-twitter-hashtags-insights-from-chatgpt/"><u>Tailoring Twitter Hashtags: Insights From ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/techniques-to-block-chatgpts-storage-of-conversations/"><u>Techniques to Block ChatGPT's Storage of Conversations</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-dawn-of-bard-googles-revolutionary-response-to-chatgpt/"><u>The Dawn of 'Bard' - Google's Revolutionary Response to ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-future-of-friendly-faces-snapchat-ai-vs-gpt-powered-convo/"><u>The Future of Friendly Faces: Snapchat AI vs GPT-Powered Convo</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-future-of-storytelling-chatais-potential/"><u>The Future of Storytelling: ChatAI's Potential</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/thoughtful-interactions-employing-gpt-ethically/"><u>Thoughtful Interactions: Employing GPT Ethically</u></a></li>
<li><a href="https://fake-location.techidaily.com/ultimate-guide-to-free-pptp-vpn-for-beginners-on-vivo-v27-pro-drfone-by-drfone-virtual-android/"><u>Ultimate Guide to Free PPTP VPN For Beginners On Vivo V27 Pro | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unleash-unparalleled-computing-power-on-the-go-with-our-portable-server-4tb-ram-480tb-nvme-and-ampere-altra-cpu-packed-in-a-fly-away-kit/"><u>Unleash Unparalleled Computing Power On-The-Go With Our Portable Server: 4TB RAM, 480TB NVMe, and Ampere Altra CPU Packed in a Fly-Away Kit</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/voice-for-algorithms-chatgpts-new-command-respondive-capability/"><u>Voice for Algorithms: ChatGPT's New Command-Respondive Capability</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<span id="1993650">
					<video width="720" height="300" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1993650.jpeg"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/22993-1993650">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1993650.jpeg" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:720px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fhomestyler.sjv.io%2Fc%2F5597632%2F1993650%2F22993'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1993650/22993" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->