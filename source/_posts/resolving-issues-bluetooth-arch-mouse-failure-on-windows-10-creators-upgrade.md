---
title: "Resolving Issues: Bluetooth Arch Mouse Failure on Windows 10 Creator's Upgrade"
date: 2024-08-18T09:48:53.603Z
updated: 2024-08-19T09:48:53.603Z
tags:
  - win11
  - win10
  - win7
categories:
  - driver
description: "This Article Describes Resolving Issues: Bluetooth Arch Mouse Failure on Windows 10 Creator's Upgrade"
excerpt: "This Article Describes Resolving Issues: Bluetooth Arch Mouse Failure on Windows 10 Creator's Upgrade"
thumbnail: https://thmb.techidaily.com/069b298bfedee9c280f30a09eb725e41e8884f90fc111239be7bdf14c7e0c06b.jpg
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
<li><a href="https://facebook-video-footage.techidaily.com/new-2024-approved-audio-recording-101-from-youtube-playback-to-files/"><u>[New] 2024 Approved  Audio Recording 101  From YouTube Playback To Files</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/new-2024-approved-from-still-shots-to-soundscapes-an-instagram-mp3-journey/"><u>[New] 2024 Approved  From Still Shots to Soundscapes  An Instagram-MP3 Journey</u></a></li>
<li><a href="https://fox-blue.techidaily.com/new-in-2024-unveiling-top-8-no-cost-3d-videos-players-pcmac/"><u>[New] In 2024, Unveiling Top 8 No-Cost 3D Videos Players PC/Mac</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/new-photographic-purity-and-proficiency-in-chromatic-control/"><u>[New] Photographic Purity and Proficiency in Chromatic Control</u></a></li>
<li><a href="https://facebook-videos.techidaily.com/updated-2024-approved-uploading-movies-instagram-guide/"><u>[Updated] 2024 Approved  Uploading Movies  Instagram Guide</u></a></li>
<li><a href="https://instagram-video-files.techidaily.com/updated-insta-cinematography-tips-three-way-borders-for-2024/"><u>[Updated] Insta Cinematography Tips  Three-Way Borders for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/athletes-guide-to-enhanced-gpt-interactions/"><u>Athlete's Guide to Enhanced GPT Interactions</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/brainpower-battlegrounds-gpt-and-google-bard-collide/"><u>Brainpower Battlegrounds: GPT & Google Bard Collide</u></a></li>
<li><a href="https://howto.techidaily.com/bricked-your-tecno-pop-8-heres-a-full-solution-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>Bricked Your Tecno Pop 8? Heres A Full Solution | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/caution-googles-bard-might-be-more-bug-than-genius/"><u>Caution: Google's Bard Might Be More Bug than Genius</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatai-profits-and-pc-building-hacks-for-enthusiasts/"><u>ChatAI Profits & PC Building Hacks for Enthusiasts</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-an-emerging-seo-hurdle/"><u>ChatGPT: An Emerging SEO Hurdle?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpts-role-in-the-future-classroom-five-essential-uses-for-students/"><u>ChatGPT's Role in the Future Classroom: Five Essential Uses for Students</u></a></li>
<li><a href="https://buynow-help.techidaily.com/construct-and-grow-unveiling-the-addictive-gameplay-of-cities-skylines/"><u>Construct & Grow: Unveiling the Addictive Gameplay of Cities: Skylines</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/crafting-future-navigating-the-most-promising-ai-hardware-tech/"><u>Crafting Future: Navigating the Most Promising AI Hardware Tech</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/customize-today-accessible-8-innovative-gpt-services/"><u>Customize Today: Accessible 8 Innovative GPT Services</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/discovering-opportunities-6-ways-chatgpt-assists/"><u>Discovering Opportunities: 6 Ways ChatGPT Assists</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/excel-mastery-unlocked-embrace-chatgpts-ai-assistance/"><u>Excel Mastery Unlocked: Embrace ChatGPT's AI Assistance</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/generative-technology-and-new-work-realities/"><u>Generative Technology and New Work Realities</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ground-rules-to-learn-langchain-llms/"><u>Ground Rules to Learn LangChain LLMs</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-discern-legitimate-chatbot-ios-programs/"><u>How to Discern Legitimate ChatBot iOS Programs</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-install-and-run-chatgpt-as-a-windows-app/"><u>How to Install and Run ChatGPT as a Windows App</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/improve-health-regimens-with-top-8-ai-plugins/"><u>Improve Health Regimens with Top 8 AI Plugins</u></a></li>
<li><a href="https://review-topics.techidaily.com/in-2024-can-life360-track-you-when-your-vivo-y77t-is-off-drfone-by-drfone-virtual-android/"><u>In 2024, Can Life360 Track You When Your Vivo Y77t is off? | Dr.fone</u></a></li>
<li><a href="https://location-social.techidaily.com/in-2024-how-to-leave-a-life360-group-on-realme-12-pro-5g-without-anyone-knowing-drfone-by-drfone-virtual-android/"><u>In 2024, How To Leave a Life360 Group On Realme 12 Pro 5G Without Anyone Knowing? | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/innovate-communication-apples-siri-and-microsofts-chatgpt/"><u>Innovate Communication: Apple’s Siri & Microsoft's ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/instant-gpt-worldwide-entry-via-chatgpt-everywhere/"><u>Instant GPT Worldwide Entry via ChatGPT Everywhere</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/interactive-innovation-will-claude-surpass-gpts-skills/"><u>Interactive Innovation: Will Claude Surpass GPT's Skills?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/labor-landscapes-altered-by-ais-advances/"><u>Labor Landscapes Altered by AI's Advances</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/leverage-ai-for-reading-pdfs-with-these-four-tactics/"><u>Leverage AI for Reading PDFs with These Four Tactics</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mitigating-risks-gpt-modifications-and-your-data/"><u>Mitigating Risks: GPT Modifications & Your Data</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/openais-gpt-on-ubuntu-command-line-connections-with-shellgpt/"><u>OpenAI's GPT on Ubuntu: Command-Line Connections with ShellGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/optimizing-productivity-4-strategies-with-chatgpt/"><u>Optimizing Productivity: 4 Strategies with ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/protecting-originality-openais-gpt-output-detector/"><u>Protecting Originality: OpenAI's GPT Output Detector</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/regaining-full-access-to-chatgpt-post-blocking/"><u>Regaining Full Access to ChatGPT Post-Blocking</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/secure-and-eternalize-a-chatgpt-storage-solution/"><u>Secure & Eternalize: A ChatGPT Storage Solution</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/secure-communication-stopping-chatgpt-record-keeping/"><u>Secure Communication: Stopping ChatGPT Record Keeping</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/should-we-demonstrate-decorum-with-chatgpt-siri-and-more/"><u>Should We Demonstrate Decorum with ChatGPT? Siri & More</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/sifting-through-codegpt-can-it-realistically-write-complex-code/"><u>Sifting Through CodeGPT: Can It Realistically Write Complex Code?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-threat-of-gpt-to-seo-and-search-techniques/"><u>The Threat of GPT to SEO and Search Techniques</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-unpredictability-of-creative-writing-outside-algorithms/"><u>The Unpredictability of Creative Writing Outside Algorithms</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-unpredictable-consequences-of-unquestioned-ai/"><u>The Unpredictable Consequences of Unquestioned AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-workings-of-intrinsic-computerized-thinking-models/"><u>The Workings of Intrinsic Computerized Thinking Models</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/trimming-ai-hallucinations-six-effective-phrasing-strategies/"><u>Trimming AI Hallucinations: Six Effective Phrasing Strategies</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/understanding-gptzeros-function-in-ai-detection/"><u>Understanding GPTZero's Function in AI Detection</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-solutions-for-chatgpt-and-plugin-discrepancies/"><u>Unveiling Solutions for ChatGPT & Plugin Discrepancies</u></a></li>
<li><a href="https://technical-tips.techidaily.com/unveiling-the-secret-of-fans-saving-your-photos-on-instagram-easily/"><u>Unveiling the Secret of Fans Saving Your Photos on Instagram Easily</u></a></li>
<li><a href="https://ai-topics.techidaily.com/updated-in-2024-the-best-english-voice-generator-to-convert-text-into-desired-accent/"><u>Updated In 2024, The Best English Voice Generator To Convert Text Into Desired Accent</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/visual-visionaries-leveraging-gpt-4-and-dall-e-for-artistry/"><u>Visual Visionaries: Leveraging GPT-4 and DALL-E for Artistry</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/weighing-your-options-which-is-better-bing-chat-for-freelancers/"><u>Weighing Your Options: Which Is Better, Bing Chat for Freelancers?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/write-winning-cover-letters-with-the-help-of-chatgpt/"><u>Write Winning Cover Letters with the Help of ChatGPT</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=30901410&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/ce9a6fb2becc2d235e62b125e9260102/products/copy_1_copy_vMixCallScreenshot1-large.jpg" border="0"> vMix Pro - Software based live production. vMix Pro includes everything in vMix 4K plus 8 channels of Replay and 8 vMix Call 
This bundle includes Studio 200 for vMix from Virtualsetworks, HTTP Matrix 1.0 automation scheduler, and 4 introductory training videos from the Udemy vMix Basic to Amazing course. </a>
<!-- affiliate ads end -->