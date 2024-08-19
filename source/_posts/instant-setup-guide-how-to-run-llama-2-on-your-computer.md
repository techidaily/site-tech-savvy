---
title: "Instant Setup Guide: How to Run Llama 2 on Your Computer"
date: 2024-08-18T09:56:58.777Z
updated: 2024-08-19T09:56:58.777Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Instant Setup Guide: How to Run Llama 2 on Your Computer"
excerpt: "This Article Describes Instant Setup Guide: How to Run Llama 2 on Your Computer"
thumbnail: https://thmb.techidaily.com/b2e6162c64c71916b12953aa4e598d6dbab13589e9351dbafbf801be610ecb70.jpg
---

## Instant Setup Guide: How to Run Llama 2 on Your Computer

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
<a href="https://store.nero.com/order/checkout.php?PRODS=22889392&QTY=1&AFFILIATE=108875&CART=1"><img src="http://webstatic.nero.com/nero2015-com-wAssets/img/affiliate/media/banner728-90eng.jpg" border="0"></a>
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
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=30901410&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/ce9a6fb2becc2d235e62b125e9260102/products/copy_1_copy_vMixCallScreenshot1-large.jpg" border="0"> vMix Pro - Software based live production. vMix Pro includes everything in vMix 4K plus 8 channels of Replay and 8 vMix Call 
This bundle includes Studio 200 for vMix from Virtualsetworks, HTTP Matrix 1.0 automation scheduler, and 4 introductory training videos from the Udemy vMix Basic to Amazing course. </a>
<!-- affiliate ads end -->
![How to launch-Text-Generation-WebUI](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/6-launch-text-generation-webui.jpg)
6. The WebUI is now ready for use.  
![Text-Generation-WebUI](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/7-text-generation-webui-view.jpg)

<!-- affiliate ads begin -->
<a href="https://shop.dbschema.com/order/checkout.php?PRODS=19867419&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/176b22bab4e94a28619ca2433b2ef241/products/1_icon256.png" border="0">
DbSchema database designer for all databases, schema design in the team, schema deployment, interactive diagrams, documentation, data and query tools. </a>
<!-- affiliate ads end -->
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
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=3851655&QTY=1&AFFILIATE=108875&CART=1"><img src="http://www.aiseesoft.com/avangate/30p/banner.jpg" border="0"></a>
<!-- affiliate ads end -->
 After the download is finished, place the model in **text-generation-webui-main** \> **models**.

![Placing Llama 2 model to model folder](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/9-place-model-to-model-folder.jpg)

Now that you have your model downloaded and placed in the model folder, it's time to configure the model loader.

<!-- affiliate ads begin -->
<a href="https://turtlebeacheu.sjv.io/c/5597632/1996818/23722" target="_top" id="1996818"><img src="//a.impactradius-go.com/display-ad/23722-1996818" border="0" alt="" width="600" height="600"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1996818/23722" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Step 4: Configure Text-Generation-WebUI

 Now, let's begin the configuration phase.

1. Once again, open Text-Generation-WebUI by running the **start\_(your OS)** file (see the previous steps above).
2. On the tabs located above the GUI, click **Model.** Click the refresh button at the model dropdown menu and select your model.
3. Now click on the dropdown menu of the **Model loader** and select **AutoGPTQ** for those using a GTPQ model and **ctransformers** for those using a GGML model. Finally, click on **Load** to load your model.  
![Setting model loader](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/10-select-model-loader.jpg)
4. To use the model, open the Chat tab and start testing the model.  
![Testing Llama 2 locally](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/12-testing-llama-2-locally.jpg)

 Congratulations, you've successfully loaded Llama2 on your local computer!

<!-- affiliate ads begin -->
<a href="https://store.revouninstaller.com/order/checkout.php?PRODS=28010250&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/4282ec8de8c9be897e7aff4aa231b1a4/336__280a.jpg" border="0"></a>
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
<li><a href="https://fox-http.techidaily.com/new-2024-approved-connect-and-play-xbox-one-zoom-guidebook/"><u>[New] 2024 Approved  Connect and Play  Xbox One Zoom Guidebook</u></a></li>
<li><a href="https://twitter-clips.techidaily.com/new-amplify-volume-for-twitters-silent-videos/"><u>[New] Amplify Volume for Twitter's Silent Videos</u></a></li>
<li><a href="https://facebook-videos.techidaily.com/new-detailed-instructions-mastering-the-art-of-uploading-vr-media-to-fb/"><u>[New] Detailed Instructions  Mastering the Art of Uploading VR Media to FB</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/new-exclusive-insights-elevating-your-mobizen-screencast-game/"><u>[New] Exclusive Insights  Elevating Your Mobizen Screencast Game</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-how-to-create-time-lapse-video-with-canon-camera/"><u>[New] How to Create Time-Lapse Video with Canon Camera</u></a></li>
<li><a href="https://facebook-video-content.techidaily.com/new-premier-mp4-uploader-and-downloader-for-fb-for-2024/"><u>[New] Premier MP4 Uploader & Downloader for FB for 2024</u></a></li>
<li><a href="https://facebook-video-footage.techidaily.com/updated-2024-approved-dominate-youtube-traffic-with-proficient-use-of-creator-studio/"><u>[Updated] 2024 Approved  Dominate YouTube Traffic with Proficient Use of Creator Studio</u></a></li>
<li><a href="https://facebook-video-share.techidaily.com/updated-download-youtube-icons-quickly-web-os-specific-options-explained-for-2024/"><u>[Updated] Download YouTube Icons Quickly  Web, OS-Specific Options Explained for 2024</u></a></li>
<li><a href="https://twitter-videos.techidaily.com/updated-enhancing-conversion-rates-with-twitter-ads/"><u>[Updated] Enhancing Conversion Rates with Twitter Ads</u></a></li>
<li><a href="https://instagram-clips.techidaily.com/updated-exclusive-guide-ranking-most-effective-ig-money-makers/"><u>[Updated] Exclusive Guide  Ranking Most Effective IG Money Makers</u></a></li>
<li><a href="https://fox-helps.techidaily.com/updated-minds-on-trial-best-general-knowledge-channels-for-2024/"><u>[Updated] Minds on Trial  Best General Knowledge Channels for 2024</u></a></li>
<li><a href="https://youtube-clips.techidaily.com/2024-approved-elevate-your-recordings-doing-without-a-microphone/"><u>2024 Approved  Elevate Your Recordings  Doing Without a Microphone</u></a></li>
<li><a href="https://screen-video-capture.techidaily.com/2024-approved-high-definition-top-win-11-cameras-and-recorder-list/"><u>2024 Approved  High Definition  Top Win 11 Cameras and Recorder List</u></a></li>
<li><a href="https://extra-support.techidaily.com/2024-approved-laugh-o-matic-crafting-gags-on-the-house-rate/"><u>2024 Approved  Laugh-O-Matic  Crafting Gags on the House Rate</u></a></li>
<li><a href="https://article-knowledge.techidaily.com/2024-approved-pathways-to-accumulate-free-photo-frame-media/"><u>2024 Approved  Pathways to Accumulate Free Photo Frame Media</u></a></li>
<li><a href="https://howto.techidaily.com/7-solutions-to-fix-error-code-963-on-google-play-of-oppo-find-x7-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>7 Solutions to Fix Error Code 963 on Google Play Of Oppo Find X7 | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ais-might-matrix-the-vital-variants/"><u>AI's Might Matrix: The Vital Variants</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/algorithmic-humorists-at-play-will-tech-tickle-us/"><u>Algorithmic Humorists at Play: Will Tech Tickle Us?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/all-now-free-explore-gpt-4-but-dont-disregard-plus-perks/"><u>All Now Free: Explore GPT-4, But Don't Disregard Plus Perks</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/auto-gtp-innovation-hacks-for-professionals/"><u>Auto-GTP Innovation Hacks for Professionals</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chat-ai-showdown-10-traits-of-gpt-and-bingbot/"><u>Chat AI Showdown: 10 Traits of GPT and BingBot</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/command-line-conversations-bash-and-chatgpt/"><u>Command-Line Conversations: Bash and ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/decoding-and-rectifying-6-predominant-chatgpt-errors/"><u>Decoding and Rectifying 6 Predominant ChatGPT Errors</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/elevate-your-argumentation-skills-with-gpt-assisted-proposals/"><u>Elevate Your Argumentation Skills with GPT-Assisted Proposals</u></a></li>
<li><a href="https://some-techniques.techidaily.com/evaluating-spend-on-youtube-campaigns-for-2024/"><u>Evaluating Spend on YouTube Campaigns for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/exploring-vector-databases-for-ai-progress/"><u>Exploring Vector Databases for AI Progress</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/from-conversations-to-characters-developing-personas-in-chatgpt/"><u>From Conversations to Characters: Developing Personas in ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/google-unveils-bard-new-ai-to-challenge-chatgpts-dominance/"><u>Google Unveils 'Bard', New AI To Challenge ChatGPT's Dominance</u></a></li>
<li><a href="https://apple-account.techidaily.com/how-to-erase-an-iphone-12-pro-without-apple-id-password-by-drfone-ios/"><u>How To Erase an iPhone 12 Pro Without Apple ID Password?</u></a></li>
<li><a href="https://unlock-android.techidaily.com/in-2024-how-to-unlock-xiaomi-redmi-note-13-5g-phone-without-password-by-drfone-android/"><u>In 2024, How To Unlock Xiaomi Redmi Note 13 5G Phone Without Password?</u></a></li>
<li><a href="https://some-skills.techidaily.com/in-2024-ultimate-techniques-for-youtube-mp4-creation/"><u>In 2024, Ultimate Techniques for YouTube MP4 Creation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/initiating-auto-excellence-with-ai-dialogues-and-advice/"><u>Initiating Auto Excellence with AI Dialogues and Advice</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/intrinsic-computation-how-devices-learn-independently/"><u>Intrinsic Computation: How Devices Learn Independently</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/investigating-codegpt-is-it-a-new-developer-tool/"><u>Investigating CodeGPT: Is It a New Developer Tool?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/is-dialogue-with-humans-critical-for-machines-knowledge-expansion/"><u>Is Dialogue With Humans Critical for Machine's Knowledge Expansion?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/is-elite-access-to-gpt-justifiable/"><u>Is Elite Access to GPT Justifiable?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/italys-swift-ban-on-chatgpt-whats-the-reason/"><u>Italy's Swift Ban on ChatGPT: What's the Reason?</u></a></li>
<li><a href="https://techno-recovery.techidaily.com/macbook-multi-monitor-mastery-a-step-by-step-guide/"><u>MacBook Multi-Monitor Mastery: A Step-by-Step Guide</u></a></li>
<li><a href="https://tech-revival.techidaily.com/master-the-kitchen-with-ai-7-uses-of-chatgpt-for-aspiring-chefs/"><u>Master the Kitchen with AI: 7 Uses of ChatGPT for Aspiring Chefs</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-chatgpt-top-5-tactics-for-crafting-excellent-prompts/"><u>Mastering ChatGPT: Top 5 Tactics for Crafting Excellent Prompts</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-talks-with-these-7-ai-tools/"><u>Mastering Talks with These 7 AI Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/million-dollar-context-geminis-15-evolved-strategy-revealed/"><u>Million Dollar Context: Gemini's 1.5 Evolved Strategy Revealed</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/newsfeed-reimagined-by-google/"><u>NewsFeed Reimagined by Google</u></a></li>
<li><a href="https://howto.techidaily.com/oneplus-open-camera-not-working-unexpected-error-fix-it-now-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>OnePlus Open Camera Not Working Unexpected Error? Fix It Now | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/protecting-intellectual-property-business-gpt-use/"><u>Protecting Intellectual Property: Business GPT Use</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/redefine-mobile-browsing-bings-intelligent-search-now-available/"><u>Redefine Mobile Browsing - Bing's Intelligent Search Now Available</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/securing-tech-bargains-ransomware-decryption-explained/"><u>Securing Tech Bargains: Ransomware Decryption Explained</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/sifting-truth-in-online-medical-advice-by-ai/"><u>Sifting Truth in Online Medical Advice by AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/storing-permanent-records-of-gpt-talks/"><u>Storing Permanent Records of GPT Talks</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/tailor-made-ai-the-complete-guide-to-crafted-gpt/"><u>Tailor-Made AI: The Complete Guide to Crafted GPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-art-of-crafting-unique-chatgpt-directives/"><u>The Art of Crafting Unique ChatGPT Directives</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/the-rise-and-challenges-of-video-streaming-profits-for-2024/"><u>The Rise and Challenges of Video Streaming Profits for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-split-path-of-natural-language-and-ml-tech/"><u>The Split Path of Natural Language and ML Tech</u></a></li>
<li><a href="https://apple-account.techidaily.com/troubleshooting-error-connecting-to-the-apple-id-server-on-apple-iphone-14-by-drfone-ios/"><u>Troubleshooting Error Connecting to the Apple ID Server On Apple iPhone 14</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unlock-the-potential-of-your-website-via-chatgpts-4-pathways/"><u>Unlock the Potential of Your Website via ChatGPT's 4 Pathways</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/what-you-can-achieve-with-claude-3/"><u>What You Can Achieve With Claude 3</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/who-should-programmers-pick-for-efficiency-copilotchatgpt-discussion/"><u>Who Should Programmers Pick for Efficiency? Copilot/ChatGPT Discussion</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/witty-wordsmiths-war-chatgpt-vs-the-wise-bard/"><u>Witty Wordsmiths' War: ChatGPT Vs. The Wise Bard</u></a></li>
</ul></div>
