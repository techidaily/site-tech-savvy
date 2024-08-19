---
title: Quick-Fix Solutions to Accelerate Your Windows 10 Update Process
date: 2024-08-18T09:50:52.990Z
updated: 2024-08-19T09:50:52.990Z
tags:
  - win11
  - win10
  - win7
categories:
  - driver
description: This Article Describes Quick-Fix Solutions to Accelerate Your Windows 10 Update Process
excerpt: This Article Describes Quick-Fix Solutions to Accelerate Your Windows 10 Update Process
thumbnail: https://thmb.techidaily.com/03767135b547a749b9c8b697eb0f3d64de72d0e7747a0f822a4c06557ee99a61.jpg
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
<li><a href="https://digital-screen-recording.techidaily.com/new-in-2024-preventing-unseen-frames-in-video-captures/"><u>[New] In 2024, Preventing Unseen Frames in Video Captures</u></a></li>
<li><a href="https://location-fake.techidaily.com/10-best-fake-gps-location-spoofers-for-oppo-reno-11-pro-5g-drfone-by-drfone-virtual-android/"><u>10 Best Fake GPS Location Spoofers for Oppo Reno 11 Pro 5G | Dr.fone</u></a></li>
<li><a href="https://extra-hints.techidaily.com/2024-approved-a-complete-overview-regulating-snapchats-video-velocity/"><u>2024 Approved  A Complete Overview  Regulating Snapchat's Video Velocity</u></a></li>
<li><a href="https://extra-support.techidaily.com/2024-approved-learn-and-master-nft-generation-with-ease/"><u>2024 Approved  Learn and Master NFT Generation with Ease</u></a></li>
<li><a href="https://tech-recovery.techidaily.com/accept-invitation-to-shared-photo-library-via-iphone-easy-steps-inside/"><u>Accept Invitation to Shared Photo Library via iPhone – Easy Steps Inside</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/athletes-guide-to-enhanced-gpt-interactions/"><u>Athlete's Guide to Enhanced GPT Interactions</u></a></li>
<li><a href="https://extra-tips.techidaily.com/best-20-public-license-pubg-image-collections/"><u>Best 20 Public License PUBG Image Collections</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/caution-googles-bard-might-be-more-bug-than-genius/"><u>Caution: Google's Bard Might Be More Bug than Genius</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatai-profits-and-pc-building-hacks-for-enthusiasts/"><u>ChatAI Profits & PC Building Hacks for Enthusiasts</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpts-role-in-the-future-classroom-five-essential-uses-for-students/"><u>ChatGPT's Role in the Future Classroom: Five Essential Uses for Students</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/crafting-future-navigating-the-most-promising-ai-hardware-tech/"><u>Crafting Future: Navigating the Most Promising AI Hardware Tech</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/excel-mastery-unlocked-embrace-chatgpts-ai-assistance/"><u>Excel Mastery Unlocked: Embrace ChatGPT's AI Assistance</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/generative-technology-and-new-work-realities/"><u>Generative Technology and New Work Realities</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ground-rules-to-learn-langchain-llms/"><u>Ground Rules to Learn LangChain LLMs</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-discern-legitimate-chatbot-ios-programs/"><u>How to Discern Legitimate ChatBot iOS Programs</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-install-and-run-chatgpt-as-a-windows-app/"><u>How to Install and Run ChatGPT as a Windows App</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/improve-health-regimens-with-top-8-ai-plugins/"><u>Improve Health Regimens with Top 8 AI Plugins</u></a></li>
<li><a href="https://fox-links.techidaily.com/in-2024-lean-cloud-archive-efficient-low-cost-large-data/"><u>In 2024, Lean Cloud Archive  Efficient, Low-Cost Large Data</u></a></li>
<li><a href="https://screen-video-capture.techidaily.com/in-2024-mastering-windows-animation-top-9-apps-for-high-quality-gif-capture/"><u>In 2024, Mastering Windows Animation  Top 9 Apps for High-Quality GIF Capture</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/innovate-communication-apples-siri-and-microsofts-chatgpt/"><u>Innovate Communication: Apple’s Siri & Microsoft's ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/interactive-innovation-will-claude-surpass-gpts-skills/"><u>Interactive Innovation: Will Claude Surpass GPT's Skills?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mitigating-risks-gpt-modifications-and-your-data/"><u>Mitigating Risks: GPT Modifications & Your Data</u></a></li>
<li><a href="https://extra-information.techidaily.com/most-admired-iphone-based-podcast-platforms/"><u>Most Admired iPhone-Based Podcast Platforms</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/openais-gpt-on-ubuntu-command-line-connections-with-shellgpt/"><u>OpenAI's GPT on Ubuntu: Command-Line Connections with ShellGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/optimizing-productivity-4-strategies-with-chatgpt/"><u>Optimizing Productivity: 4 Strategies with ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/regaining-full-access-to-chatgpt-post-blocking/"><u>Regaining Full Access to ChatGPT Post-Blocking</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/secure-and-eternalize-a-chatgpt-storage-solution/"><u>Secure & Eternalize: A ChatGPT Storage Solution</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/should-we-demonstrate-decorum-with-chatgpt-siri-and-more/"><u>Should We Demonstrate Decorum with ChatGPT? Siri & More</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/sifting-through-codegpt-can-it-realistically-write-complex-code/"><u>Sifting Through CodeGPT: Can It Realistically Write Complex Code?</u></a></li>
<li><a href="https://extra-information.techidaily.com/the-ultimate-guide-to-ipados-drawing-wonders/"><u>The Ultimate Guide to iPadOS Drawing Wonders</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-unpredictability-of-creative-writing-outside-algorithms/"><u>The Unpredictability of Creative Writing Outside Algorithms</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/trimming-ai-hallucinations-six-effective-phrasing-strategies/"><u>Trimming AI Hallucinations: Six Effective Phrasing Strategies</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-solutions-for-chatgpt-and-plugin-discrepancies/"><u>Unveiling Solutions for ChatGPT & Plugin Discrepancies</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/weighing-your-options-which-is-better-bing-chat-for-freelancers/"><u>Weighing Your Options: Which Is Better, Bing Chat for Freelancers?</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4600114&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.epubor.com/images/drm-removal-feature2.png" border="0">Any DRM Removal for Mac： Remove DRM from Adobe, Kindle, Sony eReader, Kobo, etc, read your ebooks anywhere.</a>
<!-- affiliate ads end -->