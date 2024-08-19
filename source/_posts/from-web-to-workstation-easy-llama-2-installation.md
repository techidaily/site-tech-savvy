---
title: "From Web to Workstation: Easy Llama 2 Installation"
date: 2024-08-18T10:00:29.579Z
updated: 2024-08-19T10:00:29.579Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes From Web to Workstation: Easy Llama 2 Installation"
excerpt: "This Article Describes From Web to Workstation: Easy Llama 2 Installation"
thumbnail: https://thmb.techidaily.com/9ed4d2a342c503dc1182b48b6f97e1914eb836100fe0df4621fadbbe35959f4b.jpg
---

## From Web to Workstation: Easy Llama 2 Installation

 Meta released Llama 2 in the summer of 2023\. The new version of Llama is fine-tuned with 40% more tokens than the original Llama model, doubling its context length and significantly outperforming other open-sourced models available. The fastest and easiest way to access Llama 2 is via an API through an online platform. However, if you want the best experience, installing and loading Llama 2 directly on your computer is best.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 With that in mind, we've created a step-by-step guide on how to use Text-Generation-WebUI to load a quantized Llama 2 LLM locally on your computer.

## Why Install Llama 2 Locally

 There are many reasons why people choose to run Llama 2 directly. Some do it for privacy concerns, some for customization, and others for offline capabilities. If you're researching, fine-tuning, or integrating Llama 2 for your projects, then accessing Llama 2 via API might not be for you. The point of running an LLM locally on your PC is to reduce reliance on [third-party AI tools](https://www.makeuseof.com/best-ai-web-apps/) and use AI anytime, anywhere, without worrying about leaking potentially sensitive data to companies and other organizations.

 With that said, let's begin with the step-by-step guide to installing Llama 2 locally.

## Step 1: Install Visual Studio 2019 Build Tool

 To simplify things, we will use a one-click installer for Text-Generation-WebUI (the program used to load Llama 2 with GUI). However, for this installer to work, you need to download the Visual Studio 2019 Build Tool and install the necessary resources.

**Download:**[Visual Studio 2019](https://learn.microsoft.com/en-us/visualstudio/releases/2019/release-notes) (Free)

1. Go ahead and download the community edition of the software.
2. Now install Visual Studio 2019, then open the software. Once opened, tick the box on **Desktop development with C++** and hit install.  
![Install-Desktop-Development-With-C++](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/2-install-desktop-development-with-c.jpg)

 Now that you have Desktop development with C++ installed, it's time to download the Text-Generation-WebUI one-click installer.

<!-- affiliate ads begin -->
<a href="https://mindmanager.sjv.io/c/5597632/1787667/20231" target="_top" id="1787667"><img src="//a.impactradius-go.com/display-ad/20231-1787667" border="0" alt="" width="728" height="90"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1787667/20231" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Step 2: Install Text-Generation-WebUI

 The Text-Generation-WebUI one-click installer is a script that automatically creates the required folders and sets up the Conda environment and all necessary requirements to run an AI model.

 To install the script, download the one-click installer by clicking on **Code** \> **Download ZIP.**

**Download:**[Text-Generation-WebUI Installer](https://github.com/oobabooga/text-generation-webui/tree/main) (Free)

1. Once downloaded, extract the ZIP file to your preferred location, then open the extracted folder.
2. Within the folder, scroll down and look for the appropriate start program for your operating system. Run the programs by double-clicking the appropriate script.  
   * If you are on Windows, select **start\_windows** batch file  
   * for MacOS, select **start\_macos** shell scrip  
   * for Linux, **start\_linux** shell script.  
   ![Select operating system](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/4-select-operating-system.jpg)
3. Your anti-virus might create an alert; this is fine. The prompt is just an [antivirus false positive](https://www.makeuseof.com/what-is-antivirus-false-result/) for running a batch file or script. Click on **Run anyway**.
4. A terminal will open and start the setup. Early on, the setup will pause and ask you what GPU you are using. Select the appropriate type of GPU installed on your computer and hit enter. For those without a dedicated graphics card, select **None (I want to run models in CPU mode)**. Keep in mind that running on CPU mode is much slower when compared to running the model with a dedicated GPU.  
![Selecting GPU hardware installed](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/5-select-gpu-settings.jpg)
5. Once the setup is complete, you can now launch Text-Generation-WebUI locally. You can do so by opening your preferred web browser and entering the provided IP address on the URL.  
![How to launch-Text-Generation-WebUI](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/6-launch-text-generation-webui.jpg)
6. The WebUI is now ready for use.  
![Text-Generation-WebUI](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/7-text-generation-webui-view.jpg)

 However, the program is only a model loader. Let's download Llama 2 for the model loader to launch.

<!-- affiliate ads begin -->
<a href="https://ukaidot.sjv.io/c/5597632/1793237/19578" target="_top" id="1793237"><img src="//a.impactradius-go.com/display-ad/19578-1793237" border="0" alt="" width="1200" height="1200"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1793237/19578" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Step 3: Download the Llama 2 Model

 There are quite a few things to consider when deciding which iteration of Llama 2 you need. These include parameters, quantization, hardware optimization, size, and usage. All of this information will be found denoted in the model's name.

* **Parameters:** The number of parameters used to train the model. Bigger parameters make more capable models but at the cost of performance.
* **Usage:** Can either be standard or chat. A chat model is optimized to be used as a chatbot like ChatGPT, while the standard is the default model.
* **Hardware Optimization:** Refers to what hardware best runs the model. GPTQ means the model is optimized to run on a dedicated GPU, while GGML is optimized to run on a CPU.
* **Quantization:** Denotes the precision of weights and activations in a model. For inferencing, a precision of q4 is optimal.
* **Size:** Refers to the size of the specific model.

 Note that some models may be arranged differently and may not even have the same types of information displayed. However, this type of naming convention is fairly common in the [HuggingFace](https://www.makeuseof.com/what-is-hugging-face-and-what-is-it-used-for/) Model library, so it's still worth understanding.

![HuggingFace model naming convention](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/wm/2023/10/huggingface-model-naming-convention-1.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4631056&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/997e65474a248252883b485717f7d098/products/buy-windows.png" border="0">Allavsoft Batch Download Online Videos, Music Offline to MP4, MP3, MOV, etc format </a>
<!-- affiliate ads end -->
 In this example, the model can be identified as a medium-sized Llama 2 model trained on 13 billion parameters optimized for chat inferencing using a dedicated CPU.

 For those running on a dedicated GPU, choose a **GPTQ** model, while for those using a CPU, choose **GGML**. If you want to chat with the model like you would with ChatGPT, choose **chat**, but if you want to experiment with the model with its full capabilities, use the **standard** model. As for parameters, know that using bigger models will provide better results at the expense of performance. I would personally recommend you start with a 7B model. As for quantization, use q4, as it's only for inferencing.

**Download:**[GGML](https://huggingface.co/localmodels/Llama-2-7B-ggml/tree/main) (Free)

**Download:**[GPTQ](https://huggingface.co/localmodels/Llama-2-7B-Chat-GPTQ/tree/main) (Free)

 Now that you know what iteration of Llama 2 you need, go ahead and download the model you want.

 In my case, since I'm running this on an ultrabook, I'll be using a GGML model fine-tuned for chat, **llama-2-7b-chat-ggmlv3.q4\_K\_S.bin.**

![Downloading Llama 2 model of your preference](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/8-download-llama-2-model.jpg)

 After the download is finished, place the model in **text-generation-webui-main** \> **models**.

![Placing Llama 2 model to model folder](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/9-place-model-to-model-folder.jpg)

Now that you have your model downloaded and placed in the model folder, it's time to configure the model loader.

## Step 4: Configure Text-Generation-WebUI

 Now, let's begin the configuration phase.

1. Once again, open Text-Generation-WebUI by running the **start\_(your OS)** file (see the previous steps above).
2. On the tabs located above the GUI, click **Model.** Click the refresh button at the model dropdown menu and select your model.
3. Now click on the dropdown menu of the **Model loader** and select **AutoGPTQ** for those using a GTPQ model and **ctransformers** for those using a GGML model. Finally, click on **Load** to load your model.  
![Setting model loader](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/10-select-model-loader.jpg)
4. To use the model, open the Chat tab and start testing the model.  
<!-- affiliate ads begin -->
<a href="https://coinrule.sjv.io/c/5597632/1958374/18409" target="_top" id="1958374"><img src="//a.impactradius-go.com/display-ad/18409-1958374" border="0" alt="" width="300" height="300"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1958374/18409" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![Testing Llama 2 locally](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/12-testing-llama-2-locally.jpg)

<!-- affiliate ads begin -->
<a href="https://printrendy.pxf.io/c/5597632/1453720/17020" target="_top" id="1453720"><img src="//a.impactradius-go.com/display-ad/17020-1453720" border="0" alt="" width="300" height="250"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1453720/17020" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 Congratulations, you've successfully loaded Llama2 on your local computer!

<!-- affiliate ads begin -->
<a href="https://shop.mondly.com/affiliate.php?ACCOUNT=ATISTUDI&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.mondly.com%3FAFFILIATE%3D108875%26RESOURCE%3D%2BGeneral%2B970x90%2B"><img src="https://secure.avangate.com/images/merchant/69c418c33ec2e1a4267fa9bb77fa1428/general-970x90.gif" border="0"></a>
<!-- affiliate ads end -->
## Try Out Other LLMs

 Now that you know how to run Llama 2 directly on your computer using Text-Generation-WebUI, you should also be able to run other LLMs besides Llama. Just remember the naming conventions of models and that only quantized versions of models (usually q4 precision) can be loaded on regular PCs. Many quantized LLMs are available on HuggingFace. If you want to explore other models, search for TheBloke in HuggingFace's model library, and you should find many models available.

**SCROLL TO CONTINUE WITH CONTENT**

 With that in mind, we've created a step-by-step guide on how to use Text-Generation-WebUI to load a quantized Llama 2 LLM locally on your computer.

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
<li><a href="https://instagram-clips.techidaily.com/new-discover-the-best-instagram-video-editors-for-mobile-devices/"><u>[New] Discover the Best Instagram Video Editors for Mobile Devices</u></a></li>
<li><a href="https://facebook-video-recording.techidaily.com/updated-2024-approved-hitting-your-targets-with-these-8-social-media-planners/"><u>[Updated] 2024 Approved  Hitting Your Targets with These 8 Social Media Planners</u></a></li>
<li><a href="https://fox-hovers.techidaily.com/updated-in-2024-iphone-hacks-for-minimalist-video-presentation/"><u>[Updated] In 2024, IPhone Hacks for Minimalist Video Presentation</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/2024-approved-navigating-free-art-online-a-guide-and-top-sites/"><u>2024 Approved  Navigating Free Art Online  A Guide & Top Sites</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-in-action-boosting-crypto-returns-via-chatgpt/"><u>AI in Action: Boosting Crypto Returns via ChatGPT</u></a></li>
<li><a href="https://fox-that.techidaily.com/airpods-troubleshooting-guide-fix-no-sound-problem-in-just-9-simple-methods/"><u>AirPods Troubleshooting Guide: Fix No Sound Problem in Just 9 Simple Methods</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/analyzing-security-in-browser-ai-plugins/"><u>Analyzing Security in Browser AI Plugins</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/androids-new-wave-of-conversation-with-chatgpt/"><u>Android's New Wave of Conversation – With ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/battling-bother-ais-role-in-relaxation/"><u>Battling Bother: AI's Role in Relaxation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-unlocks-wearable-potential-with-six-pioneering-capabilities/"><u>ChatGPT Unlocks Wearable Potential with Six Pioneering Capabilities</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/computational-math-chatgpts-role/"><u>Computational Math: ChatGPT’s Role</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/crafting-successful-fitness-goals-through-gpt/"><u>Crafting Successful Fitness Goals Through GPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/crafting-tales-leveraging-chatgpt-for-epic-narratives/"><u>Crafting Tales: Leveraging ChatGPT for Epic Narratives</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ethical-guidelines-utilizing-chatgpt-for-wellness/"><u>Ethical Guidelines: Utilizing ChatGPT for Wellness</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/examining-the-safety-of-ais-like-chatgpt/"><u>Examining the Safety of AI's Like ChatGPT</u></a></li>
<li><a href="https://win-answers.techidaily.com/1722993198084-fixes-for-origin-not-working-get-back-online-now/"><u>Fixes for Origin Not Working - Get Back Online Now!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/free-voyage-vision-pinpoint-your-dream-trip-with-top-7-ai-tools/"><u>Free Voyage Vision: Pinpoint Your Dream Trip with Top 7 AI Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-ai-ignores-its-syntax-slips/"><u>How AI Ignores Its Syntax Slips</u></a></li>
<li><a href="https://change-location.techidaily.com/how-to-use-life360-on-windows-pc-for-tecno-spark-10c-drfone-by-drfone-virtual-android/"><u>How to Use Life360 on Windows PC For Tecno Spark 10C? | Dr.fone</u></a></li>
<li><a href="https://android-frp.techidaily.com/in-2024-hassle-free-ways-to-remove-frp-lock-on-meizuwithwithout-a-pc-by-drfone-android/"><u>In 2024, Hassle-Free Ways to Remove FRP Lock on Meizuwith/without a PC</u></a></li>
<li><a href="https://ios-unlock.techidaily.com/in-2024-how-to-bypass-iphone-14-pro-max-passcode-easily-video-inside-by-drfone-ios/"><u>In 2024, How to Bypass iPhone 14 Pro Max Passcode Easily Video Inside</u></a></li>
<li><a href="https://android-location-track.techidaily.com/in-2024-top-10-telegram-spy-tools-on-samsung-galaxy-s23-fe-for-parents-drfone-by-drfone-virtual-android/"><u>In 2024, Top 10 Telegram Spy Tools On Samsung Galaxy S23 FE for Parents | Dr.fone</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/in-2024-windows-11-excellent-video-capture-tools-compared/"><u>In 2024, Windows 11  Excellent Video Capture Tools Compared</u></a></li>
<li><a href="https://change-location.techidaily.com/list-of-pokemon-go-joysticks-on-vivo-v30-lite-5g-drfone-by-drfone-virtual-android/"><u>List of Pokémon Go Joysticks On Vivo V30 Lite 5G | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/outperform-googlee-search-unleash-perplexity-ai/"><u>Outperform Google’e Search - Unleash Perplexity AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/pause-comparing-siri-and-chatgpt-key-differences-explored/"><u>Pause Comparing Siri & ChatGPT: Key Differences Explored</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/recognizing-fraudulent-chatgpt-websites-prevention-and-response-measures/"><u>Recognizing Fraudulent ChatGPT Websites: Prevention and Response Measures</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/shield-your-digital-domain-stop-bot-harvesters/"><u>Shield Your Digital Domain: Stop Bot Harvesters</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/sources-scrutinized-chatgpts-originality-assessment/"><u>Sources Scrutinized: ChatGPT’s Originality Assessment</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/step-up-your-gaming-skills-with-chatgpts-coolest-games/"><u>Step Up Your Gaming Skills With ChatGPT's Coolest Games</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-hidden-dangers-of-trusting-ai-blindly/"><u>The Hidden Dangers of Trusting AI Blindly</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-ultimate-list-10-alternatives-to-chatgpt/"><u>The Ultimate List: 10 Alternatives to ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/token-evolution-gemini-unveils-million-context-shift/"><u>Token Evolution: Gemini Unveils Million Context Shift</u></a></li>
<li><a href="https://extra-lessons.techidaily.com/top-platforms-for-amplifying-youtube-content/"><u>Top Platforms for Amplifying YouTube Content</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unlocking-dungeon-mastery-chatgpts-role-in-epic-fantasy-games/"><u>Unlocking Dungeon Mastery: ChatGPT's Role in Epic Fantasy Games</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-7-apps-with-gpt-4-functionality-insights/"><u>Unveiling 7 Apps with GPT-4: Functionality Insights</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-ai-potential-in-domestic-task-planning/"><u>Unveiling AI Potential in Domestic Task Planning</u></a></li>
<li><a href="https://ai-topics.techidaily.com/updated-what-is-ai-text-to-video-in-2024/"><u>Updated What Is AI Text to Video, In 2024</u></a></li>
</ul></div>
