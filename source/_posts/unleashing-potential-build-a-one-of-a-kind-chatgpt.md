---
title: "Unleashing Potential: Build a One-of-a-Kind ChatGPT"
date: 2024-08-18T09:57:08.979Z
updated: 2024-08-19T09:57:08.979Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Unleashing Potential: Build a One-of-a-Kind ChatGPT"
excerpt: "This Article Describes Unleashing Potential: Build a One-of-a-Kind ChatGPT"
thumbnail: https://thmb.techidaily.com/1e90b427765970b2a66b4df52c7b1587d47d7c547c6bb5f5df0fa9181f11e1b7.jpg
---

## Unleashing Potential: Build a One-of-a-Kind ChatGPT

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
<a href="https://ukaidot.sjv.io/c/5597632/1793233/19578" target="_top" id="1793233"><img src="//a.impactradius-go.com/display-ad/19578-1793233" border="0" alt="" width="1200" height="1200"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1793233/19578" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
### Python3 and Microsoft C++ Installation Notes

 When installing Python3, make sure that you tick the **Add python.exe to PATH** option before clicking **Install Now**. This is important as it allows you to access Python in any directory on your computer.

![Adding Python to PATH](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/1-download-python.jpg)

<!-- affiliate ads begin -->
<a href="https://sentrypc.7eer.net/c/5597632/398457/3022" target="_top" id="398457"><img src="//a.impactradius-go.com/display-ad/3022-398457" border="0" alt="www.sentrypc.com" width="980" height="120"/></a><img height="0" width="0" src="https://sentrypc.7eer.net/i/5597632/398457/3022" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 When Installing Microsoft C++, you'll want to install **Microsoft Visual Studio Build Tools** first. Once installed, you can tick the **Desktop development with C++** option and click **Install** with all the optional tools automatically ticked on the right sidebar.

![Installing Microsoft C++ through Build Tools](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/2-install-c.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4572700&QTY=1&AFFILIATE=108875&CART=1"><img src="	https://www.tubedigger.com/wp-content/uploads/2020/08/tubedigger-software-new.png" border="0">TubeDigger - online video downloader from mostly any site</a>
<!-- affiliate ads end -->
 Now that you have installed the latest versions of Python3, Git, and Microsoft C++, you can download the Python script to easily query custom local data.

**Download:** [ChatGPT-retrieval script](https://github.com/techleadhd/chatgpt-retrieval) (Free)

 To download the script, click on **Code,** then select **Download ZIP**. This should download the Python script into your default or selected directory.

![Downloading Python script on GitHub](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/3-download-script.jpg)

 Once downloaded, we can now set up a local environment.

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

<!-- affiliate ads begin -->
<a href="https://shop.copernic.com/order/checkout.php?PRODS=41033101&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.2checkout.com/images/merchant/8d30aa96e72440759f74bd2306c1fa3d/Copernic-2023-Affiliate-728x90-Elite.png" border="0"></a>
<!-- affiliate ads end -->
 Now that you have successfully set up your virtual environment and added your OpenAI API key as an environment variable. You can now provide your custom data to ChatGPT.

<!-- affiliate ads begin -->
<a href="https://shop.mondly.com/affiliate.php?ACCOUNT=ATISTUDI&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.mondly.com%3FAFFILIATE%3D108875%26RESOURCE%3D%2BEducational%2B300x600%2B"><img src="https://secure.avangate.com/images/merchant/69c418c33ec2e1a4267fa9bb77fa1428/educational-300x600.gif" border="0"></a>
<!-- affiliate ads end -->
## Step 3: Adding Custom Data

 To add custom data, place all your custom text data in the **data** folder within chatgpt-retrieval-main. The format of the text data may be in the form of a PDF, TXT, or DOC.

![Adding custom data for ChatGPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/adding-data.jpg)

<!-- affiliate ads begin -->
<a href="https://ancheer.sjv.io/c/5597632/1657301/17326" target="_top" id="1657301"><img src="//a.impactradius-go.com/display-ad/17326-1657301" border="0" alt="" width="1920" height="933"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1657301/17326" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 As you can see from the screenshot above, I've added a text file containing a made-up personal schedule, an article I wrote on [AMD's Instinct Accelerators](https://www.makeuseof.com/what-are-amd-instinct-ai-accelerators/), and a PDF document.

## Step 4: Querying ChatGPT Through Terminal

 The Python script allows us to query data from the custom data we've added to the data folder and the internet. In other words, you will have access to the usual ChatGPT backend and all the data stored locally in the data folder.

 To use the script, run the python [chatgpt.py](http://chatgpt.py) script and then add your question or query as the argument.

python [chatgpt.py](http://chatgpt.py) "YOUR QUESTION"

 Make sure to put your questions in quotation marks.

 To test if we have successfully fed ChatGPT our data, I'll ask a personal question regarding the **Personal Sched.txt** file.

![Testing ChatGPT with custom data](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/visit.jpg)

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
<li><a href="https://instagram-videos.techidaily.com/new-in-2024-use-of-analytics/"><u>[New] In 2024, Use of Analytics</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/new-narratives-before-night-an-analysis-of-storytelling-videos/"><u>[New] Narratives Before Night  An Analysis of Storytelling Videos</u></a></li>
<li><a href="https://youtube-tips.techidaily.com/ed-2024-approved-the-art-of-keeping-your-audience-attentive-and-committed-top-6-methods-revealed/"><u>[Updated] 2024 Approved  The Art of Keeping Your Audience Attentive & Committed  Top 6 Methods Revealed</u></a></li>
<li><a href="https://facebook-video-share.techidaily.com/updated-a-step-by-step-guide-on-applying-cc-rights-effectively-for-2024/"><u>[Updated] A Step-by-Step Guide on Applying CC Rights Effectively for 2024</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/updated-mastering-video-trailers-on-youtube-via-filmora-tools/"><u>[Updated] Mastering Video Trailers on YouTube via Filmora Tools</u></a></li>
<li><a href="https://location-fake.techidaily.com/10-best-fake-gps-location-spoofers-for-samsung-galaxy-s23-tactical-edition-drfone-by-drfone-virtual-android/"><u>10 Best Fake GPS Location Spoofers for Samsung Galaxy S23 Tactical Edition | Dr.fone</u></a></li>
<li><a href="https://extra-approaches.techidaily.com/2024-approved-insights-into-procuring-freeness-in-frame-vids/"><u>2024 Approved  Insights Into Procuring Freeness in Frame Vids</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-history-in-your-hands-essential-export-tools-reviewed/"><u>AI History in Your Hands – Essential Export Tools Reviewed</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-vs-fortune-tellers-which-shines-light-on-tomorrow/"><u>AI Vs. Fortune-Tellers: Which Shines Light on Tomorrow?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/artificial-intelligence-redefines-work-strategies/"><u>Artificial Intelligence Redefines Work Strategies</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/augmenting-data-analysis-in-excel-through-chatgpt-methods/"><u>Augmenting Data Analysis in Excel Through ChatGPT Methods</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/balancing-benefits-and-drawbacks-chatgpt-in-creativity/"><u>Balancing Benefits & Drawbacks: ChatGPT in Creativity</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/bend-ai-language-to-your-will/"><u>Bend AI Language to Your Will</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/boost-your-workflow-top-8-ai-infused-chrome-plug-ins/"><u>Boost Your Workflow: Top 8 AI-Infused Chrome Plug-Ins</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/breakthrough-ai-by-google-the-dawn-of-bard-challenging-chatgpt/"><u>Breakthrough AI by Google: The Dawn of 'Bard', Challenging ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/bypassing-limits-gpts-hidden-potentials/"><u>Bypassing Limits: GPT's Hidden Potentials</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/charting-the-course-for-safe-ai-ceos-regulatory-plea/"><u>Charting the Course for Safe AI: CEO’s Regulatory Plea</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/conversation-algorithms-ais-way-to-talk-like-us/"><u>Conversation Algorithms: AI's Way to Talk Like Us</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/critical-indicators-when-opting-for-bot-services/"><u>Critical Indicators When Opting for Bot Services</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/demystifying-gpt4alls-complex-processes/"><u>Demystifying GPT4All's Complex Processes</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/discerning-authenticity-in-chatgpt-using-gpt-tags/"><u>Discerning Authenticity in ChatGPT Using GPT Tags</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/elevate-your-chatgpt-now-with-gpt-4-integration/"><u>Elevate Your ChatGPT Now with GPT-4 Integration</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/evaluating-browser-addons-for-secure-gpt-interaction/"><u>Evaluating Browser AddOns for Secure GPT Interaction</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/exploring-the-future-of-ai-with-gpt-4-without-investment/"><u>Exploring the Future of AI with GPT-4 Without Investment</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/gpts-impact-on-legal-aid-explored/"><u>GPT's Impact on Legal Aid Explored</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-use-canva-and-chatgpt-to-bulk-create-content-designs/"><u>How to Use Canva and ChatGPT to Bulk Create Content Designs</u></a></li>
<li><a href="https://fake-location.techidaily.com/in-2024-a-detailed-guide-on-faking-your-location-in-mozilla-firefox-on-oppo-reno-11-pro-5g-drfone-by-drfone-virtual-android/"><u>In 2024, A Detailed Guide on Faking Your Location in Mozilla Firefox On Oppo Reno 11 Pro 5G | Dr.fone</u></a></li>
<li><a href="https://ios-unlock.techidaily.com/in-2024-forgot-locked-apple-iphone-se-2020-password-learn-the-best-methods-to-unlock-by-drfone-ios/"><u>In 2024, Forgot Locked Apple iPhone SE (2020) Password? Learn the Best Methods To Unlock</u></a></li>
<li><a href="https://android-unlock.techidaily.com/in-2024-how-to-unlock-vivo-v29e-phone-pattern-lock-without-factory-reset-by-drfone-android/"><u>In 2024, How to Unlock Vivo V29e Phone Pattern Lock without Factory Reset</u></a></li>
<li><a href="https://extra-support.techidaily.com/in-2024-prime-premiere-pro-blueprints-best-free-2023/"><u>In 2024, Prime Premiere Pro Blueprints - Best Free 2023</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/innovating-proposal-writing-through-ai-with-chatgpt/"><u>Innovating Proposal Writing Through AI with ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/inside-the-mind-of-gpt-the-code-that-powers-dialogue/"><u>Inside the Mind of GPT: The Code That Powers Dialogue</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/intelligence-stands-firm-in-chatgpt-opensai-declares/"><u>Intelligence Stands Firm in ChatGPT, OpensAI Declares</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/invisible-errors-chatgpts-dilemma/"><u>Invisible Errors: ChatGPT's Dilemma</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/is-truthgpt-the-real-deal-or-just-hot-air/"><u>Is TruthGPT The Real Deal or Just Hot Air?</u></a></li>
<li><a href="https://youtube-help.techidaily.com/monetization-timeline-for-successful-youtubers-for-2024/"><u>Monetization Timeline for Successful YouTubers for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/narrative-crafting-via-chatgpt-text-games/"><u>Narrative Crafting via ChatGPT Text Games</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/navigate-with-caution-common-gpt-hoaxes/"><u>Navigate with Caution: Common GPT Hoaxes</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/new-ai-contender-is-gemini-superior-to-chatgpt/"><u>New AI Contender: Is Gemini Superior to ChatGPT?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/next-gen-search-microsoft-upgrades-bing-with-ai-technology/"><u>Next-Gen Search: Microsoft Upgrades Bing with AI Technology</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/optimal-queries-for-ai-driven-crypto-analysis/"><u>Optimal Queries for AI-Driven Crypto Analysis</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/regulating-artificial-intelligence-principles/"><u>Regulating Artificial Intelligence: Principles</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-dichotomy-of-ai-titans-vs-tamer-machines/"><u>The Dichotomy of AI: Titans Vs. Tamer Machines</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/tracing-ais-evolution-through-time-and-space/"><u>Tracing AI's Evolution Through Time and Space</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unleashing-unused-powers-a-guide-to-enhanced-chatgpt-experience/"><u>Unleashing Unused Powers: A Guide to Enhanced ChatGPT Experience</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unlock-travel-dreams-best-7-free-ai-apps-for-spontaneous-trips/"><u>Unlock Travel Dreams: Best 7 Free AI Apps for Spontaneous Trips</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unraveling-ai-chat-expertise-gpt-versus-bings-bot/"><u>Unraveling AI Chat Expertise: GPT versus Bing's Bot</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-real-world-applications-gpts-influence-today/"><u>Unveiling Real-World Applications: GPT's Influence Today</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/x-factors-in-crypto-queries-with-chatgpt/"><u>X-Factors in Crypto Queries with ChatGPT</u></a></li>
</ul></div>
