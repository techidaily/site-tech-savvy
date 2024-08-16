---
title: Designing Your Unique GPT Model From Scratch
date: 2024-08-15T02:35:35.260Z
updated: 2024-08-16T02:35:35.260Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Designing Your Unique GPT Model From Scratch
excerpt: This Article Describes Designing Your Unique GPT Model From Scratch
thumbnail: https://thmb.techidaily.com/eb0b88fc8ea01a6f57ac593062a230bcd4f411a04c405e68f58f5857acd450ec.jpg
---

## Designing Your Unique GPT Model From Scratch

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
<a href="https://secure.textstudio.com/order/checkout.php?PRODS=35633309&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/d6eb8222c9718486bdabce8b897380f7/products/3_premium-icon.png" border="0"> Take advantage of PREMIUM features for 12 months. 
Create your texts / logos without any limitation. 
No attribution required when downloading. 
No advertising on the website. 
 TextStudio.com  PREMIUM - Yearly Membership</a>
<!-- affiliate ads end -->
### Python3 and Microsoft C++ Installation Notes

 When installing Python3, make sure that you tick the **Add python.exe to PATH** option before clicking **Install Now**. This is important as it allows you to access Python in any directory on your computer.

![Adding Python to PATH](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/1-download-python.jpg)
<!-- affiliate ads begin -->
<a href="https://propmoneyinc.pxf.io/c/5597632/1803116/14559" target="_top" id="1803116"><img src="//a.impactradius-go.com/display-ad/14559-1803116" border="0" alt="" width="859" height="859"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1803116/14559" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 When Installing Microsoft C++, you'll want to install **Microsoft Visual Studio Build Tools** first. Once installed, you can tick the **Desktop development with C++** option and click **Install** with all the optional tools automatically ticked on the right sidebar.

![Installing Microsoft C++ through Build Tools](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/2-install-c.jpg)

 Now that you have installed the latest versions of Python3, Git, and Microsoft C++, you can download the Python script to easily query custom local data.

**Download:** [ChatGPT-retrieval script](https://github.com/techleadhd/chatgpt-retrieval) (Free)

 To download the script, click on **Code,** then select **Download ZIP**. This should download the Python script into your default or selected directory.

![Downloading Python script on GitHub](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/3-download-script.jpg)

 Once downloaded, we can now set up a local environment.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4718730&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/ce9a6fb2becc2d235e62b125e9260102/products/copy_vMixCallScreenshot1-large.jpg" border="0">vMix HD - Software based live production. vMix HD includes everything in vMix Basic HD plus 1000 inputs, Video List, 4 Overlay Channels, and 1 vMix Call 
This bundle includes Studio 200 for vMix from Virtualsetworks, HTTP Matrix 1.0 automation scheduler, and 4 introductory training videos from the Udemy vMix Basic to Amazing course. </a>
<!-- affiliate ads end -->
## Step 2: Set Up the Local Environment

 To set up the environment, you'll need to open a terminal in the chatgpt-retrieval-main folder you downloaded. To do that, open **chatgpt-retrieval-main** folder, right-click, and select **Open in Terminal**.

![Opening terminal on directory folder](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/4-open-terminal.jpg)

 Once the terminal is open, copy and paste this command:

pip install langchain openai chromadb tiktoken unstructured

 This command uses Python's package manager to [create and manage the Python virtual environment](https://www.makeuseof.com/create-manage-python-virtual-environments/) needed.

 After creating the virtual environment, we need to supply an OpenAI API key to access their services. We'll first need to generate an API key from the [OpenAI API keys site](https://platform.openai.com/account/api-keys) by clicking on **Create new secret key**, adding a name for the key, then hitting the **Create secret key button**.

![Creating secret API key](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/generate-api-key.jpg)
<!-- affiliate ads begin -->
<a href="https://store.nero.com/order/checkout.php?PRODS=42296985&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/9cea886b9f44a3c2df1163730ab64994/products/copy_nero_burning_rom_cart.png" border="0">
</a>
<!-- affiliate ads end -->

 You will be provided with a string of characters. This is your OpenAI API key. Copy it by clicking on the copy icon on the side of the API key. Keep note that this API key should be kept secret. Do not share it with others unless you really intend for them to use it with you.

 Once copied, return to the chatgpt-retrieval-main folder and open constants with **Notepad**. Now replace the placeholder with your API key. Remember to save the file!

![Adding API key as environment variable](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/add-api-key.jpg)

 Now that you have successfully set up your virtual environment and added your OpenAI API key as an environment variable. You can now provide your custom data to ChatGPT.

<!-- affiliate ads begin -->
<a href="https://checkout.abbyy.com/order/checkout.php?PRODS=39254762&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/0e5fb5c76fca16adbee503c9aff393cd/products/11_FR-Badges-NEW-FR-Standard-16-WIN-200.png" border="0"> PDF application, powered by AI-based OCR, for unified workflows with both digital and scanned documents. </a>
<!-- affiliate ads end -->
## Step 3: Adding Custom Data

 To add custom data, place all your custom text data in the **data** folder within chatgpt-retrieval-main. The format of the text data may be in the form of a PDF, TXT, or DOC.

![Adding custom data for ChatGPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/adding-data.jpg)
<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=32667153&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.coolmuster.com/uploads/image/20201228/feature02.png" border="0"></a>
<!-- affiliate ads end -->

 As you can see from the screenshot above, I've added a text file containing a made-up personal schedule, an article I wrote on [AMD's Instinct Accelerators](https://www.makeuseof.com/what-are-amd-instinct-ai-accelerators/), and a PDF document.

<!-- affiliate ads begin -->
<a href="https://modlily.sjv.io/c/5597632/1997817/17059" target="_top" id="1997817"><img src="//a.impactradius-go.com/display-ad/17059-1997817" border="0" alt="" width="300" height="250"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1997817/17059" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
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

## Limitations of Custom ChatGPT

 Although feeding GPT-3.5 with custom data opens more ways to apply and use the LLM, there are a few drawbacks and limitations.

 Firstly, you need to provide all the data yourself. You can still access all the knowledge of GPT-3.5 until its knowledge cutoff date; however, you must provide all the extra data. This means if you want your local model to be knowledgeable of a certain subject on the internet that GPT-3.5 don't already know, you'll have to go to the internet and scrape the data yourself and save it as a text on the data folder of chatgpt-retrieval-main.

 Another issue is that querying ChatGPT like this takes more time to load when compared to asking ChatGPT directly.

 Lastly, the only model currently available is GPT-3.5 Turbo. So even if you have access to GPT-4, you won't be able to use it to power your custom ChatGPT instance.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4615471&QTY=1&AFFILIATE=108875&CART=1"><img src="https://images.wondershare.com/affiliate-image/affiliate_banners_en/max_782x90.png" border="0"></a>
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
<li><a href="https://instagram-clips.techidaily.com/new-innovative-approaches-adding-borders-to-your-instagram-content/"><u>[New] Innovative Approaches  Adding Borders to Your Instagram Content</u></a></li>
<li><a href="https://vp-tips.techidaily.com/new-off-facebook-activity-analysis-and-secure-browsing-practices/"><u>[New] Off-Facebook Activity Analysis & Secure Browsing Practices</u></a></li>
<li><a href="https://facebook-videos.techidaily.com/new-revealed-the-best-videos-from-facebooks-pages-for-2024/"><u>[New] Revealed  The Best Videos From Facebook’s Pages for 2024</u></a></li>
<li><a href="https://fox-boxes.techidaily.com/updated-ultimate-free-stopwatches-without-a-price-tag-for-2024/"><u>[Updated] Ultimate Free Stopwatches Without a Price Tag for 2024</u></a></li>
<li><a href="https://some-skills.techidaily.com/2024-approved-the-2019-evolution-of-vegaspro/"><u>2024 Approved  The 2019 Evolution of VegasPro</u></a></li>
<li><a href="https://location-fake.techidaily.com/5-hassle-free-solutions-to-fake-location-on-find-my-friends-of-honor-90-pro-drfone-by-drfone-virtual-android/"><u>5 Hassle-Free Solutions to Fake Location on Find My Friends Of Honor 90 Pro | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-evolution-from-tools-to-smart-assistants/"><u>AI Evolution: From Tools to Smart Assistants</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-assisted-content-chatgpts-creative-edge/"><u>AI-Assisted Content: ChatGPT's Creative Edge</u></a></li>
<li><a href="https://youtube-zero.techidaily.com/10-echo-augmentation-apps-desktopmobile-for-2024/"><u>Best 10 Echo Augmentation Apps  Desktop/Mobile for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/bridging-human-and-machine-in-academic-research/"><u>Bridging Human and Machine in Academic Research</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-in-excel-conquer-your-data-fears/"><u>ChatGPT in Excel: Conquer Your Data Fears</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-enhancing-vs-complicating-creative-endeavors/"><u>ChatGPT: Enhancing vs Complicating Creative Endeavors</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/content-authenticity-human-vs-machine-craftsmanship/"><u>Content Authenticity: Human vs Machine Craftsmanship</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/conversational-ai-the-new-era-of-interactive-communication/"><u>Conversational AI: The New Era of Interactive Communication</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/crafting-digital-worlds-6-chatgpt-based-techniques-for-video-games/"><u>Crafting Digital Worlds: 6 ChatGPT-Based Techniques for Video Games</u></a></li>
<li><a href="https://mondly-stories.techidaily.com/decoding-the-belgian-tongue-conundrum/"><u>Decoding the Belgian Tongue Conundrum</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/employment-mastery-made-possible-by-smart-ai-tech/"><u>Employment Mastery Made Possible by Smart AI Tech</u></a></li>
<li><a href="https://win11-tips.techidaily.com/enhancing-the-visibility-of-search-outcomes-in-windows-1011/"><u>Enhancing the Visibility of Search Outcomes in Windows 10/11</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/essays-in-the-digital-age-is-ai-overruling-student-effort/"><u>Essays in the Digital Age: Is AI Overruling Student Effort?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/examining-chatgpts-truthfulness-claims/"><u>Examining ChatGPT's Truthfulness Claims</u></a></li>
<li><a href="https://screen-sharing-recording.techidaily.com/farm-frenzy-fun-pack-the-ultimate-agritainment-guide-for-2024/"><u>Farm Frenzy Fun-Pack  The Ultimate Agritainment Guide for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/from-ideas-to-impressions-writing-with-ais-insight/"><u>From Ideas to Impressions: Writing with AI's Insight</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/getting-to-the-frontier-of-ai-with-gpt-4-for-free/"><u>Getting to the Frontier of AI with GPT-4 for Free</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/gpt-2-guidelines-sidestep-mistakes-quickly/"><u>GPT-2 Guidelines: Sidestep Mistakes Quickly</u></a></li>
<li><a href="https://fake-location.techidaily.com/how-can-i-use-a-fake-gps-without-mock-location-on-honor-play-7t-drfone-by-drfone-virtual-android/"><u>How Can I Use a Fake GPS Without Mock Location On Honor Play 7T? | Dr.fone</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/how-do-i-add-my-signature-to-wpt-file-by-ldigisigner-sign-a-word-sign-a-word/"><u>How do i add my signature to .wpt file</u></a></li>
<li><a href="https://fake-location.techidaily.com/how-to-sharefake-gps-on-uber-for-vivo-y100-5g-drfone-by-drfone-virtual-android/"><u>How to share/fake gps on Uber for Vivo Y100 5G | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-use-quoras-poe-to-access-ai-chatbots-and-llms/"><u>How to Use Quora's Poe to Access AI Chatbots and LLMs</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ideal-chatgpt-query-templates-from-githubs-best-list/"><u>Ideal ChatGPT Query Templates From GitHub's Best List</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/impacting-development-the-ai-revolution/"><u>Impacting Development: The AI Revolution</u></a></li>
<li><a href="https://extra-hints.techidaily.com/in-2024-chortlechaos-dive-deep-into-meme-genesis/"><u>In 2024, ChortleChaos  Dive Deep Into Meme Genesis</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/in-2024-comprehensive-ultimate-guide-to-instagram-stories/"><u>In 2024, Comprehensive Ultimate Guide to Instagram Stories</u></a></li>
<li><a href="https://unlock-android.techidaily.com/in-2024-full-guide-to-unlock-your-xiaomi-redmi-12-5g-by-drfone-android/"><u>In 2024, Full Guide to Unlock Your Xiaomi Redmi 12 5G</u></a></li>
<li><a href="https://some-approaches.techidaily.com/in-2024-the-complete-beginners-manual-to-using-final-cut-pro/"><u>In 2024, The Complete Beginner's Manual to Using Final Cut Pro</u></a></li>
<li><a href="https://youtube-help.techidaily.com/in-2024-ultimate-a-list-viewing-channel-guide-for-films/"><u>In 2024, Ultimate A-List Viewing  Channel Guide for Films</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/innovative-plot-development-with-chatgpts-nine-insights/"><u>Innovative Plot Development with ChatGPT's Nine Insights</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/introduce-a-budget-friendly-gpt-local-instance-on-windows/"><u>Introduce a Budget-Friendly GPT Local Instance on Windows</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/leveraging-ai-written-layers-four-tips-to-read-pdfs-via-chatgpt/"><u>Leveraging AI' Written Layers: Four Tips to Read PDFs via ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/maximizing-connection-utilizing-chatgpt-for-social-engagement/"><u>Maximizing Connection: Utilizing ChatGPT for Social Engagement</u></a></li>
<li><a href="https://facebook-video-recording.techidaily.com/mend-iphones-facebook-video-displays/"><u>Mend iPhones' Facebook Video Displays</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/navigating-new-web-capabilities-in-gpt-3s-beta-update/"><u>Navigating New Web Capabilities in GPT-3's Beta Update</u></a></li>
<li><a href="https://voice-adjusting.techidaily.com/new-how-to-remove-audio-seamlessly-a-windows-10-users-handbook-for-sound-free-vids-free-of-charge-for-2024/"><u>New How to Remove Audio Seamlessly A Windows 10 Users Handbook for Sound-Free Vids (Free of Charge) for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/next-gen-ai-methods-elevating-web-search-standards/"><u>Next-Gen AI Methods Elevating Web Search Standards</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/nightshades-arsenal-to-outmaneuver-generative-ai-copycats/"><u>Nightshade's Arsenal to Outmaneuver Generative AI Copycats</u></a></li>
<li><a href="https://tech-recovery.techidaily.com/photoshop-overflow-problem-fixing-scratch-disk-full-with-simple-tricks/"><u>Photoshop Overflow Problem? Fixing 'Scratch Disk Full' With Simple Tricks</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/pseudo-agent-program-snaffles-facebook-sign-ins/"><u>Pseudo-Agent Program: Snaffles Facebook Sign-Ins</u></a></li>
<li><a href="https://techidaily.com/remove-google-frp-lock-on-xiaomi-redmi-note-13-proplus-5g-by-drfone-android-unlock-remove-google-frp/"><u>Remove Google FRP lock on Xiaomi Redmi Note 13 Pro+ 5G</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/retain-gpt-conversations-easily/"><u>Retain GPT Conversations Easily</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revolutionize-writing-the-leading-5-ai-inspirational-tools/"><u>Revolutionize Writing: The Leading 5 AI Inspirational Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/semantic-showdown-chatgpt-versus-googles-accuracy/"><u>Semantic Showdown: ChatGPT Versus Google's Accuracy</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/streamline-conversations-the-chatgpt-folder-methodology/"><u>Streamline Conversations: The ChatGPT Folder Methodology</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-hidden-perils-of-ai-penned-literature/"><u>The Hidden Perils of AI-Penned Literature</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-missing-self-editing-feature-in-gpt/"><u>The Missing Self-Editing Feature in GPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-new-frontier-are-ai-systems-ready-for-a-change/"><u>The New Frontier: Are AI Systems Ready for a Change?</u></a></li>
<li><a href="https://audio-editing.techidaily.com/the-premier-list-smartphone-applications-that-revolutionize-vocal-identity-for-2024/"><u>The Premier List Smartphone Applications That Revolutionize Vocal Identity for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-quintessential-guide-to-writing-powerful-chatgpt-prompts/"><u>The Quintessential Guide to Writing Powerful ChatGPT Prompts</u></a></li>
<li><a href="https://howto.techidaily.com/top-10-fixes-for-phone-keep-disconnecting-from-wi-fi-on-xiaomi-redmi-12-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>Top 10 Fixes for Phone Keep Disconnecting from Wi-Fi On Xiaomi Redmi 12 | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/top-6-mods-elevating-your-interaction-with-chatgpt-and-vs-code/"><u>Top 6 Mods: Elevating Your Interaction with ChatGPT & VS Code</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/top-6-reasons-ios-outshines-chatgpt-website/"><u>Top 6 Reasons: IOS Outshines ChatGPT Website</u></a></li>
<li><a href="https://win-blog.techidaily.com/unblocking-web-pages-on-chrome-solutions-for-smooth-online-navigation/"><u>Unblocking Web Pages on Chrome - Solutions for Smooth Online Navigation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unlock-career-potentials-with-these-6-reasons-to-learn-chatgpt/"><u>Unlock Career Potentials with These 6 Reasons to Learn ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unraveling-the-paperclip-predicament-ties-to-ai/"><u>Unraveling the Paperclip Predicament: Ties to AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/why-human-touch-matters-in-therapy-more-than-computerized-care/"><u>Why Human Touch Matters in Therapy, More Than Computerized Care</u></a></li>
</ul></div>
