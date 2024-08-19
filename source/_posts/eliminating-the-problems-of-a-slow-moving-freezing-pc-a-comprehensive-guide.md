---
title: "Eliminating the Problems of a Slow-Moving, Freezing PC: A Comprehensive Guide"
date: 2024-08-18T09:50:33.137Z
updated: 2024-08-19T09:50:33.137Z
tags:
  - win11
  - win10
  - win7
categories:
  - driver
description: "This Article Describes Eliminating the Problems of a Slow-Moving, Freezing PC: A Comprehensive Guide"
excerpt: "This Article Describes Eliminating the Problems of a Slow-Moving, Freezing PC: A Comprehensive Guide"
thumbnail: https://thmb.techidaily.com/6631d02aad6297e4d6f700e032b5f1a6df7f0a4821dff69d11f95fe1acb0191f.jpg
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
<li><a href="https://extra-guidance.techidaily.com/new-mastering-gopro-studio-ultimate-video-edits-step-by-step/"><u>[New] Mastering GoPro Studio  Ultimate Video Edits Step-by-Step</u></a></li>
<li><a href="https://extra-support.techidaily.com/new-navigate-the-art-of-film-with-xps-easy-tools/"><u>[New] Navigate the Art of Film with XP's Easy Tools</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/new-revolutionize-online-transmission-essential-browsers-screen-capture-vendors-for-2024/"><u>[New] Revolutionize Online Transmission  Essential Browsers' Screen Capture Vendors for 2024</u></a></li>
<li><a href="https://youtube-help.techidaily.com/new-select-5-high-quality-audio-headphones/"><u>[New] Select 5 High-Quality Audio Headphones</u></a></li>
<li><a href="https://some-guidance.techidaily.com/new-the-essentials-of-professional-level-audio-crossfade/"><u>[New] The Essentials of Professional-Level Audio Crossfade</u></a></li>
<li><a href="https://facebook-video-share.techidaily.com/updated-2024-approved-detailed-steps-to-supercharge-your-youtube-audio-content/"><u>[Updated] 2024 Approved  Detailed Steps to Supercharge Your YouTube Audio Content</u></a></li>
<li><a href="https://desktop-recording.techidaily.com/updated-broadcast-software-beyond-standard-obs-for-2024/"><u>[Updated] Broadcast Software Beyond Standard OBS for 2024</u></a></li>
<li><a href="https://youtube-sure.techidaily.com/approved-achieve-perfect-youtube-broadcasts-with-superior-webcams/"><u>2024 Approved  Achieve Perfect YouTube Broadcasts with Superior Webcams</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-restrictions-7-unanswerable-queries-by-gpt/"><u>AI Restrictions: 7 Unanswerable Queries by GPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/beyond-tokens-maximizing-chatgpt-capacity/"><u>Beyond Tokens: Maximizing ChatGPT Capacity</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/breaking-ground-as-a-language-engineer-for-chatbots/"><u>Breaking Ground as a Language Engineer for Chatbots</u></a></li>
<li><a href="https://extra-tips.techidaily.com/capture-perfection-dive-into-top-12-websites-offering-stock-photos-without-cost-for-2024/"><u>Capture Perfection  Dive Into Top 12 Websites Offering Stock Photos Without Cost for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/cha-tting-with-ai-androids-voice-controlled-gpt-explained/"><u>Cha [T]ting with AI? Android's Voice Controlled GPT Explained</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chaos-in-communication-why-hackers-love-gpt/"><u>Chaos in Communication: Why Hackers Love GPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/charting-the-past-the-inception-of-ai/"><u>Charting the Past: The Inception of AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpts-capability-in-mixing-drinks/"><u>ChatGPT's Capability in Mixing Drinks</u></a></li>
<li><a href="https://win-able.techidaily.com/comprehensive-guide-fixing-the-infamous-thaumaturge-game-crashes-on-personal-computers/"><u>Comprehensive Guide: Fixing the Infamous Thaumaturge Game Crashes on Personal Computers</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/crafting-a-well-balanced-meal-plan-via-ai-insights/"><u>Crafting a Well-Balanced Meal Plan via AI Insights</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/cutting-edge-mobile-technology-the-top-8-ai-apps-for-you/"><u>Cutting-Edge Mobile Technology: The Top 8 AI Apps for You</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/disregarding-6-ineffective-chatgpt-tools/"><u>Disregarding 6 Ineffective ChatGPT Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/effortless-history-handling-top-4-extensions-for-gpt-3/"><u>Effortless History Handling - Top 4 Extensions for GPT-3</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/elevate-your-public-speaking-with-these-ai-helpers/"><u>Elevate Your Public Speaking with These AI Helpers</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/exploring-the-limits-of-zerogpts-accuracy/"><u>Exploring the Limits of ZeroGPT's Accuracy</u></a></li>
<li><a href="https://extra-tips.techidaily.com/fundamentals-of-digital-tale-construction/"><u>Fundamentals of Digital Tale Construction</u></a></li>
<li><a href="https://driver-install.techidaily.com/gain-edge-in-gaming-download-gtx-1050-ti-drivers/"><u>Gain Edge in Gaming: Download GTX 1050 Ti Drivers</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/how-to-mirror-xiaomi-redmi-k70e-to-mac-drfone-by-drfone-android/"><u>How to Mirror Xiaomi Redmi K70E to Mac? | Dr.fone</u></a></li>
<li><a href="https://location-social.techidaily.com/how-to-sharefake-location-on-whatsapp-for-lava-yuva-3-drfone-by-drfone-virtual-android/"><u>How to Share/Fake Location on WhatsApp for Lava Yuva 3 | Dr.fone</u></a></li>
<li><a href="https://review-topics.techidaily.com/how-to-unlock-the-lock-screen-on-my-itel-by-drfone-android-unlock-android-unlock/"><u>How to Unlock the Lock Screen on my Itel</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-use-chatgpt-to-write-a-poem/"><u>How to Use ChatGPT to Write a Poem</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/huggingchat-insights-an-open-source-counterpart-with-no-cost/"><u>HuggingChat Insights: An Open Source Counterpart with No Cost</u></a></li>
<li><a href="https://location-social.techidaily.com/in-2024-how-to-activate-and-use-life360-ghost-mode-on-samsung-galaxy-f14-5g-drfone-by-drfone-virtual-android/"><u>In 2024, How To Activate and Use Life360 Ghost Mode On Samsung Galaxy F14 5G | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/launching-chatgpt-bash-scripts-and-shellgpt-tactics/"><u>Launching ChatGPT: Bash Scripts and ShellGPT Tactics</u></a></li>
<li><a href="https://extra-hints.techidaily.com/mastery-of-visual-storytelling-advanced-techniques-with-luts-in-after-effects/"><u>Mastery of Visual Storytelling  Advanced Techniques with LUTs in After Effects</u></a></li>
<li><a href="https://fox-hovers.techidaily.com/metaversal-musings-a-preamble-of-inspirational-thoughts/"><u>Metaversal Musings  A Preamble of Inspirational Thoughts</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mislead-no-more-recognize-real-and-rigged-chatgpt-apps/"><u>Mislead No More: Recognize Real and Rigged ChatGPT Apps!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/neural-networks-defended-against-inversion/"><u>Neural Networks Defended Against Inversion</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/openai-reveals-tool-against-unauthorized-gpt-outputs/"><u>OpenAI Reveals Tool Against Unauthorized GPT Outputs</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/optimize-your-speeches-top-7-ai-assistants/"><u>Optimize Your Speeches: Top 7 AI Assistants</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/peeking-behind-ais-curtain-black-box-dynamics/"><u>Peeking Behind AI's Curtain: Black Box Dynamics</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/perfecting-your-novels-cast-the-most-effective-gpt-techniques/"><u>Perfecting Your Novel's Cast: The Most Effective GPT Techniques</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/securely-transporting-your-chatgpt-interactions/"><u>Securely Transporting Your ChatGPT Interactions</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/shut-down-chatgpts-data-collection/"><u>Shut Down ChatGPT's Data Collection</u></a></li>
<li><a href="https://remote-screen-capture.techidaily.com/splitscreen-viewer-insights/"><u>SplitScreen Viewer Insights</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/talk-tech-titles-exploring-the-distinctions-between-gpt-and-bings-bot-dialogues/"><u>Talk Tech Titles: Exploring the Distinctions Between GPT & Bing's Bot Dialogues</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-bottom-line-on-chatgpt-as-an-earnings-engine/"><u>The Bottom Line on ChatGPT as an Earnings Engine</u></a></li>
<li><a href="https://extra-tips.techidaily.com/the-essential-list-of-gratuitous-quality-memes/"><u>The Essential List of Gratuitous, Quality Memes</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-ultimate-speakers-guide-to-controlling-chatgpt/"><u>The Ultimate Speaker's Guide to Controlling ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/thoughtful-interactions-employing-gpt-ethically/"><u>Thoughtful Interactions: Employing GPT Ethically</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/transform-your-web-design-projects-the-gpt-3-approach/"><u>Transform Your Web Design Projects: The GPT-3 Approach</u></a></li>
<li><a href="https://tech-revival.techidaily.com/upcoming-gpt-4-revolutionizing-diy-with-advanced-artificial-intelligence/"><u>Upcoming GPT-4: Revolutionizing DIY with Advanced Artificial Intelligence</u></a></li>
<li><a href="https://youtube-video-recordings.techidaily.com/video-enhancement-incorporating-youtube-into-slides/"><u>Video Enhancement  Incorporating YouTube Into Slides</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/when-algorithms-fail-the-perils-of-generative-ai/"><u>When Algorithms Fail: The Perils of Generative AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/why-ai-cant-spot-its-writing-faults/"><u>Why AI Can't Spot Its Writing Faults</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/writing-top-notch-resumes-chatgpt-guide/"><u>Writing Top-Notch Resumes: ChatGPT Guide</u></a></li>
</ul></div>

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=2337838&QTY=1&AFFILIATE=108875&CART=1"><iframe width="640" height="390" src="https://www.youtube.com/embed/rzZwphIv4RM" title="APFill - Ink and Toner Coverage Calculator" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe></a>
<!-- affiliate ads end -->