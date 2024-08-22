---
title: "From Online to Offline: Installed Llama 2 Basics"
date: 2024-08-21T15:42:04.273Z
updated: 2024-08-22T15:42:04.273Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes From Online to Offline: Installed Llama 2 Basics"
excerpt: "This Article Describes From Online to Offline: Installed Llama 2 Basics"
thumbnail: https://thmb.techidaily.com/c96841199ff180b06a551ff8b5da580eafb5a9f0013849780e2ea631a72bda1d.jpg
---

## From Online to Offline: Installed Llama 2 Basics

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
<a href="https://shop.mondly.com/affiliate.php?ACCOUNT=ATISTUDI&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.mondly.com%3FAFFILIATE%3D108875%26RESOURCE%3D%2BGeneral%2B970x90%2B"><img src="https://secure.avangate.com/images/merchant/69c418c33ec2e1a4267fa9bb77fa1428/general-970x90.gif" border="0"></a>
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
<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=174416&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.easygifanimator.net/images/gif-animator.png" border="0">Easy GIF Animator is a powerful animated GIF editor and the top tool for creating animated pictures, banners, buttons and GIF videos. You get extensive animation editing features, animation effects, unmatched image quality and optimization for the web. No other GIF animation software matches our features and ease of use, that's why Easy GIF Animator is so popular.</a>
<!-- affiliate ads end -->
![How to launch-Text-Generation-WebUI](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/6-launch-text-generation-webui.jpg)
6. The WebUI is now ready for use.  
<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4620778&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/07dd4d5a72f5740ef0f035f201951476/300__250banner.jpg" border="0"></a>
<!-- affiliate ads end -->
![Text-Generation-WebUI](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/7-text-generation-webui-view.jpg)

 However, the program is only a model loader. Let's download Llama 2 for the model loader to launch.

## Step 3: Download the Llama 2 Model

 There are quite a few things to consider when deciding which iteration of Llama 2 you need. These include parameters, quantization, hardware optimization, size, and usage. All of this information will be found denoted in the model's name.

* **Parameters:** The number of parameters used to train the model. Bigger parameters make more capable models but at the cost of performance.
* **Usage:** Can either be standard or chat. A chat model is optimized to be used as a chatbot like ChatGPT, while the standard is the default model.
* **Hardware Optimization:** Refers to what hardware best runs the model. GPTQ means the model is optimized to run on a dedicated GPU, while GGML is optimized to run on a CPU.
* **Quantization:** Denotes the precision of weights and activations in a model. For inferencing, a precision of q4 is optimal.
* **Size:** Refers to the size of the specific model.

 Note that some models may be arranged differently and may not even have the same types of information displayed. However, this type of naming convention is fairly common in the [HuggingFace](https://www.makeuseof.com/what-is-hugging-face-and-what-is-it-used-for/) Model library, so it's still worth understanding.

![HuggingFace model naming convention](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/wm/2023/10/huggingface-model-naming-convention-1.jpg)

 In this example, the model can be identified as a medium-sized Llama 2 model trained on 13 billion parameters optimized for chat inferencing using a dedicated CPU.

 For those running on a dedicated GPU, choose a **GPTQ** model, while for those using a CPU, choose **GGML**. If you want to chat with the model like you would with ChatGPT, choose **chat**, but if you want to experiment with the model with its full capabilities, use the **standard** model. As for parameters, know that using bigger models will provide better results at the expense of performance. I would personally recommend you start with a 7B model. As for quantization, use q4, as it's only for inferencing.

**Download:**[GGML](https://huggingface.co/localmodels/Llama-2-7B-ggml/tree/main) (Free)

**Download:**[GPTQ](https://huggingface.co/localmodels/Llama-2-7B-Chat-GPTQ/tree/main) (Free)

 Now that you know what iteration of Llama 2 you need, go ahead and download the model you want.

 In my case, since I'm running this on an ultrabook, I'll be using a GGML model fine-tuned for chat, **llama-2-7b-chat-ggmlv3.q4\_K\_S.bin.**

![Downloading Llama 2 model of your preference](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/8-download-llama-2-model.jpg)

<!-- affiliate ads begin -->
<a href="https://natural-cycles.sjv.io/c/5597632/2072200/17885" target="_top" id="2072200"><img src="//a.impactradius-go.com/display-ad/17885-2072200" border="0" alt="" width="728" height="90"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2072200/17885" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
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
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4530091&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.pearlmountainsoft.com/n_img/product/cit_win/banScrn.jpg" border="0">CollageIt Pro</a>
<!-- affiliate ads end -->
![Testing Llama 2 locally](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/12-testing-llama-2-locally.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=3922934&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/4b0a0290ad7df100b77e86839989a75e/products/ripperpro.png" border="0">WonderFox DVD Ripper Pro</a>
<!-- affiliate ads end -->
 Congratulations, you've successfully loaded Llama2 on your local computer!

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
<li><a href="https://facebook-video-share.techidaily.com/new-a-comprehensive-look-at-decelerating-youtube-video-speed-50-chars-for-2024/"><u>[New] A Comprehensive Look at Decelerating YouTube Video Speed (50 Chars) for 2024</u></a></li>
<li><a href="https://video-screen-grab.techidaily.com/new-pixireview-criticism-app-for-2024/"><u>[New] PixiReview Criticism App for 2024</u></a></li>
<li><a href="https://screen-activity-recording.techidaily.com/new-role-playing-realms-vintage-versus-variant-forms-for-2024/"><u>[New] Role-Playing Realms  Vintage Versus Variant Forms for 2024</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/updated-in-2024-instagram-influence-without-compromise/"><u>[Updated] In 2024, Instagram Influence Without Compromise</u></a></li>
<li><a href="https://screen-video-capture.techidaily.com/updated-perfectly-crafted-online-meeting-backdrops-for-2024/"><u>[Updated] Perfectly Crafted Online Meeting Backdrops for 2024</u></a></li>
<li><a href="https://screen-video-capture.techidaily.com/updated-transforming-viewers-experience-obs-strategies-on-youtube-and-twitch-for-2024/"><u>[Updated] Transforming Viewers' Experience  OBS Strategies on YouTube & Twitch for 2024</u></a></li>
<li><a href="https://extra-information.techidaily.com/2024-approved-colorful-compositions-in-a-click-photoshops-guide/"><u>2024 Approved  Colorful Compositions in a Click  Photoshop's Guide</u></a></li>
<li><a href="https://vimeo-videos.techidaily.com/2024-approved-crafting-quality-content-for-youtube-success/"><u>2024 Approved  Crafting Quality Content for YouTube Success</u></a></li>
<li><a href="https://youtube-videos.techidaily.com/2024-approved-embark-into-the-best-youtube-vr-content-ever/"><u>2024 Approved  Embark Into the Best YouTube VR Content Ever</u></a></li>
<li><a href="https://snapchat-videos.techidaily.com/2024-approved-interpreting-user-inactivity-could-it-be-a-blocked-status/"><u>2024 Approved  Interpreting User Inactivity  Could It Be a Blocked Status?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-breakthroughs-essential-updates-in-the-latest-chatgpt-version/"><u>AI Breakthroughs: Essential Updates in the Latest ChatGPT Version</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/beware-of-macapps-gpt-lures-hidden-dangers-revealed/"><u>Beware of MacApp's GPT Lures - Hidden Dangers Revealed</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/bootstrap-a-free-locally-hosted-chatgpt-relative-on-windows/"><u>Bootstrap a Free, Locally Hosted ChatGPT Relative on Windows</u></a></li>
<li><a href="https://youtube-web.techidaily.com/-your-content-download-complimentary-templates-for-youtube-makers-for-2024/"><u>Brand Your Content  Download Complimentary Templates for YouTube Makers for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/businesses-dilemnas-five-arguments-for-keeping-ai-out/"><u>Businesses' Dilemnas: Five Arguments for Keeping AI Out</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/can-chatgpt-create-a-breakthrough-in-health-tech/"><u>Can ChatGPT Create a Breakthrough in Health Tech?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatbots-explained-the-tech-thats-shaping-interactive-futures/"><u>Chatbots Explained: The Tech That's Shaping Interactive Futures</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-in-action-building-dynamic-and-intelligent-websites/"><u>ChatGPT in Action: Building Dynamic and Intelligent Websites</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpts-prescription-for-peacefulness/"><u>ChatGPT’s Prescription for Peacefulness</u></a></li>
<li><a href="https://mondly-stories.techidaily.com/chinese-letter-system-basics-for-new-learners/"><u>Chinese Letter System Basics for New Learners</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/elevate-conversations-the-compelling-case-for-chatgptplus-upgrade/"><u>Elevate Conversations - The Compelling Case for ChatGPT+ Upgrade</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/elevate-your-device-experience-smart-ai-search-from-bing/"><u>Elevate Your Device Experience: Smart AI Search From Bing.</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/essential-alterations-for-an-enhanced-user-experience-in-gpt-plugins-store/"><u>Essential Alterations for an Enhanced User Experience in GPT Plugins Store</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/expert-tips-genuine-gpt-practices/"><u>Expert Tips: Genuine GPT Practices</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/five-key-considerations-every-buyer-should-evaluate-before-acquiring-a-fitness-device/"><u>Five Key Considerations Every Buyer Should Evaluate Before Acquiring a Fitness Device</u></a></li>
<li><a href="https://youtube-video-recordings.techidaily.com/free-best-youtube-video-editor-apps-for-android/"><u>FREE Best YouTube Video Editor Apps for Android</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/generative-ai-redefining-professional-roles/"><u>Generative AI: Redefining Professional Roles</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/in-2024-how-to-cast-itel-p40-to-computer-for-iphone-and-android-drfone-by-drfone-android/"><u>In 2024, How to Cast Itel P40 to Computer for iPhone and Android? | Dr.fone</u></a></li>
<li><a href="https://location-social.techidaily.com/in-2024-how-to-change-your-oppo-a18-location-on-life360-without-anyone-knowing-drfone-by-drfone-virtual-android/"><u>In 2024, How to Change Your Oppo A18 Location on life360 Without Anyone Knowing? | Dr.fone</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/in-2024-how-to-use-pokemon-go-joystick-on-xiaomi-14-drfone-by-drfone-virtual-android/"><u>In 2024, How to use Pokemon Go Joystick on Xiaomi 14? | Dr.fone</u></a></li>
<li><a href="https://unlock-android.techidaily.com/in-2024-unlock-your-itel-p55-5g-phone-with-ease-the-3-best-lock-screen-removal-tools-by-drfone-android/"><u>In 2024, Unlock Your Itel P55 5G Phone with Ease The 3 Best Lock Screen Removal Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/innovative-applications-maximizing-chatgpts-vision-capabilities/"><u>Innovative Applications: Maximizing ChatGPT's Vision Capabilities</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/instructions-for-auto-gpt-installation/"><u>Instructions for Auto-GPT Installation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/jumping-to-ais-next-chapter-gpt-4-vs-gpt-35/"><u>Jumping to AI's Next Chapter: GPT-4 Vs. GPT-3.5</u></a></li>
<li><a href="https://audio-editing.techidaily.com/new-2024-approved-nero-waveedit-a-thorough-examination-updates/"><u>New 2024 Approved Nero WaveEdit A Thorough Examination Updates</u></a></li>
<li><a href="https://fix-guide.techidaily.com/nubia-red-magic-8s-pro-not-connecting-to-wi-fi-12-quick-ways-to-fix-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>Nubia Red Magic 8S Pro Not Connecting to Wi-Fi? 12 Quick Ways to Fix | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/openai-insiders-quick-reference-guide/"><u>OpenAI Insider's Quick Reference Guide</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/preventing-unauthorized-data-access-by-adaptive-ai/"><u>Preventing Unauthorized Data Access by Adaptive AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/questioning-the-reliability-of-zerogpt-and-similar-tech-tools/"><u>Questioning the Reliability of ZeroGPT & Similar Tech Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/real-world-examples-the-impact-of-gpt-today/"><u>Real-World Examples: The Impact of GPT Today</u></a></li>
<li><a href="https://some-guidance.techidaily.com/revamp-iphone-photos-effective-red-eye-removal-for-free-for-2024/"><u>Revamp iPhone Photos  Effective Red-Eye Removal for FREE for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/running-freechat-on-win-a-freedomgpt-guide/"><u>Running FreeChat on Win: A FreedomGPT Guide</u></a></li>
<li><a href="https://extra-resources.techidaily.com/skype-soundtrack-hub-finding-the-right-tones-online/"><u>Skype Soundtrack Hub  Finding the Right Tones Online</u></a></li>
<li><a href="https://win-blog.techidaily.com/1722984503353-stabilized-bioshock-2-remaster-discover-the-improved-adventure/"><u>Stabilized BioShock 2 Remaster: Discover the Improved Adventure</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/swift-communication-with-bing-ai-chat-on-your-android-keyboard/"><u>Swift Communication with Bing AI Chat on Your Android Keyboard</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-conundrum-of-tech-empathy-can-ai-mirror-our-feelings/"><u>The Conundrum of Tech Empathy: Can AI Mirror Our Feelings?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-future-of-digital-dialogue-mastering-the-art-of-custom-chatgpt-instructions/"><u>The Future of Digital Dialogue: Mastering the Art of Custom ChatGPT Instructions</u></a></li>
<li><a href="https://win-howtos.techidaily.com/ultimate-guide-resolving-airpods-connection-issues-on-windows-11/"><u>Ultimate Guide: Resolving AirPods Connection Issues on Windows 11</u></a></li>
<li><a href="https://ai-video-apps.techidaily.com/unleash-your-creativity-top-5-li-for-2024/"><u>Unleash Your Creativity Top 5 Li for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-palm-2-googles-enhanced-ai-linguistic-powerhouse/"><u>Unveiling PaLM 2: Google's Enhanced AI Linguistic Powerhouse</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-the-powers-of-co-pilot-in-chatgpt-applications/"><u>Unveiling the Powers of Co-Pilot in ChatGPT Applications</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/utilizing-anthropics-new-claude-prompts/"><u>Utilizing Anthropic's New Claude Prompts</u></a></li>
</ul></div>
