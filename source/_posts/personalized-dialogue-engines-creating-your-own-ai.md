---
title: "Personalized Dialogue Engines: Creating Your Own AI"
date: 2024-08-03T00:53:15.321Z
updated: 2024-08-04T00:53:15.321Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Personalized Dialogue Engines: Creating Your Own AI"
excerpt: "This Article Describes Personalized Dialogue Engines: Creating Your Own AI"
thumbnail: https://thmb.techidaily.com/51b5c705b272c6a35f26cbee92033b8d25124b814164fccb1a1f598c30e520f7.jpg
---

## Personalized Dialogue Engines: Creating Your Own AI

 Providing GPT technology in a powerful and easy-to-use chatbot, ChatGPT has become the world's most popular AI tool. Many people use ChatGPT to provide engaging conversations, answer queries, offer creative suggestions, and aid in coding and writing. However, ChatGPT is limited as you cannot store your data for long-term personal use, and its September 2021 knowledge data cutoff point.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 As a workaround, we can use OpenAI's API and LangChain to provide ChatGPT with custom data and updated info past 2021 to create a custom ChatGPT instance.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2075475/7443" target="_top" id="2075475"><img src="//a.impactradius-go.com/display-ad/7443-2075475" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2075475/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
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

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4940312&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/333ac5d90817d69113471fbb6e531bee/sps-partnership-728x90eng.png" border="0"></a>
<!-- affiliate ads end -->
![Adding Python to PATH](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/1-download-python.jpg)

 When Installing Microsoft C++, you'll want to install **Microsoft Visual Studio Build Tools** first. Once installed, you can tick the **Desktop development with C++** option and click **Install** with all the optional tools automatically ticked on the right sidebar.

![Installing Microsoft C++ through Build Tools](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/2-install-c.jpg)

 Now that you have installed the latest versions of Python3, Git, and Microsoft C++, you can download the Python script to easily query custom local data.

**Download:** [ChatGPT-retrieval script](https://github.com/techleadhd/chatgpt-retrieval) (Free)

 To download the script, click on **Code,** then select **Download ZIP**. This should download the Python script into your default or selected directory.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2087389/7443" target="_top" id="2087389"><img src="//a.impactradius-go.com/display-ad/7443-2087389" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2087389/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![Downloading Python script on GitHub](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/3-download-script.jpg)

 Once downloaded, we can now set up a local environment.

## Step 2: Set Up the Local Environment

 To set up the environment, you'll need to open a terminal in the chatgpt-retrieval-main folder you downloaded. To do that, open **chatgpt-retrieval-main** folder, right-click, and select **Open in Terminal**.

<!-- affiliate ads begin -->
<a href="https://aspironcom.sjv.io/c/5597632/1941789/21554" target="_top" id="1941789"><img src="//a.impactradius-go.com/display-ad/21554-1941789" border="0" alt="" width="650" height="800"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1941789/21554" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![Opening terminal on directory folder](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/4-open-terminal.jpg)

 Once the terminal is open, copy and paste this command:

pip install langchain openai chromadb tiktoken unstructured

 This command uses Python's package manager to [create and manage the Python virtual environment](https://www.makeuseof.com/create-manage-python-virtual-environments/) needed.

 After creating the virtual environment, we need to supply an OpenAI API key to access their services. We'll first need to generate an API key from the [OpenAI API keys site](https://platform.openai.com/account/api-keys) by clicking on **Create new secret key**, adding a name for the key, then hitting the **Create secret key button**.

![Creating secret API key](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/generate-api-key.jpg)

 You will be provided with a string of characters. This is your OpenAI API key. Copy it by clicking on the copy icon on the side of the API key. Keep note that this API key should be kept secret. Do not share it with others unless you really intend for them to use it with you.

 Once copied, return to the chatgpt-retrieval-main folder and open constants with **Notepad**. Now replace the placeholder with your API key. Remember to save the file!

<!-- affiliate ads begin -->
<a href="https://caperobbin.sjv.io/c/5597632/2006123/18460" target="_top" id="2006123"><img src="//a.impactradius-go.com/display-ad/18460-2006123" border="0" alt="" width="300" height="250"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2006123/18460" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![Adding API key as environment variable](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/add-api-key.jpg)

 Now that you have successfully set up your virtual environment and added your OpenAI API key as an environment variable. You can now provide your custom data to ChatGPT.

## Step 3: Adding Custom Data

 To add custom data, place all your custom text data in the **data** folder within chatgpt-retrieval-main. The format of the text data may be in the form of a PDF, TXT, or DOC.

![Adding custom data for ChatGPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/adding-data.jpg)

 As you can see from the screenshot above, I've added a text file containing a made-up personal schedule, an article I wrote on [AMD's Instinct Accelerators](https://www.makeuseof.com/what-are-amd-instinct-ai-accelerators/), and a PDF document.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2075471/7443" target="_top" id="2075471"><img src="//a.impactradius-go.com/display-ad/7443-2075471" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2075471/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Step 4: Querying ChatGPT Through Terminal

 The Python script allows us to query data from the custom data we've added to the data folder and the internet. In other words, you will have access to the usual ChatGPT backend and all the data stored locally in the data folder.

 To use the script, run the python [chatgpt.py](http://chatgpt.py) script and then add your question or query as the argument.

python [chatgpt.py](http://chatgpt.py) "YOUR QUESTION"

 Make sure to put your questions in quotation marks.

 To test if we have successfully fed ChatGPT our data, I'll ask a personal question regarding the **Personal Sched.txt** file.

<!-- affiliate ads begin -->
<a href="https://godlikehost.sjv.io/c/5597632/1920047/21774" target="_top" id="1920047"><img src="//a.impactradius-go.com/display-ad/21774-1920047" border="0" alt="" width="300" height="250"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1920047/21774" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![Testing ChatGPT with custom data](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/visit.jpg)

 It worked! This means ChatGPT was able to read the Personal Sched.txt provided earlier. Now let's see if we have successfully fed ChatGPT with information it does not know due to its knowledge cutoff date.

![Asking custom ChatGPT about topic outside knowledge cut off data](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/m250x.jpg)

 As you can see, it correctly described the AMD Instinct MI250x, which was released after ChatGPT -3's knowledge cutoff date.

## Limitations of Custom ChatGPT

 Although feeding GPT-3.5 with custom data opens more ways to apply and use the LLM, there are a few drawbacks and limitations.

 Firstly, you need to provide all the data yourself. You can still access all the knowledge of GPT-3.5 until its knowledge cutoff date; however, you must provide all the extra data. This means if you want your local model to be knowledgeable of a certain subject on the internet that GPT-3.5 don't already know, you'll have to go to the internet and scrape the data yourself and save it as a text on the data folder of chatgpt-retrieval-main.

 Another issue is that querying ChatGPT like this takes more time to load when compared to asking ChatGPT directly.

 Lastly, the only model currently available is GPT-3.5 Turbo. So even if you have access to GPT-4, you won't be able to use it to power your custom ChatGPT instance.

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
<li><a href="https://facebook-clips.techidaily.com/new-acoustic-amplification-of-social-media-content-on-facebook/"><u>[New] Acoustic Amplification of Social Media Content on Facebook</u></a></li>
<li><a href="https://snapchat-videos.techidaily.com/new-in-2024-top-15-snapchat-sharing-tactics-for-maximum-impact/"><u>[New] In 2024, Top 15 Snapchat Sharing Tactics for Maximum Impact</u></a></li>
<li><a href="https://vp-tips.techidaily.com/new-unleash-creativity-androids-leading-drawing-software-selection-for-2024/"><u>[New] Unleash Creativity  Android's Leading Drawing Software Selection for 2024</u></a></li>
<li><a href="https://snapchat-videos.techidaily.com/updated-2024-approved-fiery-friendship-keeping-your-snapstreak-hot-and-steady/"><u>[Updated] 2024 Approved  Fiery Friendship  Keeping Your Snapstreak Hot and Steady</u></a></li>
<li><a href="https://fox-http.techidaily.com/updated-in-2024-illustrator-tutorial-bringing-text-to-life/"><u>[Updated] In 2024, Illustrator Tutorial  Bringing Text to Life</u></a></li>
<li><a href="https://facebook-video-footage.techidaily.com/updated-integrating-youtube-tracks-into-imovie-projects-easily/"><u>[Updated] Integrating YouTube Tracks Into iMovie Projects Easily</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/updated-masterclass-in-muting-and-dismantling-an-instagram-account/"><u>[Updated] Masterclass in Muting & Dismantling an Instagram Account</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/2024-approved-make-a-stir-in-the-app-ingenious-bio-strategies-to-captivate-swipes/"><u>2024 Approved  Make a Stir in the App - Ingenious Bio Strategies to Captivate Swipes</u></a></li>
<li><a href="https://digital-screen-recording.techidaily.com/2024-approved-unlocking-fullscreen-footage-screen-recording-made-simple-for-mac-users/"><u>2024 Approved  Unlocking Fullscreen Footage  Screen Recording Made Simple for Mac Users</u></a></li>
<li><a href="https://printer-issues.techidaily.com/2024s-guide-to-perfectly-pairing-hp-printer-with-laptops/"><u>2024'S Guide to Perfectly Pairing HP Printer with Laptops</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-journey-through-openais-gpt-generations/"><u>A Journey Through OpenAI’s GPT Generations</u></a></li>
<li><a href="https://bypass-frp.techidaily.com/addrom-bypass-an-android-tool-to-unlock-frp-lock-screen-for-your-google-pixel-7a-by-drfone-android/"><u>AddROM Bypass An Android Tool to Unlock FRP Lock Screen For your Google Pixel 7a</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/assessing-machine-intelligence-beyond-traditional-trials/"><u>Assessing Machine Intelligence Beyond Traditional Trials</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/automated-prose-perfection-the-hix-way/"><u>Automated Prose Perfection: The HIX Way</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/barricade-website-from-robotic-data-collectors/"><u>Barricade Website From Robotic Data Collectors</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/beyond-bots-separating-truth-from-ai-mythology/"><u>Beyond Bots: Separating Truth From AI Mythology</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/beyond-standard-the-top-10-customizations-for-chatgpt/"><u>Beyond Standard: The Top 10 Customizations for ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-the-ai-thats-revolutionizing-video-content-crafting/"><u>ChatGPT: The AI That's Revolutionizing Video Content Crafting</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721400487456-chatgpts-ios-application-launched/"><u>ChatGPT's iOS Application Launched!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/choosing-the-right-llm-unraveling-the-pros-and-cons-quickly/"><u>Choosing the Right LLM: Unraveling the Pros & Cons Quickly</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/conquer-language-varieties-chatgpt-techniques/"><u>Conquer Language Varieties: ChatGPT Techniques</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/content-construction-revolutionized-by-chatbot-innovation/"><u>Content Construction Revolutionized by Chatbot Innovation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/creating-characters-crafting-chronicles-gpts-sixfold-strategy/"><u>Creating Characters, Crafting Chronicles: GPT's Sixfold Strategy</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/deciphering-nlps-role-versus-mls-role/"><u>Deciphering NLP's Role Versus ML's Role</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/decoding-gpt4alls-functionality/"><u>Decoding GPT4All's Functionality</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/decoding-mathematical-conundrums/"><u>Decoding Mathematical Conundrums</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/duel-of-the-devices-github-copilot-vs-openais-gpt/"><u>Duel of the Devices: GitHub Copilot Vs. OpenAI's GPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/elons-explanation-grok-ai-functionality-relevance-and-associated-costs/"><u>Elon's Explanation: Grok AI Functionality, Relevance & Associated Costs</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/everyday-language-on-ai/"><u>Everyday Language on AI</u></a></li>
<li><a href="https://ai-driven-video-production.techidaily.com/expert-approved-highlight-video-makers-for-any-device-for-2024/"><u>Expert-Approved Highlight Video Makers for Any Device for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/exploring-chatgpts-integrity/"><u>Exploring ChatGPT's Integrity</u></a></li>
<li><a href="https://article-helps.techidaily.com/exploring-premium-free-lut-options-a-guide-to-quality-tools/"><u>Exploring Premium-Free LUT Options  A Guide to Quality Tools</u></a></li>
<li><a href="https://screen-video-capture.techidaily.com/gpu-chronicles-radeon-reimagined/"><u>GPU Chronicles  Radeon Reimagined</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/harness-the-power-of-ai-the-best-pdf-extensions-ranked/"><u>Harness the Power of AI: The Best PDF Extensions Ranked</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-avoidance-of-ai-in-keys-can-secure-your-windows-11-install/"><u>How Avoidance of AI in Keys Can Secure Your Windows 11 Install</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/important-8-gpt-advice-for-enhancing-concentration-in-a-digital-era/"><u>Important 8 GPT Advice for Enhancing Concentration in a Digital Era</u></a></li>
<li><a href="https://android-location-track.techidaily.com/in-2024-2-ways-to-monitor-samsung-galaxy-m54-5g-activity-drfone-by-drfone-virtual-android/"><u>In 2024, 2 Ways to Monitor Samsung Galaxy M54 5G Activity | Dr.fone</u></a></li>
<li><a href="https://video-capture.techidaily.com/in-2024-expert-techniques-to-efficiently-manipulate-whiteboards-in-web-conferencing-tools/"><u>In 2024, Expert Techniques to Efficiently Manipulate Whiteboards in Web Conferencing Tools</u></a></li>
<li><a href="https://bypass-frp.techidaily.com/in-2024-full-guide-to-bypass-samsung-galaxy-a05s-frp-by-drfone-android/"><u>In 2024, Full Guide to Bypass Samsung Galaxy A05s FRP</u></a></li>
<li><a href="https://android-unlock.techidaily.com/in-2024-how-to-use-google-assistant-on-your-lock-screen-of-samsung-galaxy-a54-5g-phone-by-drfone-android/"><u>In 2024, How to Use Google Assistant on Your Lock Screen Of Samsung Galaxy A54 5G Phone</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/in-2024-instagram-disconnect-watch-stay-ahead/"><u>In 2024, Instagram Disconnect Watch  Stay Ahead</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/inside-hugging-face-concept-and-applications/"><u>Inside Hugging Face: Concept & Applications</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/integrating-chatgpt-into-diverse-language-settings/"><u>Integrating ChatGPT Into Diverse Language Settings</u></a></li>
<li><a href="https://extra-information.techidaily.com/kickstarting-a-successful-social-good-campaign-online/"><u>Kickstarting a Successful Social Good Campaign Online</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/leap-into-advanced-chatgpt-top-9-essential-plugins-here/"><u>Leap Into Advanced ChatGPT – Top 9 Essential Plugins Here</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/leveraging-chatgpt-for-impressive-resumes/"><u>Leveraging ChatGPT for Impressive Resumes</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/leveraging-chatgpt-to-streamline-corporate-operations-and-strategy/"><u>Leveraging ChatGPT to Streamline Corporate Operations and Strategy</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/misinformation-clear-gpt-win-clientfalse-claim/"><u>Misinformation Clear: GPT-Win Client—False Claim</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/pioneering-plots-creating-rpgs-in-the-gpt-realm/"><u>Pioneering Plots: Creating RPGs in the GPT Realm</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revolutionizing-communication-post-chatgpt-era/"><u>Revolutionizing Communication: Post-ChatGPT Era</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/say-no-to-gpt-dumbness-openais-rebuttal/"><u>Say No to GPT Dumbness: OpenAI's Rebuttal</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/structured-eating-schemes-inspired-by-gpt/"><u>Structured Eating Schemes Inspired by GPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/stunning-truth-easy-communication-with-ai-gpt/"><u>Stunning Truth: Easy Communication With AI GPT</u></a></li>
<li><a href="https://tech-hub.techidaily.com/top-7-ai-tools-beyond-gpt-for-code-automation/"><u>Top 7 AI Tools Beyond GPT for Code Automation</u></a></li>
<li><a href="https://some-guidance.techidaily.com/top-tracks-for-a-professional-unboxing-presentation-for-2024/"><u>Top Tracks for a Professional Unboxing Presentation for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ubuntu-terminal-tactics-initiating-shellgpt-with-gpt/"><u>Ubuntu Terminal Tactics: Initiating ShellGPT with GPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unleashing-ai-potential-browser-deployment-via-agentgpt/"><u>Unleashing AI Potential: Browser Deployment via AgentGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unlocking-character-potential-with-gpt-and-visionary-ai-tools/"><u>Unlocking Character Potential with GPT and Visionary AI Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unmasking-the-policies-behind-virtual-assistants-censorship/"><u>Unmasking the Policies Behind Virtual Assistants' Censorship</u></a></li>
</ul></div>
