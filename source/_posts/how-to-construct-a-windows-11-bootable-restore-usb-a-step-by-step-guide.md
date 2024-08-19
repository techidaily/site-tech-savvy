---
title: "How to Construct a Windows 11 Bootable Restore USB: A Step-by-Step Guide"
date: 2024-08-18T09:50:42.195Z
updated: 2024-08-19T09:50:42.195Z
tags:
  - win11
  - win10
  - win7
categories:
  - driver
description: "This Article Describes How to Construct a Windows 11 Bootable Restore USB: A Step-by-Step Guide"
excerpt: "This Article Describes How to Construct a Windows 11 Bootable Restore USB: A Step-by-Step Guide"
thumbnail: https://thmb.techidaily.com/527ec40dbef906cadfd5828e1a10f887ec75fd463af4e51940397e62459c5f66.jpg
---

## Error Code 80240020 Deciphered: Easy Steps to Successfully Install Windows 10 without a Glitch

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
<li><a href="https://some-guidance.techidaily.com/new-is-there-a-cash-incentive-in-critique-videos/"><u>[New] Is There a Cash Incentive in Critique Videos?</u></a></li>
<li><a href="https://fox-http.techidaily.com/new-the-secret-sauce-to-swipe-right-crafting-captivating-bio-on-tinder/"><u>[New] The Secret Sauce to Swipe Right  Crafting Captivating Bio on Tinder</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/updated-2024-approved-choosing-the-right-lights-and-cameras-for-youtube-videos/"><u>[Updated] 2024 Approved  Choosing the Right Lights & Cameras for YouTube Videos</u></a></li>
<li><a href="https://on-screen-recording.techidaily.com/updated-the-complete-guide-to-voice-overs-in-multimedia-projects/"><u>[Updated] The Complete Guide to Voice-Overs in Multimedia Projects</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/adventure-coding-roleplaying-games-in-the-gpt-world/"><u>Adventure Coding: Roleplaying Games in the GPT World</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/bypassing-gpt-text-length-limits/"><u>Bypassing GPT Text Length Limits</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/bypassing-gpts-char-count-restrictions/"><u>Bypassing GPT's Char Count Restrictions</u></a></li>
<li><a href="https://technical-tips.techidaily.com/can-you-chat-with-messenger-alone-tips-for-a-standalone-experience/"><u>Can You Chat with Messenger Alone? Tips for a Standalone Experience</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/challenging-ai-the-case-for-altering-chatgpt/"><u>Challenging AI: The Case for Altering ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-plus-a-toolkit-for-fluency-in-new-languages/"><u>ChatGPT Plus: A Toolkit for Fluency in New Languages</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-beyond-standard-interactions-with-custom-instructions/"><u>ChatGPT: Beyond Standard Interactions with Custom Instructions</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatxt-influence-on-modern-media-production/"><u>ChaTxt Influence on Modern Media Production</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/colorizing-your-folders-in-macos-a-step-by-step-guide/"><u>Colorizing Your Folders in macOS – A Step-by-Step Guide</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/craft-instructions-like-a-pro-discover-the-top-7-online-aids/"><u>Craft Instructions Like a Pro: Discover the Top 7 Online Aids</u></a></li>
<li><a href="https://youtube-sure.techidaily.com/ing-attention-a-look-at-the-best-15-video-intro-plans/"><u>Crafting Attention  A Look at the Best 15 Video Intro Plans</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/dissecting-ai-threat-prompt-injection-attacks-defined/"><u>Dissecting AI Threat - Prompt Injection Attacks Defined</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/dissecting-deceptions-how-to-differentiate-real-data-from-artifico/"><u>Dissecting Deceptions: How to Differentiate Real Data From Artifico</u></a></li>
<li><a href="https://android-location.techidaily.com/easy-ways-to-manage-your-xiaomi-redmi-note-12-5g-location-settings-drfone-by-drfone-virtual/"><u>Easy Ways to Manage Your Xiaomi Redmi Note 12 5G Location Settings | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/enhance-efficiency-by-ditching-these-6-chatgpt-apps/"><u>Enhance Efficiency by Ditching These 6 ChatGPT Apps</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/etiquette-essentials-when-speaking-to-alexa-or-similar-tech/"><u>Etiquette Essentials When Speaking to Alexa or Similar Tech</u></a></li>
<li><a href="https://howto.techidaily.com/fixes-for-apps-keep-crashing-on-itel-a05s-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>Fixes for Apps Keep Crashing on Itel A05s | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/guiding-steps-linking-gpt-3-to-whatsapp-assistance/"><u>Guiding Steps: Linking GPT-3 to WhatsApp Assistance</u></a></li>
<li><a href="https://location-social.techidaily.com/how-to-fake-snapchat-location-on-nokia-c02-drfone-by-drfone-virtual-android/"><u>How to Fake Snapchat Location on Nokia C02 | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-smooth-out-gpts-body-stream-glitches/"><u>How to Smooth Out GPT's Body Stream Glitches</u></a></li>
<li><a href="https://android-unlock.techidaily.com/how-to-unlock-samsung-galaxy-m14-5g-phone-without-any-data-loss-by-drfone-android/"><u>How to Unlock Samsung Galaxy M14 5G Phone without Any Data Loss</u></a></li>
<li><a href="https://extra-support.techidaily.com/in-2024-optimal-hue-refiner-app/"><u>In 2024, Optimal Hue Refiner App</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/integrating-gpt-4-into-chatgpt-for-instant-results/"><u>Integrating GPT-4 Into ChatGPT for Instant Results</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/launch-budget-friendly-home-based-chatgpt-alternative/"><u>Launch Budget-Friendly, Home-Based ChatGPT Alternative</u></a></li>
<li><a href="https://extra-information.techidaily.com/m1-demystified-apple-redefines-chipset-technology/"><u>M1 Demystified  Apple Redefines Chipset Technology</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-conversational-support-merging-gpt-with-whatsapp/"><u>Mastering Conversational Support: Merging GPT with WhatsApp</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/perfecting-dialogues-advanced-strategies-for-chatgpt/"><u>Perfecting Dialogues: Advanced Strategies for ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/reimagined-ai-gpts-revolutionary-innovations-unveiled/"><u>Reimagined AI: GPT's Revolutionary Innovations Unveiled</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-hidden-flaws-in-machine-conversations-gpts-eight-key-problems/"><u>The Hidden Flaws in Machine Conversations: GPT's Eight Key Problems</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-honest-or-deceptive-narrative-of-chatgpt/"><u>The Honest or Deceptive Narrative of ChatGPT</u></a></li>
<li><a href="https://some-approaches.techidaily.com/uncompromised-creativity-best-macos-big-sur-editing-tools-ranked-for-2024/"><u>Uncompromised Creativity  Best macOS Big Sur Editing Tools Ranked for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/upgrade-to-next-gen-search-perplexity-ai-unveiled/"><u>Upgrade to Next-Gen Search: Perplexity AI Unveiled</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/vacation-internet-tips-maximize-your-experience/"><u>Vacation Internet Tips: Maximize Your Experience</u></a></li>
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