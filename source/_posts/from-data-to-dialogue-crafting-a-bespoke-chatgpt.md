---
title: "From Data to Dialogue: Crafting a Bespoke ChatGPT"
date: 2024-09-02T20:36:23.449Z
updated: 2024-09-03T20:36:23.449Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes From Data to Dialogue: Crafting a Bespoke ChatGPT"
excerpt: "This Article Describes From Data to Dialogue: Crafting a Bespoke ChatGPT"
thumbnail: https://thmb.techidaily.com/13161d4780beb13fc4b02e6aea02c1375d88cd123ec37a972f3b6c973af210c4.jpg
---

## From Data to Dialogue: Crafting a Bespoke ChatGPT

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

<!-- affiliate ads begin -->
<a href="https://coinrule.sjv.io/c/5597632/1958374/18409" target="_top" id="1958374"><img src="//a.impactradius-go.com/display-ad/18409-1958374" border="0" alt="" width="300" height="300"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1958374/18409" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
### Python3 and Microsoft C++ Installation Notes

 When installing Python3, make sure that you tick the **Add python.exe to PATH** option before clicking **Install Now**. This is important as it allows you to access Python in any directory on your computer.

![Adding Python to PATH](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/1-download-python.jpg)

 When Installing Microsoft C++, you'll want to install **Microsoft Visual Studio Build Tools** first. Once installed, you can tick the **Desktop development with C++** option and click **Install** with all the optional tools automatically ticked on the right sidebar.

![Installing Microsoft C++ through Build Tools](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/2-install-c.jpg)

<!-- affiliate ads begin -->
<a href="https://twopages.pxf.io/c/5597632/2016067/18544" target="_top" id="2016067"><img src="//a.impactradius-go.com/display-ad/18544-2016067" border="0" alt="" width="1020" height="380"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2016067/18544" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 Now that you have installed the latest versions of Python3, Git, and Microsoft C++, you can download the Python script to easily query custom local data.

**Download:** [ChatGPT-retrieval script](https://github.com/techleadhd/chatgpt-retrieval) (Free)

 To download the script, click on **Code,** then select **Download ZIP**. This should download the Python script into your default or selected directory.

![Downloading Python script on GitHub](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/3-download-script.jpg)

<!-- affiliate ads begin -->
<iframe id="iframe_672" src="//a.impactradius-go.com/gen-ad-code/5597632/1959812/17834/" width="720" height="300" scrolling="no" frameborder="0" marginheight="0" marginwidth="0"></iframe>
<!-- affiliate ads end -->
 Once downloaded, we can now set up a local environment.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4615471&QTY=1&AFFILIATE=108875&CART=1"><img src="https://images.wondershare.com/affiliate-image/affiliate_banners_en/max_782x90.png" border="0"></a>
<!-- affiliate ads end -->
## Step 2: Set Up the Local Environment

 To set up the environment, you'll need to open a terminal in the chatgpt-retrieval-main folder you downloaded. To do that, open **chatgpt-retrieval-main** folder, right-click, and select **Open in Terminal**.

![Opening terminal on directory folder](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/4-open-terminal.jpg)

 Once the terminal is open, copy and paste this command:

pip install langchain openai chromadb tiktoken unstructured

 This command uses Python's package manager to [create and manage the Python virtual environment](https://www.makeuseof.com/create-manage-python-virtual-environments/) needed.

 After creating the virtual environment, we need to supply an OpenAI API key to access their services. We'll first need to generate an API key from the [OpenAI API keys site](https://platform.openai.com/account/api-keys) by clicking on **Create new secret key**, adding a name for the key, then hitting the **Create secret key button**.

![Creating secret API key](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/generate-api-key.jpg)

 You will be provided with a string of characters. This is your OpenAI API key. Copy it by clicking on the copy icon on the side of the API key. Keep note that this API key should be kept secret. Do not share it with others unless you really intend for them to use it with you.

 Once copied, return to the chatgpt-retrieval-main folder and open constants with **Notepad**. Now replace the placeholder with your API key. Remember to save the file!

![Adding API key as environment variable](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/add-api-key.jpg)

 Now that you have successfully set up your virtual environment and added your OpenAI API key as an environment variable. You can now provide your custom data to ChatGPT.

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

<!-- affiliate ads begin -->
<a href="https://modlily.sjv.io/c/5597632/2072819/17059" target="_top" id="2072819"><img src="//a.impactradius-go.com/display-ad/17059-2072819" border="0" alt="" width="300" height="250"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2072819/17059" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 It worked! This means ChatGPT was able to read the Personal Sched.txt provided earlier. Now let's see if we have successfully fed ChatGPT with information it does not know due to its knowledge cutoff date.

![Asking custom ChatGPT about topic outside knowledge cut off data](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/m250x.jpg)

<!-- affiliate ads begin -->
<a href="https://laganoo.pxf.io/c/5597632/1657397/16446" target="_top" id="1657397"><img src="//a.impactradius-go.com/display-ad/16446-1657397" border="0" alt="" width="336" height="280"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1657397/16446" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 As you can see, it correctly described the AMD Instinct MI250x, which was released after ChatGPT -3's knowledge cutoff date.

## Limitations of Custom ChatGPT

 Although feeding GPT-3.5 with custom data opens more ways to apply and use the LLM, there are a few drawbacks and limitations.

 Firstly, you need to provide all the data yourself. You can still access all the knowledge of GPT-3.5 until its knowledge cutoff date; however, you must provide all the extra data. This means if you want your local model to be knowledgeable of a certain subject on the internet that GPT-3.5 don't already know, you'll have to go to the internet and scrape the data yourself and save it as a text on the data folder of chatgpt-retrieval-main.

 Another issue is that querying ChatGPT like this takes more time to load when compared to asking ChatGPT directly.

 Lastly, the only model currently available is GPT-3.5 Turbo. So even if you have access to GPT-4, you won't be able to use it to power your custom ChatGPT instance.

<!-- affiliate ads begin -->
<a href="https://ephamedtechinc.pxf.io/c/5597632/2097467/26400?prodsku=B700" target="_top" id="2097467"><img src="//a.impactradius-go.com/display-ad/26400-2097467" border="0" alt="" width="640" height="640"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2097467/26400" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://extra-resources.techidaily.com/new-capturing-radiance-advanced-techniques-in-ps-hdr/"><u>[New] Capturing Radiance  Advanced Techniques in PS HDR</u></a></li>
<li><a href="https://youtube-data.techidaily.com/iggles-in-the-garage-ingenious-funny-video-concepts-for-youtubers/"><u>[New] Giggles in the Garage  Ingenious Funny Video Concepts for YouTubers</u></a></li>
<li><a href="https://youtube-lab.techidaily.com/n-2024-youtube-earnings-update-what-you-need-to-know/"><u>[New] In 2024, YouTube Earnings Update - What You Need to Know</u></a></li>
<li><a href="https://some-skills.techidaily.com/new-the-art-of-panoramic-capture-9-techniques-to-perfection/"><u>[New] The Art of Panoramic Capture  9 Techniques to Perfection</u></a></li>
<li><a href="https://discord-videos.techidaily.com/updated-2024-approved-unplugging-the-servers-deleting-discord-on-devices/"><u>[Updated] 2024 Approved  Unplugging the Servers  Deleting Discord on Devices</u></a></li>
<li><a href="https://video-screen-grab.techidaily.com/updated-elevate-your-online-engagements-with-pc-and-phone-recordings/"><u>[Updated] Elevate Your Online Engagements with PC & Phone Recordings</u></a></li>
<li><a href="https://fox-cloud.techidaily.com/updated-in-2024-premiere-ready-text-configurations/"><u>[Updated] In 2024, Premiere-Ready Text Configurations</u></a></li>
<li><a href="https://article-posts.techidaily.com/2024-approved-free-high-quality-srt-translation-services-1-8/"><u>2024 Approved  Free, High-Quality SRT Translation Services – #1-#8</u></a></li>
<li><a href="https://android-location-track.techidaily.com/9-best-phone-monitoring-apps-for-xiaomi-redmi-k70-pro-drfone-by-drfone-virtual-android/"><u>9 Best Phone Monitoring Apps for Xiaomi Redmi K70 Pro | Dr.fone</u></a></li>
<li><a href="https://tech-revival.techidaily.com/a-world-without-boundaries-with-gpt-4/"><u>A World Without Boundaries with GPT-4</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/altering-email-on-protonbrowser-a-comprehensive-guide/"><u>Altering Email on ProtonBrowser - A Comprehensive Guide</u></a></li>
<li><a href="https://howto.techidaily.com/app-wont-open-on-your-samsung-galaxy-a23-5g-here-are-all-fixes-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>App Wont Open on Your Samsung Galaxy A23 5G? Here Are All Fixes | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/artistic-integrity-vs-tech-might-the-sarah-silverman-suit/"><u>Artistic Integrity Vs. Tech Might: The Sarah Silverman Suit</u></a></li>
<li><a href="https://win11.techidaily.com/bypass-ignored-win11-themes-worth-checking/"><u>Bypass Ignored: Win11 Themes Worth Checking</u></a></li>
<li><a href="https://network-issues.techidaily.com/cease-oled-screens-stutter/"><u>Cease OLED Screens Stutter</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/deciphering-chatgpt-control-pros-and-cons/"><u>Deciphering ChatGPT Control: Pros & Cons</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/decoding-six-common-car-ai-configurations-fails/"><u>Decoding Six Common Car AI Configurations Fails</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/digital-storytelling-engaging-text-based-rpg-with-chatgpt/"><u>Digital Storytelling: Engaging Text-Based RPG with ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/evaluating-artificial-companions-in-psychological-care/"><u>Evaluating Artificial Companions in Psychological Care</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/github-copilot-vs-chatgpt-which-is-better-for-programming/"><u>GitHub Copilot Vs. ChatGPT: Which Is Better for Programming?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ideal-enhancements-boosting-chatgpt-and-vs-code-synergy/"><u>Ideal Enhancements: Boosting ChatGPT & VS Code Synergy</u></a></li>
<li><a href="https://extra-resources.techidaily.com/in-2024-a-comprehensive-guide-to-canon-time-lapse-video/"><u>In 2024, A Comprehensive Guide to Canon Time-Lapse Video</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/in-2024-how-to-turn-off-suggested-posts-on-instagram/"><u>In 2024, How to Turn Off Suggested Posts on Instagram?</u></a></li>
<li><a href="https://youtube-help.techidaily.com/in-2024-the-art-of-youtube-trailers-using-filmora-tools/"><u>In 2024, The Art of YouTube Trailers Using Filmora Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/inside-ais-frailty-decoding-how-prompt-injection-threat-operates/"><u>Inside AI's Frailty: Decoding How Prompt Injection Threat Operates</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/is-fake-gps-location-spoofer-a-good-choice-on-realme-gt-neo-5-drfone-by-drfone-virtual-android/"><u>Is Fake GPS Location Spoofer a Good Choice On Realme GT Neo 5? | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/laughter-algorithm-computing-milestones-and-privacy-in-the-cloud/"><u>Laughter Algorithm: Computing Milestones & Privacy in the Cloud</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/overcoming-the-top-4-barriers-in-your-gpt-account/"><u>Overcoming the Top 4 Barriers in Your GPT Account</u></a></li>
<li><a href="https://driver-error.techidaily.com/quick-guide-to-taming-nonstop-buzzing-of-bluetooth-devices-on-latest-os-update-fix-revealed/"><u>Quick Guide to Taming Nonstop Buzzing of Bluetooth Devices on Latest OS Update ![Fix Revealed]</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/safety-advisory-chatgpt-for-windowsnot-a-security-risk/"><u>Safety Advisory: ChatGPT for Windows—Not a Security Risk</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/shielding-sensitive-information-from-customized-ai/"><u>Shielding Sensitive Information From Customized AI</u></a></li>
<li><a href="https://driver-download.techidaily.com/solution-for-the-undetectable-tl-wn722n-wifi-adapter-on-windows-platforms/"><u>Solution for the Undetectable TL-WN722N WiFi Adapter on Windows Platforms</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/stealthy-gpt-conversation-archiving-strategies/"><u>Stealthy GPT Conversation Archiving Strategies</u></a></li>
<li><a href="https://technical-tips.techidaily.com/step-by-step-guide-successfully-disabling-safe-mode-in-windows-11/"><u>Step-by-Step Guide: Successfully Disabling Safe Mode in Windows 11</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/subscriptionshutdowns-seeking-new-access-era/"><u>SubscriptionShutdowns: Seeking New Access Era</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/surprising-fact-start-a-dialogue-with-chatgpt/"><u>Surprising Fact: Start a Dialogue with ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-9-most-overlooked-dangers-when-using-ai-for-mental-support/"><u>The 9 Most Overlooked Dangers When Using AI for Mental Support</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-journey-from-concept-to-collection-via-chatgpt/"><u>The Journey From Concept to Collection via ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-power-of-conversational-ai-for-workflow-optimization/"><u>The Power of Conversational AI for Workflow Optimization</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-spectrum-of-ai-intelligence-what-difference/"><u>The Spectrum of AI Intelligence: What Difference?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-synergy-of-technology-and-spirituality-with-chatgpt/"><u>The Synergy of Technology and Spirituality with ChatGPT</u></a></li>
<li><a href="https://technical-tips.techidaily.com/top-5-iphone-gps-navigation-apps-you-cant-live-without/"><u>Top 5 iPhone GPS Navigation Apps You Can't Live Without</u></a></li>
<li><a href="https://buynow-info.techidaily.com/top-rated-protective-covers-for-ipad-pro-13-the-ultimate-selection/"><u>Top Rated Protective Covers for iPad Pro 13 - The Ultimate Selection</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ubuntu-bash-integrating-shellgpt-with-openais-chatgpt/"><u>Ubuntu Bash: Integrating ShellGPT with OpenAI's ChatGPT</u></a></li>
<li><a href="https://unlock-android.techidaily.com/unlock-your-xiaomi-redmi-note-12-proplus-5gs-potential-the-top-20-lock-screen-apps-you-need-to-try-by-drfone-android/"><u>Unlock Your Xiaomi Redmi Note 12 Pro+ 5Gs Potential The Top 20 Lock Screen Apps You Need to Try</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-7-issues-with-generative-ai-for-chats/"><u>Unveiling 7 Issues with Generative AI for Chats</u></a></li>
<li><a href="https://some-tips.techidaily.com/unveiling-asmrs-benefits-a-health-perspective-for-2024/"><u>Unveiling ASMR’s Benefits  A Health Perspective for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-auto-gpt-download-and-installation/"><u>Unveiling Auto-GPT: Download & Installation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/voice-activated-strategies-for-directing-ai-5-gpt-techniques/"><u>Voice-Activated Strategies for Directing AI: 5 GPT Techniques</u></a></li>
</ul></div>
