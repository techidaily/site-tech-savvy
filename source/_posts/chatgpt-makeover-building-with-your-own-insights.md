---
title: "ChatGPT Makeover: Building with Your Own Insights"
date: 2024-08-21T15:40:39.721Z
updated: 2024-08-22T15:40:39.721Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes ChatGPT Makeover: Building with Your Own Insights"
excerpt: "This Article Describes ChatGPT Makeover: Building with Your Own Insights"
thumbnail: https://thmb.techidaily.com/78af3078c80b8e3712553330740f219cdae8af451a75522402de746ab069fea1.jpg
---

## ChatGPT Makeover: Building with Your Own Insights

 Providing GPT technology in a powerful and easy-to-use chatbot, ChatGPT has become the world's most popular AI tool. Many people use ChatGPT to provide engaging conversations, answer queries, offer creative suggestions, and aid in coding and writing. However, ChatGPT is limited as you cannot store your data for long-term personal use, and its September 2021 knowledge data cutoff point.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 As a workaround, we can use OpenAI's API and LangChain to provide ChatGPT with custom data and updated info past 2021 to create a custom ChatGPT instance.

## Why Provide ChatGPT with Custom Data?

 Feeding ChatGPT with custom data and providing updated information beyond its knowledge cutoff date provides several benefits over just using ChatGPT as usual. Here are a few of them:

* **Personalized Interactions:** By providing ChatGPT with custom data, users can create a more customized experience. The model can be trained on specific datasets relevant to individual users or organizations, resulting in responses tailored to their unique needs and preferences.
* **Domain-Specific Expertise:** Custom data integration allows ChatGPT to specialize in particular domains or industries. It can be trained on industry-specific knowledge, terminology, and trends, enabling more accurate and insightful responses within those specific areas.
* **Current and Accurate Information:** Access to updated information ensures that ChatGPT stays current with the latest developments and knowledge. It can provide accurate responses based on recent events, news, or research, making it a more reliable source of information.

 Now that you understand the importance of providing custom data to ChatGPT, here's a step-by-step on how to do so on your local computer.

## Step 1: Install and Download Software and Pre-Made Script

 Please note the following instructions are for a Windows 10 or Windows 11 machine.

 To provide custom data to ChatGPT, you'll need to install and download the latest Python3, Git, Microsoft C++, and the ChatGPT-retrieval script from GitHub. If you already have some of the software installed on your PC, make sure they are updated with the latest version to avoid any hiccups during the process.

 Start by installing:

* **Download:**[Python3](https://www.python.org/downloads/) (Free)
* **Download:**[Git](https://git-scm.com/downloads) (Free)
* **Download:**[Microsoft Visual Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/) (Free)

### Python3 and Microsoft C++ Installation Notes

 When installing Python3, make sure that you tick the **Add python.exe to PATH** option before clicking **Install Now**. This is important as it allows you to access Python in any directory on your computer.

![Adding Python to PATH](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/1-download-python.jpg)

 When Installing Microsoft C++, you'll want to install **Microsoft Visual Studio Build Tools** first. Once installed, you can tick the **Desktop development with C++** option and click **Install** with all the optional tools automatically ticked on the right sidebar.

![Installing Microsoft C++ through Build Tools](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/2-install-c.jpg)

 Now that you have installed the latest versions of Python3, Git, and Microsoft C++, you can download the Python script to easily query custom local data.

**Download:** [ChatGPT-retrieval script](https://github.com/techleadhd/chatgpt-retrieval) (Free)

 To download the script, click on **Code,** then select **Download ZIP**. This should download the Python script into your default or selected directory.

![Downloading Python script on GitHub](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/3-download-script.jpg)

 Once downloaded, we can now set up a local environment.

<!-- affiliate ads begin -->
<a href="https://caperobbin.sjv.io/c/5597632/2006118/18460" target="_top" id="2006118"><img src="//a.impactradius-go.com/display-ad/18460-2006118" border="0" alt="" width="300" height="250"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2006118/18460" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Step 2: Set Up the Local Environment

 To set up the environment, you'll need to open a terminal in the chatgpt-retrieval-main folder you downloaded. To do that, open **chatgpt-retrieval-main** folder, right-click, and select **Open in Terminal**.

![Opening terminal on directory folder](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/4-open-terminal.jpg)

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2082538/7443" target="_top" id="2082538"><img src="//a.impactradius-go.com/display-ad/7443-2082538" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2082538/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 Once the terminal is open, copy and paste this command:

pip install langchain openai chromadb tiktoken unstructured

 This command uses Python's package manager to [create and manage the Python virtual environment](https://www.makeuseof.com/create-manage-python-virtual-environments/) needed.

 After creating the virtual environment, we need to supply an OpenAI API key to access their services. We'll first need to generate an API key from the [OpenAI API keys site](https://platform.openai.com/account/api-keys) by clicking on **Create new secret key**, adding a name for the key, then hitting the **Create secret key button**.

![Creating secret API key](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/generate-api-key.jpg)

<!-- affiliate ads begin -->
<a href="https://store.iobit.com/order/checkout.php?PRODS=4596923&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/184260348236f9554fe9375772ff966e/ascscan_468X60.png" border="0"></a>
<!-- affiliate ads end -->
 You will be provided with a string of characters. This is your OpenAI API key. Copy it by clicking on the copy icon on the side of the API key. Keep note that this API key should be kept secret. Do not share it with others unless you really intend for them to use it with you.

 Once copied, return to the chatgpt-retrieval-main folder and open constants with **Notepad**. Now replace the placeholder with your API key. Remember to save the file!

![Adding API key as environment variable](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/add-api-key.jpg)

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2082529/7443" target="_top" id="2082529"><img src="//a.impactradius-go.com/display-ad/7443-2082529" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2082529/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 Now that you have successfully set up your virtual environment and added your OpenAI API key as an environment variable. You can now provide your custom data to ChatGPT.

<!-- affiliate ads begin -->
<a href="https://shop.pcdj.com/order/checkout.php?PRODS=4698998&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/47f4b6321e9fd8e8f7326a6adc1a7c1e/products/MacBook_Pro_lyrx-withsinger-tv.png" border="0">LYRX is an easy-to-use karaoke software with the professional features karaoke hosts need to perform with precision. LYRX is karaoke show hosting software that supports all standard karaoke file types as well as HD video formats, and it’s truly fun to use. 
LYRX Karaoke Software MAC/WINDOWS (Includes Activation For 3 Machines)</a>
<!-- affiliate ads end -->
## Step 3: Adding Custom Data

 To add custom data, place all your custom text data in the **data** folder within chatgpt-retrieval-main. The format of the text data may be in the form of a PDF, TXT, or DOC.

![Adding custom data for ChatGPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/adding-data.jpg)

 As you can see from the screenshot above, I've added a text file containing a made-up personal schedule, an article I wrote on [AMD's Instinct Accelerators](https://www.makeuseof.com/what-are-amd-instinct-ai-accelerators/), and a PDF document.

## Step 4: Querying ChatGPT Through Terminal

 The Python script allows us to query data from the custom data we've added to the data folder and the internet. In other words, you will have access to the usual ChatGPT backend and all the data stored locally in the data folder.

 To use the script, run the python [chatgpt.py](http://chatgpt.py) script and then add your question or query as the argument.

python [chatgpt.py](http://chatgpt.py) "YOUR QUESTION"

 Make sure to put your questions in quotation marks.

 To test if we have successfully fed ChatGPT our data, I'll ask a personal question regarding the **Personal Sched.txt** file.

![Testing ChatGPT with custom data](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/visit.jpg)

 It worked! This means ChatGPT was able to read the Personal Sched.txt provided earlier. Now let's see if we have successfully fed ChatGPT with information it does not know due to its knowledge cutoff date.

![Asking custom ChatGPT about topic outside knowledge cut off data](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/m250x.jpg)

 As you can see, it correctly described the AMD Instinct MI250x, which was released after ChatGPT -3's knowledge cutoff date.

<!-- affiliate ads begin -->
<a href="https://bluetties.sjv.io/c/5597632/2039292/17094" target="_top" id="2039292"><img src="//a.impactradius-go.com/display-ad/17094-2039292" border="0" alt="BLUETTI NEW LAUNCH AC240" width="954" height="1020"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2039292/17094" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Limitations of Custom ChatGPT

 Although feeding GPT-3.5 with custom data opens more ways to apply and use the LLM, there are a few drawbacks and limitations.

 Firstly, you need to provide all the data yourself. You can still access all the knowledge of GPT-3.5 until its knowledge cutoff date; however, you must provide all the extra data. This means if you want your local model to be knowledgeable of a certain subject on the internet that GPT-3.5 don't already know, you'll have to go to the internet and scrape the data yourself and save it as a text on the data folder of chatgpt-retrieval-main.

 Another issue is that querying ChatGPT like this takes more time to load when compared to asking ChatGPT directly.

 Lastly, the only model currently available is GPT-3.5 Turbo. So even if you have access to GPT-4, you won't be able to use it to power your custom ChatGPT instance.

<!-- affiliate ads begin -->
<a href="https://printrendy.pxf.io/c/5597632/1453721/17020" target="_top" id="1453721"><img src="//a.impactradius-go.com/display-ad/17020-1453721" border="0" alt="" width="300" height="250"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1453721/17020" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Custom ChatGPT Is Awesome But Limited

 Providing custom data to ChatGPT is a powerful way to get more out of the model. Through this method, you can feed the model with any text data you want and prompt it just like regular ChatGPT, albeit with some limitations. However, this will change in the future as it becomes easier to integrate our data with the LLM, along with access to the latest GPT-4 model.

**SCROLL TO CONTINUE WITH CONTENT**

 As a workaround, we can use OpenAI's API and LangChain to provide ChatGPT with custom data and updated info past 2021 to create a custom ChatGPT instance.


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
<li><a href="https://eaxpv-info.techidaily.com/new-from-novice-to-money-maker-on-youtube-for-2024/"><u>[New] From Novice to Money-Maker on YouTube for 2024</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/new-orchestrating-originality-top-8-schools-for-story-innovation/"><u>[New] Orchestrating Originality  Top 8 Schools for Story Innovation</u></a></li>
<li><a href="https://extra-approaches.techidaily.com/updated-20plus-creative-photo-collage-ideas-to-light-up-your-life/"><u>[Updated] 20+ Creative Photo Collage Ideas to Light Up Your Life</u></a></li>
<li><a href="https://fox-links.techidaily.com/updated-in-2024-face-forward-comparing-apple-and-samsungs-face-detection-capabilities/"><u>[Updated] In 2024, Face Forward  Comparing Apple and Samsung's Face-Detection Capabilities</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/2024-approved-windows-movie-maker-the-ultimate-guide-to-youtube-video-production/"><u>2024 Approved  Windows Movie Maker  The Ultimate Guide to YouTube Video Production</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/effective-solutions-for-managing-excessive-cpu-consumption-caused-by-dwmexe-on-windows-exp/"><u>Effective Solutions for Managing Excessive CPU Consumption Caused by dwm.exe on Windows eXP</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/effortless-installation-guide-for-the-celebratory-version-of-windows-10-os-upgrade/"><u>Effortless Installation Guide for the Celebratory Version of Windows 10 OS Upgrade</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/experience-breathtaking-gameplay-fluidity-in-skyrim-special-editions-latest-fps-refresh/"><u>Experience Breathtaking Gameplay Fluidity in Skyrim Special Edition's Latest FPS Refresh</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/fixed-repairing-disk-errors-on-windows-11/"><u>Fixed: Repairing Disk Errors on Windows 11</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/fixing-cannot-log-into-account-errors-on-windows-10-solutions-explored/"><u>Fixing 'Cannot Log Into Account' Errors on Windows 10 - Solutions Explored</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/fixing-the-pure-monochrome-display-a-guide-to-resolving-windows-10s-black-and-white-screen-issue/"><u>Fixing the Pure Monochrome Display: A Guide to Resolving Windows 10'S Black and White Screen Issue</u></a></li>
<li><a href="https://tech-recovery.techidaily.com/future-proof-your-career-with-these-9-essential-skype-interview-tips-for-job-seekers/"><u>Future-Proof Your Career with These 9 Essential Skype Interview Tips for Job Seekers</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/headphone-jack-not-working-easy-fixes/"><u>Headphone Jack Not Working [Easy Fixes]</u></a></li>
<li><a href="https://instagram-clips.techidaily.com/heightened-aesthetics-editing-high-resolution-footage-in-fcpx-for-instagram/"><u>Heightened Aesthetics  Editing High-Resolution Footage in FCPX for Instagram</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-fix-the-printer-cannot-be-removed-error-in-windows-complete-solution/"><u>How To Fix the 'Printer Cannot Be Removed' Error in Windows (Complete Solution)</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-install-mods-for-fallout-4-on-your-pc-beginners-guide/"><u>How to Install Mods for Fallout 4 on Your PC - Beginner’s Guide</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-recover-vanished-desktop-icons-on-your-windows-11-machine-solution/"><u>How to Recover Vanished Desktop Icons on Your Windows 11 Machine (Solution)</u></a></li>
<li><a href="https://screen-activity-recording.techidaily.com/in-2024-a-critical-look-at-the-latest-camera-recording-systems/"><u>In 2024, A Critical Look at the Latest Camera Recording Systems</u></a></li>
<li><a href="https://youtube-clips.techidaily.com/in-2024-dynamic-arrangement-of-your-youtube-selections/"><u>In 2024, Dynamic Arrangement of Your YouTube Selections</u></a></li>
<li><a href="https://easy-unlock-android.techidaily.com/in-2024-everything-you-need-to-know-about-lock-screen-settings-on-your-realme-12-proplus-5g-by-drfone-android/"><u>In 2024, Everything You Need to Know about Lock Screen Settings on your Realme 12 Pro+ 5G</u></a></li>
<li><a href="https://instagram-clips.techidaily.com/in-2024-strategies-for-measuring-igtv-popularity-indicators/"><u>In 2024, Strategies for Measuring IGTV Popularity Indicators</u></a></li>
<li><a href="https://extra-information.techidaily.com/key-strategies-for-navigating-complex-youtube-discussions/"><u>Key Strategies for Navigating Complex YouTube Discussions</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-windows-11s-reset-this-pc-best-practices-for-timing-and-execution/"><u>Mastering Windows 11'S 'Reset This PC': Best Practices for Timing and Execution</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/maximizing-your-gaming-experience-the-definitive-guide-to-boosting-fps-in-counter-strike-global-offensive/"><u>Maximizing Your Gaming Experience: The Definitive Guide to Boosting FPS in Counter-Strike: Global Offensive</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/resolved-how-to-fix-the-snipping-tool-malfunction-in-windows-10-and-11/"><u>Resolved: How to Fix the Snipping Tool Malfunction in Windows 10 and 11</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/resolving-lag-issues-effective-strategies-to-eliminate-frame-rate-drops-in-apex-legends-on-your-computer/"><u>Resolving Lag Issues: Effective Strategies to Eliminate Frame Rate Drops in Apex Legends on Your Computer</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/set-up-your-iphone-hotspot-as-a-wi-fi-hotspot/"><u>Set Up Your iPhone Hotspot as a Wi-Fi Hotspot</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/solution-uncover-the-reasons-behind-your-sluggish-hp-notebook/"><u>Solution: Uncover the Reasons Behind Your Sluggish HP Notebook</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/solved-navigating-windows-11s-boot-configuration-for-beginners/"><u>Solved: Navigating Windows 11'S Boot Configuration for Beginners</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/solving-the-problem-what-to-do-when-you-see-missing-cddvd-drive-device-driver-message/"><u>Solving the Problem: What To Do When You See 'Missing CD/DVD Drive Device Driver' Message</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/step-by-step-guide-installing-your-realtek-device-drivers/"><u>Step-by-Step Guide: Installing Your Realtek Device Drivers</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/step-by-step-guide-restoring-realtek-hd-audio-on-microsofts-latest-operating-systems/"><u>Step-by-Step Guide: Restoring Realtek HD Audio on Microsoft's Latest Operating Systems</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/step-by-step-guide-reverting-back-to-previous-graphics-card-drivers-on-windows-10/"><u>Step-by-Step Guide: Reverting Back to Previous Graphics Card Drivers on Windows 10</u></a></li>
<li><a href="https://win-howtos.techidaily.com/understanding-and-fixing-windows-host-rundll32-stopped-functioning-errors-in-windows-os/"><u>Understanding and Fixing 'Windows Host (Rundll32) Stopped Functioning' Errors in Windows OS</u></a></li>
<li><a href="https://techno-recovery.techidaily.com/unveiling-windows-11s-battery-status-feature-a-comprehensive-guide/"><u>Unveiling Windows 11'S Battery Status Feature: A Comprehensive Guide</u></a></li>
</ul></div>
