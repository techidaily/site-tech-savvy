---
title: "Tailored Transformation: Crafting a Personalized ChatGPT"
date: 2024-08-10T02:04:34.450Z
updated: 2024-08-11T02:04:34.450Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Tailored Transformation: Crafting a Personalized ChatGPT"
excerpt: "This Article Describes Tailored Transformation: Crafting a Personalized ChatGPT"
thumbnail: https://thmb.techidaily.com/d8d6563b1e83446e0eb6eee844ba3f9b3df6929eaff9c17a0488818cf8023092.jpg
---

## Tailored Transformation: Crafting a Personalized ChatGPT

 Providing GPT technology in a powerful and easy-to-use chatbot, ChatGPT has become the world's most popular AI tool. Many people use ChatGPT to provide engaging conversations, answer queries, offer creative suggestions, and aid in coding and writing. However, ChatGPT is limited as you cannot store your data for long-term personal use, and its September 2021 knowledge data cutoff point.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 As a workaround, we can use OpenAI's API and LangChain to provide ChatGPT with custom data and updated info past 2021 to create a custom ChatGPT instance.

<!-- affiliate ads begin -->
<a href="https://shop.manycam.com/order/checkout.php?PRODS=17727588&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/8230bea7d54bcdf99cdfe85cb07313d5/mcaffbanner600x500.png" border="0"></a>
<a href="https://shop.manycam.com/order/checkout.php?PRODS=17727588&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/8230bea7d54bcdf99cdfe85cb07313d5/Affiliates_300x250px_valentinesday.png" border="0"></a>
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

<!-- affiliate ads begin -->
<a href="https://ephamedtechinc.pxf.io/c/5597632/2097466/26400?prodsku=B700" target="_top" id="2097466"><img src="//a.impactradius-go.com/display-ad/26400-2097466" border="0" alt="" width="2048" height="1024"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2097466/26400" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
### Python3 and Microsoft C++ Installation Notes

 When installing Python3, make sure that you tick the **Add python.exe to PATH** option before clicking **Install Now**. This is important as it allows you to access Python in any directory on your computer.

![Adding Python to PATH](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/1-download-python.jpg)

 When Installing Microsoft C++, you'll want to install **Microsoft Visual Studio Build Tools** first. Once installed, you can tick the **Desktop development with C++** option and click **Install** with all the optional tools automatically ticked on the right sidebar.

<!-- affiliate ads begin -->
<a href="https://printrendy.pxf.io/c/5597632/1453721/17020" target="_top" id="1453721"><img src="//a.impactradius-go.com/display-ad/17020-1453721" border="0" alt="" width="300" height="250"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1453721/17020" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![Installing Microsoft C++ through Build Tools](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/2-install-c.jpg)

 Now that you have installed the latest versions of Python3, Git, and Microsoft C++, you can download the Python script to easily query custom local data.

**Download:** [ChatGPT-retrieval script](https://github.com/techleadhd/chatgpt-retrieval) (Free)

 To download the script, click on **Code,** then select **Download ZIP**. This should download the Python script into your default or selected directory.

![Downloading Python script on GitHub](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/3-download-script.jpg)

 Once downloaded, we can now set up a local environment.

<!-- affiliate ads begin -->
<a href="https://shop.incomedia.eu/order/checkout.php?PRODS=39655089&QTY=1&AFFILIATE=108875&CART=1"><img src="https://incomedia.eu/files/images/affiliates/wa/01_WA_728x90.jpg" border="0"></a>
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

<!-- affiliate ads begin -->
<a href="https://25home.pxf.io/c/5597632/2090698/16836" target="_top" id="2090698"><img src="//a.impactradius-go.com/display-ad/16836-2090698" border="0" alt="" width="720" height="300"/></a>
<!-- affiliate ads end -->
## Step 4: Querying ChatGPT Through Terminal

 The Python script allows us to query data from the custom data we've added to the data folder and the internet. In other words, you will have access to the usual ChatGPT backend and all the data stored locally in the data folder.

 To use the script, run the python [chatgpt.py](http://chatgpt.py) script and then add your question or query as the argument.

python [chatgpt.py](http://chatgpt.py) "YOUR QUESTION"

 Make sure to put your questions in quotation marks.

 To test if we have successfully fed ChatGPT our data, I'll ask a personal question regarding the **Personal Sched.txt** file.

<!-- affiliate ads begin -->
<a href="https://otszone.ots7.com/order/checkout.php?PRODS=4713324&QTY=1&AFFILIATE=108875&CART=1"><img src="https://green.ots7.com/screenshots/OtsAV/OtsAVTV1.90-300x188.jpg" border="0">OtsAV TV Webcaster</a>
<!-- affiliate ads end -->
![Testing ChatGPT with custom data](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/visit.jpg)

 It worked! This means ChatGPT was able to read the Personal Sched.txt provided earlier. Now let's see if we have successfully fed ChatGPT with information it does not know due to its knowledge cutoff date.

<!-- affiliate ads begin -->
<a href="https://shop.incomedia.eu/order/checkout.php?PRODS=12730965&QTY=1&AFFILIATE=108875&CART=1"><img src="https://incomedia.eu/files/images/affiliates/w5/03_WBSX5_728x90_red_CTA.jpg" border="0"></a>
<!-- affiliate ads end -->
![Asking custom ChatGPT about topic outside knowledge cut off data](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/m250x.jpg)

 As you can see, it correctly described the AMD Instinct MI250x, which was released after ChatGPT -3's knowledge cutoff date.

<!-- affiliate ads begin -->
<a href="https://shop.emeditor.com/order/checkout.php?PRODS=4610657&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.emeditor.com/wp-content/uploads/2024/06/emeditor_chat_ai.png" border="0">
EmEditor is a fast, lightweight, yet extensible, easy-to-use text editor, code editor, CSV editor, and large file viewer for Windows. Both native 64-bit and 32-bit builds are available, and moreover, the 64-bit includes separate builds for SSE2 (128-bit), AVX-2 (256-bit), and AVX-512 (512-bit) instruction sets. New versions support AI-assisted writing.</a>
<!-- affiliate ads end -->
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
<li><a href="https://facebook-record-videos.techidaily.com/new-2024-approved-boosting-exposure-posting-youtube-content-on-facebook-effectively/"><u>[New] 2024 Approved  Boosting Exposure  Posting YouTube Content on Facebook Effectively</u></a></li>
<li><a href="https://some-approaches.techidaily.com/new-ten-best-practices-for-meme-creation/"><u>[New] Ten Best Practices for Meme Creation</u></a></li>
<li><a href="https://fox-links.techidaily.com/updated-best-photo-and-video-display-apps-from-xi-to-x/"><u>[Updated] Best Photo & Video Display Apps  From XI to X</u></a></li>
<li><a href="https://digital-screen-recording.techidaily.com/updated-in-2024-in-depth-training-adopting-the-best-screen-recording-practices-with-adobe-captivate/"><u>[Updated] In 2024, In-Depth Training  Adopting the Best Screen Recording Practices with Adobe Captivate</u></a></li>
<li><a href="https://twitter-videos.techidaily.com/updated-in-2024-the-meme-titans-reddit-and-twitters-biggest-sensations/"><u>[Updated] In 2024, The Meme Titans  Reddit & Twitter's Biggest Sensations</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/10-ways-chatgpt-could-help-you-land-a-job-on-linkedin/"><u>10 Ways ChatGPT Could Help You Land a Job on LinkedIn</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/18-next-level-sales-management-applications-beyond-gpts-realm/"><u>18 Next-Level Sales Management Applications Beyond GPT's Realm</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/2024-approved-independent-filming-freedoms-agreement/"><u>2024 Approved  Independent Filming Freedoms Agreement</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/26-cutting-edge-solutions-to-replace-chatgpts-pos-software/"><u>26 Cutting-Edge Solutions to Replace ChatGPT's POS Software</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/4-ways-ai-transforms-scholarly-work/"><u>4 Ways AI Transforms Scholarly Work</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/4-ways-the-claude-ai-chatbot-is-better-than-chatgpt/"><u>4 Ways the Claude AI Chatbot Is Better Than ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/4-point-ai-assessment-kit-gauging-chatgpts-teaching-potency/"><u>4-Point AI Assessment Kit: Gauging ChatGPT's Teaching Potency</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/5-accessible-high-quality-ai-art-systems/"><u>5 Accessible, High-Quality AI Art Systems</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/5-creative-utilizations-of-chatbots-like-gpt/"><u>5 Creative Utilizations of ChatBots Like GPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/5-proven-techniques-to-elevate-your-chatgpt-experience/"><u>5 Proven Techniques to Elevate Your ChatGPT Experience</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/5-reasons-you-cannot-use-chatgpt-for-crypto-analysis/"><u>5 Reasons You Cannot Use ChatGPT for Crypto Analysis</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/5-reasons-excluding-gpt-from-cryptographic-research/"><u>5 Reasons: Excluding GPT From Cryptographic Research</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/5-vital-avenues-how-ai-strengthens-illegal-cyberspace-operations/"><u>5 Vital Avenues: How AI Strengthens Illegal Cyberspace Operations</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/6-cautionary-tales-of-reliance-on-artificial-brains/"><u>6 Cautionary Tales of Reliance on Artificial Brains</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/6-chatgpt-apps-to-analyze-and-chat-with-your-documents-and-pdfs/"><u>6 ChatGPT Apps to Analyze and Chat With Your Documents and PDFs</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/6-innovative-ways-to-utilize-chatgpt-for-job-seekers-and-workers/"><u>6 Innovative Ways to Utilize ChatGPT for Job Seekers & Workers</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/6-openai-sora-alternatives-you-can-try-for-free/"><u>6 OpenAI Sora Alternatives You Can Try for Free</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/6-strong-reasons-ios-app-superiority-in-gpt-domain/"><u>6 Strong Reasons: IOS App Superiority in GPT Domain</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/7-cybersecurity-trends-and-predictions/"><u>7 Cybersecurity Trends and Predictions</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-clash-of-bots-is-gpt-plus-superior-to-perplexity/"><u>A Clash of Bots: Is GPT Plus Superior to Perplexity?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-compreenasive-look-at-the-progression-of-openais-models/"><u>A Compreenasive Look at the Progression of OpenAI's Models</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-developers-guide-top-10-chatgpt-enhancements-in-vs-code/"><u>A Developer's Guide: Top 10 ChatGPT Enhancements in VS Code</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-look-at-ai-threats-chatgpts-potential-for-financial-heists/"><u>A Look at AI Threats: ChatGPT’s Potential for Financial Heists</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-peek-into-hugging-faces-workings-and-uses/"><u>A Peek Into Hugging Face’s Workings and Uses</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-step-by-step-guide-to-structuring-chatgpt-conversations/"><u>A Step-by-Step Guide to Structuring ChatGPT Conversations</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721403320790-awaken-your-smartphone-with-chatgpt/"><u>Awaken Your Smartphone with ChatGPT</u></a></li>
<li><a href="https://extra-tips.techidaily.com/free-online-tools-perfect-your-beats-like-a-pro-dj/"><u>Free Online Tools  Perfect Your Beats Like a Pro DJ</u></a></li>
<li><a href="https://some-techniques.techidaily.com/ifunny-meme-seamless-download-and-enjoyment-for-2024/"><u>IFunny Meme  Seamless Download and Enjoyment for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721408721327-intuitive-talking-to-ai-try-this-chrome-tool/"><u>Intuitive Talking to AI? Try This Chrome Tool!</u></a></li>
<li><a href="https://some-approaches.techidaily.com/leveraging-zoom-for-high-quality-facebook-live-streams-for-2024/"><u>Leveraging Zoom for High-Quality Facebook LIVE Streams for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721392425670-navigate-the-web-with-ease-bings-ai-search-on-ios-and-android/"><u>Navigate the Web with Ease: Bing's AI Search on iOS & Android</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721391750232-revolutionary-chatgpt-tweaks-youll-love/"><u>Revolutionary ChatGPT Tweaks You'll Love</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721373940749-seamless-ai-powered-bing-search-across-ios-and-android/"><u>Seamless AI-Powered Bing Search Across iOS and Android</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721407461364-supercharge-gpt-4-for-nothing-more-than-a-friendly-helper-enter-copilot/"><u>Supercharge GPT-4 for Nothing More Than a Friendly Helper - Enter Copilot</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721411226505-terminate-chatgpt-connection-now/"><u>Terminate ChatGPT Connection Now!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721424969962-twitters-without-symbols-linuss-exposed-content-trojans-demystified-and-gpt-errors-spotlighted/"><u>Twitters Without Symbols, Linus’s Exposed Content, Trojans Demystified, & GPT Errors Spotlighted.</u></a></li>
<li><a href="https://meme-emoji.techidaily.com/updated-how-to-make-a-photo-collage-on-maciphone-using-iphoto-in-2024/"><u>Updated How to Make a Photo Collage on Mac/iPhone Using iPhoto, In 2024</u></a></li>
</ul></div>
