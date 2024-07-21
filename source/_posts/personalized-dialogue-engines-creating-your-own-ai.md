---
title: "Personalized Dialogue Engines: Creating Your Own AI"
date: 2024-07-20T06:23:09.670Z
updated: 2024-07-21T06:23:09.670Z
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
<li><a href="https://vp-tips.techidaily.com/new-2024-approved-igniting-laughter-a-path-to-meme-fame/"><u>[New] 2024 Approved  Igniting Laughter  A Path to Meme Fame</u></a></li>
<li><a href="https://facebook-clips.techidaily.com/new-in-2024-unraveling-image-mysteries-the-triple-tactic-fb-backward-search/"><u>[New] In 2024, Unraveling Image Mysteries  The Triple-Tactic FB Backward Search</u></a></li>
<li><a href="https://screen-capture.techidaily.com/new-video-recording-titans-obs-studio-vs-fraps-face-off-for-2024/"><u>[New] Video Recording Titans  OBS Studio vs Fraps Face-Off for 2024</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/updated-2024-approved-broadcasting-conferences-with-no-expense-account/"><u>[Updated] 2024 Approved  Broadcasting Conferences with No Expense Account</u></a></li>
<li><a href="https://twitter-videos.techidaily.com/updated-2024-approved-twitch-and-prime-whos-watching-the-show-2023-edition/"><u>[Updated] 2024 Approved  Twitch and Prime  Who’s Watching the Show? 2023 Edition</u></a></li>
<li><a href="https://fox-helps.techidaily.com/updated-crafting-gentle-sound-declines-with-logic-pro-for-2024/"><u>[Updated] Crafting Gentle Sound Declines with Logic Pro for 2024</u></a></li>
<li><a href="https://facebook-videos.techidaily.com/updated-enhance-social-media-reach-on-facebook-using-proven-seo-methods-for-2024/"><u>[Updated] Enhance Social Media Reach on Facebook Using Proven SEO Methods for 2024</u></a></li>
<li><a href="https://fox-links.techidaily.com/updated-in-2024-detailed-examination-panorama-lens-revolution-by-samsung/"><u>[Updated] In 2024, Detailed Examination  Panorama Lens Revolution by Samsung</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/updated-in-2024-streamlined-methods-for-iphone-screen-recordings/"><u>[Updated] In 2024, Streamlined Methods for iPhone Screen Recordings</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/updated-in-2024-superior-hd-gameplay-through-top-captures/"><u>[Updated] In 2024, Superior HD Gameplay Through Top Captures</u></a></li>
<li><a href="https://extra-skills.techidaily.com/updated-leading-vision-capture-camera-hits-of-2024/"><u>[Updated] Leading Vision Capture  Camera Hits of 2024</u></a></li>
<li><a href="https://some-skills.techidaily.com/updated-top-10-ever-approved-reddit-threads-a-historical-list/"><u>[Updated] Top 10 Ever-Approved Reddit Threads  A Historical List</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/15-best-strongest-pokemon-to-use-in-pokemon-go-pvp-leagues-for-samsung-galaxy-a05-drfone-by-drfone-virtual-android/"><u>15 Best Strongest Pokémon To Use in Pokémon GO PvP Leagues For Samsung Galaxy A05 | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-conversation-kings-deciphering-top-generative-bot/"><u>AI Conversation Kings: Deciphering Top Generative Bot</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/auto-gpts-effectiveness-independent-or-not/"><u>Auto-GPT's Effectiveness: Independent or Not?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/barricade-website-from-robotic-data-collectors/"><u>Barricade Website From Robotic Data Collectors</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpts-impact-on-modern-day-job-seekers/"><u>ChatGPT's Impact on Modern-Day Job Seekers</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/clarifying-nlp-and-machine-learning-distinctions/"><u>Clarifying NLP & Machine Learning Distinctions</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/crafting-your-path-to-fitness-ai-assisted-strategy/"><u>Crafting Your Path to Fitness: AI-Assisted Strategy</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/creative-catalysts-da-vincis-triumph-in-image-generation-ai/"><u>Creative Catalysts: Da Vinci’s Triumph in Image Generation AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/cutting-edge-job-search-with-chatgpt-insights/"><u>Cutting-Edge Job Search with ChatGPT Insights</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/dodging-fraudsters-a-guide-to-genuine-vs-bogus-bingcoin-offers/"><u>Dodging Fraudsters: A Guide to Genuine vs Bogus BingCoin Offers</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/elevating-ai-writing-making-chatgpt-write-like-you/"><u>Elevating AI Writing: Making ChatGPT Write Like You</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/elevating-chatgpt-the-introduction-of-vocal-responses-to-commands/"><u>Elevating ChatGPT: The Introduction of Vocal Responses to Commands</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/envisioning-a-new-era-for-microsoft-bing-through-ai/"><u>Envisioning a New Era for Microsoft Bing Through AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/establish-a-home-friendly-low-cost-windows-simulation/"><u>Establish a Home-Friendly, Low-Cost Windows Simulation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/exploring-career-trajectories-in-ai-driven-responsiveness-design/"><u>Exploring Career Trajectories in AI-Driven Responsiveness Design</u></a></li>
<li><a href="https://techidaily.com/factory-reset-apple-iphone-12-pro-max-drfone-by-drfone-ios-system-repair-ios-system-repair/"><u>Factory Reset Apple iPhone 12 Pro Max | Dr.fone</u></a></li>
<li><a href="https://iphone-transfer.techidaily.com/fix-apple-iphone-15-pro-max-stuck-on-data-transfer-verified-solution-drfone-by-drfone-transfer-from-ios/"><u>Fix Apple iPhone 15 Pro Max Stuck on Data Transfer Verified Solution! | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721405554846-free-gpt-4-for-everyone-nonetheless-select-plus-membership-continues-to-provide-unique-services/"><u>Free GPT-4 for Everyone; Nonetheless, Select Plus Membership Continues to Provide Unique Services.</u></a></li>
<li><a href="https://change-location.techidaily.com/how-can-i-catch-the-regional-pokemon-without-traveling-on-samsung-galaxy-xcover-6-pro-tactical-edition-drfone-by-drfone-virtual-android/"><u>How Can I Catch the Regional Pokémon without Traveling On Samsung Galaxy XCover 6 Pro Tactical Edition | Dr.fone</u></a></li>
<li><a href="https://facebook-clips.techidaily.com/in-2024-becoming-a-trendsetter-viral-tactics-for-fb/"><u>In 2024, Becoming a Trendsetter  Viral Tactics for FB</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/in-2024-reasons-why-pokemon-gps-does-not-work-on-sony-xperia-10-v-drfone-by-drfone-virtual-android/"><u>In 2024, Reasons why Pokémon GPS does not Work On Sony Xperia 10 V? | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/insight-chatgpts-default-tools-explained/"><u>Insight: ChatGPT's Default Tools Explained</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/leap-into-advanced-chatgpt-top-9-essential-plugins-here/"><u>Leap Into Advanced ChatGPT – Top 9 Essential Plugins Here</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/leveraging-ai-for-compelling-youtube-thumbnails/"><u>Leveraging AI for Compelling YouTube Thumbnails</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/leveraging-ai-for-poetic-excellence-the-chatgpt-method/"><u>Leveraging AI for Poetic Excellence: The ChatGPT Method</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/machine-talk-deciphering-the-gpt-bing-divide/"><u>Machine Talk: Deciphering the GPT-Bing Divide</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/maximizing-creativity-with-chatgpts-advanced-image-recognition/"><u>Maximizing Creativity with ChatGPT's Advanced Image Recognition</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/missed-malware-alert-say-no-to-google-bard-download/"><u>Missed Malware Alert: Say No to Google Bard Download</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/navigating-the-nuances-of-chatgptenticing-api-use/"><u>Navigating the Nuances of ChatGPT'enticing API Use</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/opt-for-basic-textual-chatgpt-or-enhanced-web-integrated-version/"><u>Opt for Basic Textual ChatGPT or Enhanced Web-Integrated Version</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/pioneering-tech-advancements-the-six-sweepstakes-of-gpts-conductor/"><u>Pioneering Tech Advancements - The Six Sweepstakes of GPT's Conductor</u></a></li>
<li><a href="https://techidaily.com/the-easiest-methods-to-hard-reset-htc-u23-drfone-by-drfone-reset-android-reset-android/"><u>The Easiest Methods to Hard Reset HTC U23 | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-journey-through-generative-ais-evolution/"><u>The Journey Through Generative AI's Evolution</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-language-model-arena-gpt-vs-bert-explained/"><u>The Language Model Arena: GPT Vs. BERT Explained</u></a></li>
<li><a href="https://some-skills.techidaily.com/transform-your-laptop-with-these-8-stylish-skins-for-2024/"><u>Transform Your Laptop with These 8 Stylish Skins for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unraveling-gpt-self-driven-tech-distinct-from-chatgpts-model/"><u>Unraveling GPT Self-Driven Tech: Distinct From ChatGPT’s Model</u></a></li>
<li><a href="https://voice-adjusting.techidaily.com/updated-decoding-the-criteria-for-optimal-audio-post-production-professionals-for-2024/"><u>Updated Decoding The Criteria for Optimal Audio Post-Production Professionals for 2024</u></a></li>
<li><a href="https://video-ai-editor.techidaily.com/updated-from-shaky-to-smooth-adobe-premiere-pro-video-stabilization-tutorial/"><u>Updated From Shaky to Smooth Adobe Premiere Pro Video Stabilization Tutorial</u></a></li>
</ul></div>
