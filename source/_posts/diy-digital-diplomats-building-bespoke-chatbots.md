---
title: "DIY Digital Diplomats: Building Bespoke ChatBots"
date: 2024-08-15T02:43:43.575Z
updated: 2024-08-16T02:43:43.575Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes DIY Digital Diplomats: Building Bespoke ChatBots"
excerpt: "This Article Describes DIY Digital Diplomats: Building Bespoke ChatBots"
thumbnail: https://thmb.techidaily.com/00b577597c6ed0b7b4c19ecd66f01c2d9945d327028a5bbddef7b8d5f271b960.jpg
---

## DIY Digital Diplomats: Building Bespoke ChatBots

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
<a href="https://versadesk.pxf.io/c/5597632/1892107/21290" target="_top" id="1892107"><img src="//a.impactradius-go.com/display-ad/21290-1892107" border="0" alt="" width="1200" height="628"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1892107/21290" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
### Python3 and Microsoft C++ Installation Notes

 When installing Python3, make sure that you tick the **Add python.exe to PATH** option before clicking **Install Now**. This is important as it allows you to access Python in any directory on your computer.

![Adding Python to PATH](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/1-download-python.jpg)

 When Installing Microsoft C++, you'll want to install **Microsoft Visual Studio Build Tools** first. Once installed, you can tick the **Desktop development with C++** option and click **Install** with all the optional tools automatically ticked on the right sidebar.

![Installing Microsoft C++ through Build Tools](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/2-install-c.jpg)
<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2082532/7443" target="_top" id="2082532"><img src="//a.impactradius-go.com/display-ad/7443-2082532" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2082532/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Now that you have installed the latest versions of Python3, Git, and Microsoft C++, you can download the Python script to easily query custom local data.

**Download:** [ChatGPT-retrieval script](https://github.com/techleadhd/chatgpt-retrieval) (Free)

 To download the script, click on **Code,** then select **Download ZIP**. This should download the Python script into your default or selected directory.

![Downloading Python script on GitHub](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/3-download-script.jpg)

 Once downloaded, we can now set up a local environment.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4665597&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.pcclean.io/wp-content/uploads/2018/03/winutilities-box-130521.png" border="0">WinUtilities Pro</a>
<!-- affiliate ads end -->
## Step 2: Set Up the Local Environment

 To set up the environment, you'll need to open a terminal in the chatgpt-retrieval-main folder you downloaded. To do that, open **chatgpt-retrieval-main** folder, right-click, and select **Open in Terminal**.

![Opening terminal on directory folder](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/4-open-terminal.jpg)
<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4531356&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/8fdd149fcaa7058caccc9c4ad5b0d89a/products/tss-box.JPG" border="0">The Tube Sites Submitter is a fast and efficient tool for anyone who needs to upload videos quickly, easily and automatically to hundreds of tube sites in mere minutes . </a>
<!-- affiliate ads end -->

 Once the terminal is open, copy and paste this command:

pip install langchain openai chromadb tiktoken unstructured

 This command uses Python's package manager to [create and manage the Python virtual environment](https://www.makeuseof.com/create-manage-python-virtual-environments/) needed.

 After creating the virtual environment, we need to supply an OpenAI API key to access their services. We'll first need to generate an API key from the [OpenAI API keys site](https://platform.openai.com/account/api-keys) by clicking on **Create new secret key**, adding a name for the key, then hitting the **Create secret key button**.

![Creating secret API key](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/generate-api-key.jpg)

 You will be provided with a string of characters. This is your OpenAI API key. Copy it by clicking on the copy icon on the side of the API key. Keep note that this API key should be kept secret. Do not share it with others unless you really intend for them to use it with you.

 Once copied, return to the chatgpt-retrieval-main folder and open constants with **Notepad**. Now replace the placeholder with your API key. Remember to save the file!

![Adding API key as environment variable](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/add-api-key.jpg)
<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=37701530&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/6fe0c81e3f9438db11ebbfba6c5ce460/products/copy_cbLogo_with_text_blue.png" border="0">CalendarBudget - Monthly subscription membership to CalendarBudget via web browser or mobile app. Support included. </a>
<!-- affiliate ads end -->

 Now that you have successfully set up your virtual environment and added your OpenAI API key as an environment variable. You can now provide your custom data to ChatGPT.

<!-- affiliate ads begin -->
<a href="https://store.massmailsoftware.com/order/checkout.php?PRODS=1047974&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/dc87c13749315c7217cdc4ac692e704c/banera_for_partners-04_%281%29.jpg" border="0"></a>
<!-- affiliate ads end -->
## Step 3: Adding Custom Data

 To add custom data, place all your custom text data in the **data** folder within chatgpt-retrieval-main. The format of the text data may be in the form of a PDF, TXT, or DOC.

![Adding custom data for ChatGPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/adding-data.jpg)
<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=37100474&QTY=1&AFFILIATE=108875&CART=1"><img src="https://awario.com/images/pages/index/img-platform-ui-1280@1x.avif" border="0"></a>
<!-- affiliate ads end -->

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
<!-- affiliate ads begin -->
<a href="https://godlikehost.sjv.io/c/5597632/1920054/21774" target="_top" id="1920054"><img src="//a.impactradius-go.com/display-ad/21774-1920054" border="0" alt="" width="320" height="100"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1920054/21774" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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
<li><a href="https://twitter-videos.techidaily.com/new-2024-approved-disseminate-your-tiktok-on-twitter-effectively/"><u>[New] 2024 Approved  Disseminate Your TikTok on Twitter Effectively</u></a></li>
<li><a href="https://facebook-video-share.techidaily.com/new-2024-approved-engage-and-captivate-viewers-ultimate-tips-for-cutting-edge-youtube-edits/"><u>[New] 2024 Approved  Engage and Captivate Viewers  Ultimate Tips for Cutting-Edge Youtube Edits</u></a></li>
<li><a href="https://extra-hints.techidaily.com/new-circling-the-globe-in-one-shot-versus-layered-visuals/"><u>[New] Circling the Globe in One Shot Versus Layered Visuals</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/new-global-reach-12-video-live-stream-app/"><u>[New] Global Reach  12 Video Live Stream App</u></a></li>
<li><a href="https://instagram-video-files.techidaily.com/new-instagram-insights-how-to-make-your-videos-a-hit/"><u>[New] Instagram Insights  How to Make Your Videos a Hit</u></a></li>
<li><a href="https://article-helps.techidaily.com/new-navigating-picture-in-picture-mode-with-confidence-using-microsoft-edge/"><u>[New] Navigating Picture-In-Picture Mode with Confidence Using Microsoft Edge</u></a></li>
<li><a href="https://facebook-videos.techidaily.com/updated-facebook-live-the-world-in-minutes/"><u>[Updated] Facebook Live  The World in Minutes</u></a></li>
<li><a href="https://fox-info.techidaily.com/updated-unveiling-windows-11-a-compreayer-to-master-video-editing-techniques-for-2024/"><u>[Updated] Unveiling Windows 11  A Compreayer to Master Video Editing Techniques for 2024</u></a></li>
<li><a href="https://facebook-video-recording.techidaily.com/2024-approved-improve-youtube-viewing-of-fb-videos-on-android/"><u>2024 Approved  Improve YouTube Viewing of FB Videos on Android</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/advanced-techniques-to-silence-background-noise-in-media/"><u>Advanced Techniques to Silence Background Noise in Media</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/are-gpt-enhanced-jobs-the-next-big-income-boost/"><u>Are GPT-Enhanced Jobs the Next Big Income Boost?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/boosting-language-skills-through-chatgpt-premium/"><u>Boosting Language Skills Through ChatGPT Premium</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/breaking-down-claude-2-features-unveiled/"><u>Breaking Down Claude 2: Features Unveiled</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/compare-and-conquer-why-ios-chatgpt-wins-over-web/"><u>Compare & Conquer: Why iOS ChatGPT Wins Over Web</u></a></li>
<li><a href="https://tiktok-videos.techidaily.com/copyright-clarity-how-to-verify-video-rights-pre-upload/"><u>Copyright Clarity  How to Verify Video Rights Pre-Upload</u></a></li>
<li><a href="https://tech-recovery.techidaily.com/discover-our-picks-top-12-free-voice-over-ip-voip-calls-apps-of-2024/"><u>Discover Our Picks: Top 12 Free Voice over IP (VoIP) Calls Apps of 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/diving-into-digital-dialogue-googles-groundbreayer-palm-2/"><u>Diving Into Digital Dialogue: Google's Groundbreayer, PaLM 2</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/does-ai-like-chatgpt-have-wordcharacter-count-boundaries/"><u>Does AI, Like ChatGPT, Have Word/Character Count Boundaries?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/efficiently-navigate-away-from-dead-end-gpt-tools/"><u>Efficiently Navigate Away From Dead-End GPT Tools</u></a></li>
<li><a href="https://video-screen-grab.techidaily.com/enhancing-teamimage-blurring-backgrounds-on-microsoft-teams/"><u>Enhancing TeamImage  Blurring Backgrounds on Microsoft Teams</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/from-digital-dialogue-to-printed-poetry-collections/"><u>From Digital Dialogue to Printed Poetry Collections</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/gamifying-language-text-based-quests-via-chatgpt/"><u>Gamifying Language: Text-Based Quests via ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/googles-gemini-navigating-through-its-artificial-intelligence-landscape/"><u>Google’s Gemini: Navigating Through Its Artificial Intelligence Landscape</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-correct-chatgpt-live-dialogue-problems/"><u>How To Correct ChatGPT Live Dialogue Problems</u></a></li>
<li><a href="https://fix-guide.techidaily.com/how-to-fix-unresponsive-phone-touchscreen-of-poco-x6-pro-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>How To Fix Unresponsive Phone Touchscreen Of Poco X6 Pro | Dr.fone</u></a></li>
<li><a href="https://change-location.techidaily.com/how-to-use-snapchat-location-spoofer-to-protect-your-privacy-on-apple-iphone-13-drfone-by-drfone-virtual-ios/"><u>How to use Snapchat Location Spoofer to Protect Your Privacy On Apple iPhone 13? | Dr.fone</u></a></li>
<li><a href="https://extra-lessons.techidaily.com/in-2024-3dr-alone-unpackaging-a-single-user-review/"><u>In 2024, '3DR' Alone  Unpackaging a Single User Review</u></a></li>
<li><a href="https://android-location.techidaily.com/in-2024-10-fake-gps-location-apps-on-android-of-your-honor-90-drfone-by-drfone-virtual/"><u>In 2024, 10 Fake GPS Location Apps on Android Of your Honor 90 | Dr.fone</u></a></li>
<li><a href="https://apple-account.techidaily.com/in-2024-your-account-has-been-disabled-in-the-app-store-and-itunes-from-iphone-x-by-drfone-ios/"><u>In 2024, Your Account Has Been Disabled in the App Store and iTunes From iPhone X?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/innovative-excel-solutions-achieved-via-chatgpt-use-cases/"><u>Innovative Excel Solutions Achieved via ChatGPT Use Cases</u></a></li>
<li><a href="https://program-issues.techidaily.com/jurassic-world-evolution-stability-solutions-overcoming-game-crash-issues/"><u>Jurassic World Evolution Stability Solutions: Overcoming Game Crash Issues</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-chatgpt-plugin-integration/"><u>Mastering ChatGPT Plugin Integration</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/musks-mystery-the-future-of-gpt-revealed/"><u>Musk's Mystery: The Future of GPT Revealed?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/navigating-chatgpt-for-kids-five-child-friendly-practices/"><u>Navigating ChatGPT for Kids: Five Child-Friendly Practices</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/navigating-technological-speak-29-key-ai-concepts/"><u>Navigating Technological Speak: 29 Key AI Concepts</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/navigating-the-complexities-of-ai-made-messages/"><u>Navigating the Complexities of AI-Made Messages</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/new-era-of-conversation-chatgpt-on-ios/"><u>New Era of Conversation: ChatGPT on iOS</u></a></li>
<li><a href="https://vp-tips.techidaily.com/no-fuss-full-fun-exploring-ifunnys-meme-treasure/"><u>No Fuss, Full Fun  Exploring iFunny's Meme Treasure</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/openais-linguistic-titans-understanding-gpt-14/"><u>OpenAI’s Linguistic Titans: Understanding GPT-1–4</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/overcoming-gpts-text-limit-tips-and-tricks/"><u>Overcoming GPT's Text Limit – Tips & Tricks!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revolutionizing-creation-ten-advances-by-ai/"><u>Revolutionizing Creation: Ten Advances by AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/seek-these-six-no-cost-ai-options-similar-to-sora/"><u>Seek These Six No-Cost AI Options Similar to Sora</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/simplify-complexity-transformative-techniques-for-3d-printing-with-chatgpt/"><u>Simplify Complexity: Transformative Techniques for 3D Printing with ChatGPT</u></a></li>
<li><a href="https://win-howtos.techidaily.com/step-by-step-guide-restoring-your-windows-pcs-built-in-webcam-functionality/"><u>Step-by-Step Guide: Restoring Your Windows PC's Built-In Webcam Functionality</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/strategies-for-employing-chatgpt-in-study-papers/"><u>Strategies for Employing ChatGPT in Study Papers</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/strategies-for-exporting-data-from-your-ai-conversations/"><u>Strategies for Exporting Data From Your AI Conversations</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/tailored-transformation-crafting-a-personalized-chatgpt/"><u>Tailored Transformation: Crafting a Personalized ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/tailoring-ai-communication-implementing-gpt-creation/"><u>Tailoring AI Communication: Implementing GPT Creation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-chat-comparison-coin-how-gpt-stacks-up-against-bingbot/"><u>The Chat Comparison Coin: How GPT Stacks Up Against BingBot</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-quest-for-excellence-between-gemini-max-and-enhanced-chatgpt/"><u>The Quest for Excellence: Between Gemini Max & Enhanced ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-truth-behind-grok-ai-insights-from-musk-on-its-purpose-and-price/"><u>The Truth Behind Grok AI - Insights From Musk on Its Purpose & Price</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-ultimate-list-of-ai-powered-chrome-extensions-for-better-task-management/"><u>The Ultimate List of AI-Powered Chrome Extensions for Better Task Management</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-unreliable-shield-of-artificative-intelligence/"><u>The Unreliable Shield of Artificative Intelligence</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/top-copywriting-hurdles-how-to-easily-avoid-with-chatgpts-help/"><u>Top Copywriting Hurdles: How to Easily Avoid With ChatGPT's Help</u></a></li>
<li><a href="https://extra-lessons.techidaily.com/top-vr-bikes-to-check-out/"><u>Top VR Bikes to Check Out</u></a></li>
<li><a href="https://bypass-frp.techidaily.com/ultimate-guide-on-samsung-galaxy-a15-5g-frp-bypass-by-drfone-android/"><u>Ultimate Guide on Samsung Galaxy A15 5G FRP Bypass</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unraveling-chatgpt-premiums-worth/"><u>Unraveling ChatGPT Premium's Worth</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-the-shortcomings-of-ai-powered-message-bots/"><u>Unveiling the Shortcomings of AI-Powered Message Bots</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/warning-avoid-suspicious-win-chatgpt-software/"><u>Warning: Avoid Suspicious Win ChatGPT Software</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/why-human-authors-outperform-ai-driven-writing-assistants/"><u>Why Human Authors Outperform AI-Driven Writing Assistants</u></a></li>
</ul></div>
