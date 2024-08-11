---
title: "Dialogue Design Dexterity: Constructing Custom AI"
date: 2024-08-10T02:13:30.630Z
updated: 2024-08-11T02:13:30.630Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Dialogue Design Dexterity: Constructing Custom AI"
excerpt: "This Article Describes Dialogue Design Dexterity: Constructing Custom AI"
thumbnail: https://thmb.techidaily.com/41c40fc075ec41a6de89c571a5a74900b640b77fd911558c6dd5abd8173773bf.jpg
---

## Dialogue Design Dexterity: Constructing Custom AI

 Providing GPT technology in a powerful and easy-to-use chatbot, ChatGPT has become the world's most popular AI tool. Many people use ChatGPT to provide engaging conversations, answer queries, offer creative suggestions, and aid in coding and writing. However, ChatGPT is limited as you cannot store your data for long-term personal use, and its September 2021 knowledge data cutoff point.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 As a workaround, we can use OpenAI's API and LangChain to provide ChatGPT with custom data and updated info past 2021 to create a custom ChatGPT instance.

<!-- affiliate ads begin -->
<a href="https://godlikehost.sjv.io/c/5597632/1920054/21774" target="_top" id="1920054"><img src="//a.impactradius-go.com/display-ad/21774-1920054" border="0" alt="" width="320" height="100"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1920054/21774" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Why Provide ChatGPT with Custom Data?

 Feeding ChatGPT with custom data and providing updated information beyond its knowledge cutoff date provides several benefits over just using ChatGPT as usual. Here are a few of them:

* **Personalized Interactions:** By providing ChatGPT with custom data, users can create a more customized experience. The model can be trained on specific datasets relevant to individual users or organizations, resulting in responses tailored to their unique needs and preferences.
* **Domain-Specific Expertise:** Custom data integration allows ChatGPT to specialize in particular domains or industries. It can be trained on industry-specific knowledge, terminology, and trends, enabling more accurate and insightful responses within those specific areas.
* **Current and Accurate Information:** Access to updated information ensures that ChatGPT stays current with the latest developments and knowledge. It can provide accurate responses based on recent events, news, or research, making it a more reliable source of information.

 Now that you understand the importance of providing custom data to ChatGPT, here's a step-by-step on how to do so on your local computer.

<!-- affiliate ads begin -->
<a href="https://store.nero.com/order/checkout.php?PRODS=42296985&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/9cea886b9f44a3c2df1163730ab64994/products/copy_nero_burning_rom_cart.png" border="0">
</a>
<!-- affiliate ads end -->
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

<!-- affiliate ads begin -->
<a href="https://shop.mondly.com/affiliate.php?ACCOUNT=ATISTUDI&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.mondly.com%3FAFFILIATE%3D108875%26RESOURCE%3D%2BBusiness%2B970x90%2B"><img src="https://secure.avangate.com/images/merchant/69c418c33ec2e1a4267fa9bb77fa1428/business-970x90.gif" border="0"></a>
<!-- affiliate ads end -->
![Installing Microsoft C++ through Build Tools](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/2-install-c.jpg)

 Now that you have installed the latest versions of Python3, Git, and Microsoft C++, you can download the Python script to easily query custom local data.

**Download:** [ChatGPT-retrieval script](https://github.com/techleadhd/chatgpt-retrieval) (Free)

 To download the script, click on **Code,** then select **Download ZIP**. This should download the Python script into your default or selected directory.

![Downloading Python script on GitHub](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/3-download-script.jpg)

 Once downloaded, we can now set up a local environment.

## Step 2: Set Up the Local Environment

 To set up the environment, you'll need to open a terminal in the chatgpt-retrieval-main folder you downloaded. To do that, open **chatgpt-retrieval-main** folder, right-click, and select **Open in Terminal**.

<!-- affiliate ads begin -->
<a href="https://purchase.swifdoo.com/order/checkout.php?PRODS=38709260&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/8b932759a5a04ddb34bf79e3f9072e4b/products/Product%20box%20white-1024x1024.png" border="0">SwifDoo PDF Perpetual (2-PC)  Free upgrade. No monthly fees ever. </a>
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
<a href="https://bluetties.sjv.io/c/5597632/2039292/17094" target="_top" id="2039292"><img src="//a.impactradius-go.com/display-ad/17094-2039292" border="0" alt="BLUETTI NEW LAUNCH AC240" width="954" height="1020"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2039292/17094" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![Adding API key as environment variable](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/add-api-key.jpg)

 Now that you have successfully set up your virtual environment and added your OpenAI API key as an environment variable. You can now provide your custom data to ChatGPT.

## Step 3: Adding Custom Data

 To add custom data, place all your custom text data in the **data** folder within chatgpt-retrieval-main. The format of the text data may be in the form of a PDF, TXT, or DOC.

![Adding custom data for ChatGPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/adding-data.jpg)

 As you can see from the screenshot above, I've added a text file containing a made-up personal schedule, an article I wrote on [AMD's Instinct Accelerators](https://www.makeuseof.com/what-are-amd-instinct-ai-accelerators/), and a PDF document.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4530091&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.pearlmountainsoft.com/n_img/product/cit_win/banScrn.jpg" border="0">CollageIt Pro</a>
<!-- affiliate ads end -->
## Step 4: Querying ChatGPT Through Terminal

 The Python script allows us to query data from the custom data we've added to the data folder and the internet. In other words, you will have access to the usual ChatGPT backend and all the data stored locally in the data folder.

 To use the script, run the python [chatgpt.py](http://chatgpt.py) script and then add your question or query as the argument.

python [chatgpt.py](http://chatgpt.py) "YOUR QUESTION"

 Make sure to put your questions in quotation marks.

 To test if we have successfully fed ChatGPT our data, I'll ask a personal question regarding the **Personal Sched.txt** file.

<!-- affiliate ads begin -->
<a href="https://shop.incomedia.eu/order/checkout.php?PRODS=14095146&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.2checkout.com/images/merchant/8b6cc3ee5ec407721ce3bf5ff4c0f56b/PRO_BUY_728x90-EN.jpg" border="0"></a>
<!-- affiliate ads end -->
![Testing ChatGPT with custom data](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/visit.jpg)

 It worked! This means ChatGPT was able to read the Personal Sched.txt provided earlier. Now let's see if we have successfully fed ChatGPT with information it does not know due to its knowledge cutoff date.

![Asking custom ChatGPT about topic outside knowledge cut off data](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/m250x.jpg)

 As you can see, it correctly described the AMD Instinct MI250x, which was released after ChatGPT -3's knowledge cutoff date.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4742929&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/e09fdffe648a30658a9657bbed7b2388/products/boxshot(2).png" border="0">Kanto Player Professional</a>
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
<li><a href="https://fox-hovers.techidaily.com/new-2024-approved-historical-gems-art-unshackled-by-laws/"><u>[New] 2024 Approved  Historical Gems  Art Unshackled by Laws</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-game-changer-review-dji-mavic-air-takes-on-spark/"><u>[New] Game Changer Review  DJI Mavic Air Takes on Spark</u></a></li>
<li><a href="https://twitter-videos.techidaily.com/new-in-2024-tweeting-and-tumbling-sharing-videos-seamlessly/"><u>[New] In 2024, Tweeting & Tumbling  Sharing Videos Seamlessly</u></a></li>
<li><a href="https://twitter-videos.techidaily.com/new-twittickle-your-personalized-toolkit-for-cutest-tweets-for-2024/"><u>[New] TwitTickle  Your Personalized Toolkit for Cutest Tweets for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/10-visionaries-on-the-evolution-of-ai-technology/"><u>10 Visionaries on the Evolution of AI Technology</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/11-best-free-ais-enhancing-email-structure-and-content/"><u>11 Best Free AIs Enhancing Email Structure and Content</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/27-efficient-email-crafting-with-ai-chatgpt-and-summarize/"><u>27 Efficient Email Crafting with AI, ChatGPT & Summarize</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/5-reasons-why-chatgpt-wont-take-your-writing-job/"><u>5 Reasons Why ChatGPT Won’t Take Your Writing Job</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/5-reasons-why-companies-are-banning-chatgpt/"><u>5 Reasons Why Companies Are Banning ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/5-ways-to-control-chatgpt-with-your-voice/"><u>5 Ways to Control ChatGPT With Your Voice</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/6-costless-comparables-to-openais-sora-model/"><u>6 Costless Comparables to OpenAI's Sora Model</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/6-reasons-why-job-seekers-and-workers-should-learn-to-use-chatgpt/"><u>6 Reasons Why Job Seekers and Workers Should Learn to Use ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/7-better-alternatives-to-openais-chatgpt-mobile-app/"><u>7 Better Alternatives to OpenAI's ChatGPT Mobile App</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/7-chrome-tools-for-advanced-ai-interactions/"><u>7 Chrome Tools for Advanced AI Interactions</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/7-game-changing-bard-ai-features-revealed-at-googles-2023-tech-expo/"><u>7 Game-Changing Bard AI Features Revealed at Google's 2023 Tech Expo</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/9-innovative-applications-of-chatgpt-for-wellness/"><u>9 Innovative Applications of ChatGPT for Wellness</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-closer-look-the-8-major-problems-in-chatgpt/"><u>A Closer Look: The 8 Major Problems in ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-dive-into-nvidias-customizable-creativity-engine/"><u>A Dive Into NVIDIA's Customizable Creativity Engine</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-new-era-of-conversational-ai-usechatgpts-co-pilot-extension/"><u>A New Era of Conversational AI: UseChatGPT's Co-Pilot Extension</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-new-era-of-cybercrimes-the-quintupled-impact-of-ai/"><u>A New Era of Cybercrimes: The Quintupled Impact of AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/academic-excellence-through-ai-technology/"><u>Academic Excellence Through AI Technology</u></a></li>
<li><a href="https://win-howtos.techidaily.com/correcting-mistyped-words-strategies-to-improve-keyboard-precision/"><u>Correcting Mistyped Words: Strategies to Improve Keyboard Precision</u></a></li>
<li><a href="https://extra-hints.techidaily.com/crafting-a-unified-brand-presence-on-youtube-for-2024/"><u>Crafting a Unified Brand Presence on YouTube for 2024</u></a></li>
<li><a href="https://games-able.techidaily.com/customize-your-interactive-language-in-steam/"><u>Customize Your Interactive Language in Steam</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721404495179-dive-into-smooth-chatgpt-interactions-chrome-powered-solution/"><u>Dive Into Smooth ChatGPT Interactions - Chrome-Powered Solution!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721390291559-emoji-free-tweet-evolution-linuss-unmasking-trojan-discourse-and-chatgpt-hurdles/"><u>Emoji-Free Tweet Evolution, Linus's Unmasking, Trojan Discourse, & ChatGPT Hurdles</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721409143329-free-gpt-4-for-all-plus-still-provides-an-exclusive-set-of-6-premium-features/"><u>Free GPT-4 for All! Plus Still Provides an Exclusive Set of 6 Premium Features.</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721396161642-gpt-imposters-alert-guard-against-illicit-data-access/"><u>GPT Imposters Alert: Guard Against Illicit Data Access</u></a></li>
<li><a href="https://iphone-unlock.techidaily.com/how-to-unlock-iphone-6s-plus-without-passcode-drfone-by-drfone-ios/"><u>How to Unlock iPhone 6s Plus Without Passcode? | Dr.fone</u></a></li>
<li><a href="https://extra-information.techidaily.com/ideal-matches-mac-and-pc-video-decoders-freepaid/"><u>Ideal Matches  Mac & PC Video Decoders (FREE/PAID)</u></a></li>
<li><a href="https://some-techniques.techidaily.com/in-2024-expert-tips-for-applying-apple-music-to-your-videos/"><u>In 2024, Expert Tips for Applying Apple Music to Your Videos</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/in-2024-network-locked-sim-card-inserted-on-your-oneplus-nord-ce-3-lite-5g-phone-unlock-it-now-by-drfone-android/"><u>In 2024, Network Locked SIM Card Inserted On Your OnePlus Nord CE 3 Lite 5G Phone? Unlock It Now</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721402315595-ios-users-check-this-out-chatgpt-app/"><u>IOS Users, Check This Out: ChatGPT App</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721412760366-iphone-users-reset-your-chatgpt-experience/"><u>IPhone Users, Reset Your ChatGPT Experience</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721430132677-navigate-the-digital-world-easier-bings-new-ai-search-feature-for-phones/"><u>Navigate the Digital World Easier: Bing’s New AI Search Feature for Phones</u></a></li>
<li><a href="https://sound-tweaking.techidaily.com/new-the-newcomers-handbook-including-sound-in-your-imovie-creations/"><u>New The Newcomers Handbook Including Sound in Your iMovie Creations</u></a></li>
<li><a href="https://extra-skills.techidaily.com/seamlessly-integrating-zoom-with-facebook-live-for-2024/"><u>Seamlessly Integrating Zoom with Facebook Live for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721413290822-seize-the-day-with-a-bug-discovery-passport-join-openais-rewarding-adventure/"><u>Seize the Day with a Bug Discovery Passport; Join OpenAI’s Rewarding Adventure</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721433461562-transform-your-mobile-experience-with-bings-smart-search-technology/"><u>Transform Your Mobile Experience with Bing's Smart Search Technology.</u></a></li>
<li><a href="https://audio-shaping.techidaily.com/updated-2024-approved-navigating-video-editing-incorporating-dubbing-techniques-in-filmora/"><u>Updated 2024 Approved Navigating Video Editing Incorporating Dubbing Techniques in Filmora</u></a></li>
</ul></div>
