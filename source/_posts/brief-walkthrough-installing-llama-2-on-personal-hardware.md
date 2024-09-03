---
title: "Brief Walkthrough: Installing Llama 2 on Personal Hardware"
date: 2024-09-02T20:40:09.916Z
updated: 2024-09-03T20:40:09.916Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Brief Walkthrough: Installing Llama 2 on Personal Hardware"
excerpt: "This Article Describes Brief Walkthrough: Installing Llama 2 on Personal Hardware"
thumbnail: https://thmb.techidaily.com/a297ffbc354d264eb1493e128ad67218845cfbc005c6762fe341027fca06ba6f.jpg
---

## Brief Walkthrough: Installing Llama 2 on Personal Hardware

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
<!-- affiliate ads begin -->
<a href="https://shop.manycam.com/order/checkout.php?PRODS=17728032&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/8230bea7d54bcdf99cdfe85cb07313d5/mcaffbanner920x120.png" border="0"></a>
<!-- affiliate ads end -->
4. A terminal will open and start the setup. Early on, the setup will pause and ask you what GPU you are using. Select the appropriate type of GPU installed on your computer and hit enter. For those without a dedicated graphics card, select **None (I want to run models in CPU mode)**. Keep in mind that running on CPU mode is much slower when compared to running the model with a dedicated GPU.  
![Selecting GPU hardware installed](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/5-select-gpu-settings.jpg)
5. Once the setup is complete, you can now launch Text-Generation-WebUI locally. You can do so by opening your preferred web browser and entering the provided IP address on the URL.  
![How to launch-Text-Generation-WebUI](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/6-launch-text-generation-webui.jpg)
6. The WebUI is now ready for use.  
<!-- affiliate ads begin -->
<a href="https://versadesk.pxf.io/c/5597632/1892108/21290" target="_top" id="1892108"><img src="//a.impactradius-go.com/display-ad/21290-1892108" border="0" alt="" width="1080" height="1080"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1892108/21290" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![Text-Generation-WebUI](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/7-text-generation-webui-view.jpg)

<!-- affiliate ads begin -->
<a href="https://store.nero.com/order/checkout.php?PRODS=42296855&QTY=1&AFFILIATE=108875&CART=1"><img src="http://cdnwww.nero.com/nero-com-wAssets/img/banners/2023/recode/Nero_Recode_Screen_2.png" border="0"></a>
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
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=30901369&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/ce9a6fb2becc2d235e62b125e9260102/products/1_copy_vMixCallScreenshot1-large.jpg" border="0"> vMix 4K - Software based live production. vMix 4K includes everything in vMix HD plus 4K support, PTZ control, External/Fullscreen output, 4 Virtual Outputs, 1 Replay, 4 vMix Call, and 2 Recorders. 
This bundle includes Studio 200 for vMix from Virtualsetworks, HTTP Matrix 1.0 automation scheduler, and 4 introductory training videos from the Udemy vMix Basic to Amazing course. </a>
<!-- affiliate ads end -->
 After the download is finished, place the model in **text-generation-webui-main** \> **models**.

![Placing Llama 2 model to model folder](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/9-place-model-to-model-folder.jpg)

Now that you have your model downloaded and placed in the model folder, it's time to configure the model loader.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4631056&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/997e65474a248252883b485717f7d098/products/buy-windows.png" border="0">Allavsoft Batch Download Online Videos, Music Offline to MP4, MP3, MOV, etc format </a>
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
<a href="https://turbotech.pxf.io/c/5597632/1450763/17212" target="_top" id="1450763"><img src="//a.impactradius-go.com/display-ad/17212-1450763" border="0" alt="" width="2560" height="1440"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1450763/17212" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://vp-tips.techidaily.com/new-2024-approved-cycle-shaper-set/"><u>[New] 2024 Approved  Cycle Shaper Set</u></a></li>
<li><a href="https://screen-capture.techidaily.com/new-how-to-enhance-audibility-with-adjusted-obs-settings-for-2024/"><u>[New] How to Enhance Audibility with Adjusted OBS Settings for 2024</u></a></li>
<li><a href="https://fox-friendly.techidaily.com/new-in-2024-demystifying-virtual-reality-headsets-explained/"><u>[New] In 2024, Demystifying Virtual Reality Headsets Explained</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/updated-exclusive-perk-dji-miniair-2-owners-get-20-free-luts/"><u>[Updated] Exclusive Perk  DJI Mini/Air 2 Owners Get 20 Free LUTS</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/updated-how-to-record-audio-with-audacity-on-mac-in-2024/"><u>[Updated] How to Record Audio with Audacity on Mac, In 2024</u></a></li>
<li><a href="https://facebook-video-recording.techidaily.com/updated-in-2024-virtual-venue-vaults-audiences/"><u>[Updated] In 2024, Virtual Venue Vaults Audiences</u></a></li>
<li><a href="https://instagram-clips.techidaily.com/2024-approved-unlocking-content-discovery-with-instagram-hashtags/"><u>2024 Approved  Unlocking Content Discovery with Instagram Hashtags</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/academic-writing-under-ai-scrutiny-are-student-papers-still-relevant/"><u>Academic Writing Under AI Scrutiny: Are Student Papers Still Relevant?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/adaptive-language-learning-via-chatgpt-plus-interface/"><u>Adaptive Language Learning via ChatGPT Plus Interface</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-innovation-duels-googles-gemini-vs-openais-chatgpt/"><u>AI Innovation Duels: Google's Gemini Vs. OpenAI’s ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-revolution-which-professions-might-be-abolished/"><u>AI Revolution: Which Professions Might Be Abolished?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/an-in-depth-look-at-claude-pros-differences-from-gptplusplus/"><u>An In-Depth Look at Claude Pro’s Differences From GPT++</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/artificial-intelligence-meets-content-creation/"><u>Artificial Intelligence Meets Content Creation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/augmenting-crypto-dialogues-gpts-top-8-integrative-tools-revealed/"><u>Augmenting Crypto Dialogues: GPT's Top 8 Integrative Tools Revealed</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/become-a-directive-design-whiz-the-top-7-online-helpful-apps/"><u>Become a Directive Design Whiz: The Top 7 Online Helpful Apps</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/charming-cyberspace-ai-for-romance-fraud/"><u>Charming Cyberspace: AI for Romance Fraud</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/cyber-threat-alert-the-risky-side-of-google-bard-download/"><u>Cyber Threat Alert: The Risky Side of Google Bard Download</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/deciphering-codegpt-the-future-of-programming-with-ai/"><u>Deciphering CodeGPT: The Future of Programming with AI?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/defining-intelligence-will-ai-beat-human-judges/"><u>Defining Intelligence: Will AI Beat Human Judges?</u></a></li>
<li><a href="https://twitter-videos.techidaily.com/direct-twitter-media-transfer-to-whatsapp-for-2024/"><u>Direct Twitter Media Transfer to WhatsApp for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/echoing-futures-next-generation-of-ai-talks/"><u>Echoing Futures: Next Generation of AI Talks</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/elevate-your-workflow-6-top-uses-for-ai-in-data-analysis/"><u>Elevate Your Workflow: 6 Top Uses for AI in Data Analysis</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/embrace-human-touch-with-the-help-of-artificial-intelligence/"><u>Embrace Human Touch with the Help of Artificial Intelligence</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/evaluating-the-security-of-ai-powered-conversations/"><u>Evaluating the Security of AI-Powered Conversations</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/exploring-llama-2s-features-and-applications/"><u>Exploring Llama 2'S Features and Applications</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/exploring-the-separate-worlds-of-nlp-ml/"><u>Exploring the Separate Worlds of NLP, ML</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/gpts-content-creation-vs-se-expertise/"><u>GPT's Content Creation vs SE Expertise</u></a></li>
<li><a href="https://fake-location.techidaily.com/how-to-fix-nokia-c210-find-my-friends-no-location-found-drfone-by-drfone-virtual-android/"><u>How to Fix Nokia C210 Find My Friends No Location Found? | Dr.fone</u></a></li>
<li><a href="https://vimeo-videos.techidaily.com/in-2024-the-artisans-guide-to-flawless-free-and-paid-software-video-downloads/"><u>In 2024, The Artisan's Guide to Flawless Free and Paid Software Video Downloads</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/innovation-in-interaction-top-5-advanced-ai-prompts-creators/"><u>Innovation in Interaction: Top 5 Advanced AI Prompts Creators</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/language-learning-lab-mistral-versus-chatgpt/"><u>Language Learning Lab: Mistral Versus ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-ai-language-understanding-the-fundamentals/"><u>Mastering AI Language: Understanding the Fundamentals</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-gpt-8-essential-methods/"><u>Mastering GPT: 8 Essential Methods</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/premium-gpts-role-in-achieving-language-excellence/"><u>Premium GPT's Role in Achieving Language Excellence</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/regulating-a-rapidly-evolving-ai-world-ceos-stance/"><u>Regulating a Rapidly Evolving AI World: CEO's Stance</u></a></li>
<li><a href="https://win-answers.techidaily.com/resolving-your-battle-royale-woes-what-to-do-if-warzone-wont-launch/"><u>Resolving Your Battle Royale Woes: What To Do If Warzone Won't Launch</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/rise-of-robots-survival-of-the-human-spirit-workplace-wisdom/"><u>Rise of Robots, Survival of the Human Spirit: Workplace Wisdom</u></a></li>
<li><a href="https://tech-revival.techidaily.com/steps-to-start-your-journey-as-a-prompt-engineer/"><u>Steps to Start Your Journey as a Prompt Engineer</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/synergy-in-silicon-bots-tasked-with-equal-creativity-goals/"><u>Synergy in Silicon: Bots Tasked with Equal Creativity Goals</u></a></li>
<li><a href="https://vp-tips.techidaily.com/the-future-is-here-magix-vpx-unveiled-and-tested/"><u>The Future Is Here  Magix VPX Unveiled and Tested</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-making-of-ai-interactions-is-it-an-employable-skill/"><u>The Making of AI Interactions: Is It an Employable Skill?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-rise-of-virtual-therapy-top-5-bot-innovations/"><u>The Rise of Virtual Therapy: Top 5 Bot Innovations</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-ultimate-guide-to-prime-notetaking-with-ai-innovations/"><u>The Ultimate Guide to Prime Notetaking with AI Innovations</u></a></li>
<li><a href="https://youtube-videos.techidaily.com/transforming-ordinary-videos-into-viral-hits-with-innovative-thumbnails/"><u>Transforming Ordinary Videos Into Viral Hits with Innovative Thumbnails</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/trim-perfect-clearing-thin-lines-on-youtube-for-2024/"><u>Trim Perfect  Clearing Thin Lines on YouTube for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/truth-unveiled-no-gpt-windows-client-is-not-malware/"><u>Truth Unveiled: No, GPT-Windows Client Is Not Malware</u></a></li>
<li><a href="https://techidaily.com/undelete-lost-music-from-samsung-galaxy-a15-5g-by-fonelab-android-recover-music/"><u>Undelete lost music from Samsung Galaxy A15 5G</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unleash-potential-top-7-ways-gpt-improves-workday-effectiveness/"><u>Unleash Potential: Top 7 Ways GPT Improves Workday Effectiveness</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unlocking-new-linguistic-skills-through-gpt-plus/"><u>Unlocking New Linguistic Skills Through GPT Plus</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unraveling-intrinsic-intelligence-implementations-in-hardware/"><u>Unraveling Intrinsic Intelligence Implementations in Hardware</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-cgps-accuracy-in-medical-dialogues/"><u>Unveiling CGP's Accuracy in Medical Dialogues</u></a></li>
<li><a href="https://hardware-updates.techidaily.com/winning-the-battle-against-windows-10-bluetooth-driver-troubles-final-solution/"><u>Winning the Battle Against Windows 10 Bluetooth Driver Troubles [FINAL SOLUTION]</u></a></li>
</ul></div>
