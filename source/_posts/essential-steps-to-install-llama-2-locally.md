---
title: Essential Steps to Install Llama 2 Locally
date: 2024-07-20T06:23:36.495Z
updated: 2024-07-21T06:23:36.495Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Essential Steps to Install Llama 2 Locally
excerpt: This Article Describes Essential Steps to Install Llama 2 Locally
thumbnail: https://thmb.techidaily.com/b2faccf55ba2f62eeda01fb2856eae6cf952310d841c8d8317d40b9a309e6901.jpg
---

## Essential Steps to Install Llama 2 Locally

 Meta released Llama 2 in the summer of 2023\. The new version of Llama is fine-tuned with 40% more tokens than the original Llama model, doubling its context length and significantly outperforming other open-sourced models available. The fastest and easiest way to access Llama 2 is via an API through an online platform. However, if you want the best experience, installing and loading Llama 2 directly on your computer is best.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 With that in mind, we've created a step-by-step guide on how to use Text-Generation-WebUI to load a quantized Llama 2 LLM locally on your computer.

<!-- affiliate ads begin -->
<a href="https://laganoo.pxf.io/c/5597632/1657399/16446" target="_top" id="1657399"><img src="//a.impactradius-go.com/display-ad/16446-1657399" border="0" alt="" width="728" height="90"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1657399/16446" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Why Install Llama 2 Locally

 There are many reasons why people choose to run Llama 2 directly. Some do it for privacy concerns, some for customization, and others for offline capabilities. If you're researching, fine-tuning, or integrating Llama 2 for your projects, then accessing Llama 2 via API might not be for you. The point of running an LLM locally on your PC is to reduce reliance on [third-party AI tools](https://www.makeuseof.com/best-ai-web-apps/) and use AI anytime, anywhere, without worrying about leaking potentially sensitive data to companies and other organizations.

 With that said, let's begin with the step-by-step guide to installing Llama 2 locally.

## Step 1: Install Visual Studio 2019 Build Tool

 To simplify things, we will use a one-click installer for Text-Generation-WebUI (the program used to load Llama 2 with GUI). However, for this installer to work, you need to download the Visual Studio 2019 Build Tool and install the necessary resources.

**Download:**[Visual Studio 2019](https://learn.microsoft.com/en-us/visualstudio/releases/2019/release-notes) (Free)

1. Go ahead and download the community edition of the software.
2. Now install Visual Studio 2019, then open the software. Once opened, tick the box on **Desktop development with C++** and hit install.  
<!-- affiliate ads begin -->
<a href="https://zonlipartnershipprogram.pxf.io/c/5597632/1611407/17882" target="_top" id="1611407"><img src="//a.impactradius-go.com/display-ad/17882-1611407" border="0" alt="" width="300" height="485"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1611407/17882" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![Install-Desktop-Development-With-C++](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/2-install-desktop-development-with-c.jpg)

 Now that you have Desktop development with C++ installed, it's time to download the Text-Generation-WebUI one-click installer.

<!-- affiliate ads begin -->
<a href="https://store.iobit.com/order/checkout.php?PRODS=4596923&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/184260348236f9554fe9375772ff966e/ascscan_468X60.png" border="0"></a>
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
<a href="https://ancheer.sjv.io/c/5597632/1657301/17326" target="_top" id="1657301"><img src="//a.impactradius-go.com/display-ad/17326-1657301" border="0" alt="" width="1920" height="933"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1657301/17326" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![How to launch-Text-Generation-WebUI](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/6-launch-text-generation-webui.jpg)
6. The WebUI is now ready for use.  
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

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2082529/7443" target="_top" id="2082529"><img src="//a.impactradius-go.com/display-ad/7443-2082529" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2082529/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![HuggingFace model naming convention](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/wm/2023/10/huggingface-model-naming-convention-1.jpg)

 In this example, the model can be identified as a medium-sized Llama 2 model trained on 13 billion parameters optimized for chat inferencing using a dedicated CPU.

 For those running on a dedicated GPU, choose a **GPTQ** model, while for those using a CPU, choose **GGML**. If you want to chat with the model like you would with ChatGPT, choose **chat**, but if you want to experiment with the model with its full capabilities, use the **standard** model. As for parameters, know that using bigger models will provide better results at the expense of performance. I would personally recommend you start with a 7B model. As for quantization, use q4, as it's only for inferencing.

**Download:**[GGML](https://huggingface.co/localmodels/Llama-2-7B-ggml/tree/main) (Free)

**Download:**[GPTQ](https://huggingface.co/localmodels/Llama-2-7B-Chat-GPTQ/tree/main) (Free)

 Now that you know what iteration of Llama 2 you need, go ahead and download the model you want.

 In my case, since I'm running this on an ultrabook, I'll be using a GGML model fine-tuned for chat, **llama-2-7b-chat-ggmlv3.q4\_K\_S.bin.**

![Downloading Llama 2 model of your preference](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/8-download-llama-2-model.jpg)

 After the download is finished, place the model in **text-generation-webui-main** \> **models**.

<!-- affiliate ads begin -->
<a href="https://zonlipartnershipprogram.pxf.io/c/5597632/1596691/17882" target="_top" id="1596691"><img src="//a.impactradius-go.com/display-ad/17882-1596691" border="0" alt="" width="728" height="90"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1596691/17882" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![Placing Llama 2 model to model folder](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/9-place-model-to-model-folder.jpg)

Now that you have your model downloaded and placed in the model folder, it's time to configure the model loader.

## Step 4: Configure Text-Generation-WebUI

 Now, let's begin the configuration phase.

1. Once again, open Text-Generation-WebUI by running the **start\_(your OS)** file (see the previous steps above).
2. On the tabs located above the GUI, click **Model.** Click the refresh button at the model dropdown menu and select your model.
3. Now click on the dropdown menu of the **Model loader** and select **AutoGPTQ** for those using a GTPQ model and **ctransformers** for those using a GGML model. Finally, click on **Load** to load your model.  
<!-- affiliate ads begin -->
<a href="https://store.massmailsoftware.com/order/checkout.php?PRODS=1300375&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/dc87c13749315c7217cdc4ac692e704c/banera_for_partners-15_%281%29.jpg" border="0"></a>
<!-- affiliate ads end -->
![Setting model loader](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/10-select-model-loader.jpg)
4. To use the model, open the Chat tab and start testing the model.  
![Testing Llama 2 locally](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/12-testing-llama-2-locally.jpg)

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
<li><a href="https://facebook-video-content.techidaily.com/new-conveniently-record-your-favorite-streams-top-5-grabber-apps-for-2024/"><u>[New] Conveniently Record Your Favorite Streams  Top 5 Grabber Apps for 2024</u></a></li>
<li><a href="https://discord-videos.techidaily.com/new-in-2024-top-discord-rivals-worth-exploring/"><u>[New] In 2024, Top Discord Rivals Worth Exploring</u></a></li>
<li><a href="https://twitter-videos.techidaily.com/updated-2024-approved-tiktok-triumphs-in-twitter-land-toptiktoks-revealed/"><u>[Updated] 2024 Approved  TikTok Triumphs in Twitter Land  #TopTikToks Revealed</u></a></li>
<li><a href="https://snapchat-videos.techidaily.com/2024-approved-snapchat-artistry-integrating-anime-inspired-effects/"><u>2024 Approved  Snapchat Artistry  Integrating Anime-Inspired Effects</u></a></li>
<li><a href="https://vp-tips.techidaily.com/2024-approved-transform-your-livestreams-with-eco-friendly-screen-effects/"><u>2024 Approved  Transform Your Livestreams with Eco-Friendly Screen Effects</u></a></li>
<li><a href="https://iphone-unlock.techidaily.com/5-most-effective-methods-to-unlock-iphone-15-plus-in-lost-mode-drfone-by-drfone-ios/"><u>5 Most Effective Methods to Unlock iPhone 15 Plus in Lost Mode | Dr.fone</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/a-guide-vivo-s17-wireless-and-wired-screen-mirroring-drfone-by-drfone-android/"><u>A Guide Vivo S17 Wireless and Wired Screen Mirroring | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/blizzards-new-chapter-with-microsoft-unveils-innovative-use-of-ai-in-gaming-and-artistry-audio-analysis/"><u>Blizzard's New Chapter with Microsoft Unveils Innovative Use of AI in Gaming & Artistry [Audio Analysis]</u></a></li>
<li><a href="https://extra-resources.techidaily.com/breaking-free-from-virtual-reality-discomfort-for-2024/"><u>Breaking Free From Virtual Reality Discomfort for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/bypassing-user-interface-direct-engagement-through-shellgpt/"><u>Bypassing User Interface: Direct Engagement Through ShellGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-love-lines-a-modern-approach-to-mates/"><u>ChatGPT Love Lines: A Modern Approach to Mates</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-unveiled-a-familys-perspective/"><u>ChatGPT Unveiled: A Family's Perspective</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-the-ai-thats-revolutionizing-video-content-crafting/"><u>ChatGPT: The AI That's Revolutionizing Video Content Crafting</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/claude-vs-chatgpt-the-4-innovative-improvements-that-redefine-interaction/"><u>Claude vs ChatGPT: The 4 Innovative Improvements that Redefine Interaction</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/decoding-5-key-reasons-companies-shy-away-from-gpt-applications/"><u>Decoding 5 Key Reasons Companies Shy Away From GPT Applications</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/elevate-your-abodes-productivity-with-chatgpt-techniques/"><u>Elevate Your Abode's Productivity with ChatGPT Techniques</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/embark-without-worry-best-free-chatgpt-apps-crafting-your-trip/"><u>Embark Without Worry: Best Free ChatGPT Apps Crafting Your Trip</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/essential-overlooked-gpt-features-for-innovative-dialogue/"><u>Essential, Overlooked GPT Features for Innovative Dialogue</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/expert-advice-on-lifting-your-chatgpt-ban/"><u>Expert Advice on Lifting Your ChatGPT Ban</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/fostering-fiction-6-ways-to-harness-chatgpt/"><u>Fostering Fiction: 6 Ways to Harness ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721431815367-free-access-now-however-platinum-plans-6-benefits-are-still-compelling/"><u>Free Access Now! However, Platinum Plan's 6 Benefits Are Still Compelling.</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721423078139-from-bots-to-iphones-chatgpt-arrives/"><u>From Bots to iPhones: ChatGPT Arrives</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-create-user-personas-in-chatgpt-for-better-results/"><u>How to Create User Personas in ChatGPT for Better Results</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/improving-blog-commentaries-with-ai-wisdom/"><u>Improving Blog Commentaries with AI Wisdom</u></a></li>
<li><a href="https://extra-information.techidaily.com/in-2024-beyond-the-viewfinder-top-6-android-and-ios-video-apps/"><u>In 2024, Beyond the Viewfinder  Top 6 Android and iOS Video Apps</u></a></li>
<li><a href="https://ios-pokemon-go.techidaily.com/in-2024-how-can-i-create-my-pokemon-overworld-maps-on-apple-iphone-13-drfone-by-drfone-virtual-ios/"><u>In 2024, How Can I Create My Pokemon Overworld Maps On Apple iPhone 13? | Dr.fone</u></a></li>
<li><a href="https://review-topics.techidaily.com/in-2024-how-to-change-google-play-location-on-vivo-s17t-drfone-by-drfone-virtual-android/"><u>In 2024, How to Change Google Play Location On Vivo S17t | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/intellectual-frontier-can-computers-triumph/"><u>Intellectual Frontier: Can Computers Triumph?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/introducing-mac-friendly-communication-with-gpt/"><u>Introducing Mac-Friendly Communication with GPT</u></a></li>
<li><a href="https://youtube-zero.techidaily.com/-vids-unpacked-whats-the-score-in-2024/"><u>Micro Vids Unpacked  What's the Score, In 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/navigating-the-features-of-llama-2-with-ease/"><u>Navigating the Features of Llama 2 with Ease</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/navigating-the-world-of-public-gpt-conversations/"><u>Navigating the World of Public GPT Conversations</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/optimizing-corporate-correspondence-via-ai-practical-tips-and-tricks/"><u>Optimizing Corporate Correspondence via AI: Practical Tips & Tricks</u></a></li>
<li><a href="https://fix-guide.techidaily.com/reasons-for-oppo-find-x6-pro-stuck-on-startup-screen-and-ways-to-fix-them-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>Reasons for Oppo Find X6 Pro Stuck on Startup Screen and Ways To Fix Them | Dr.fone</u></a></li>
<li><a href="https://easy-unlock-android.techidaily.com/remove-the-lock-screen-fingerprint-of-your-realme-c53-by-drfone-android/"><u>Remove the Lock Screen Fingerprint Of Your Realme C53</u></a></li>
<li><a href="https://extra-support.techidaily.com/samsungs-virtual-world-enhanced-by-compatible-smartphones-2023-guide-for-2024/"><u>Samsung's Virtual World Enhanced by Compatible Smartphones - 2023 Guide for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/six-budget-friendly-artificial-intelligence-options/"><u>Six Budget-Friendly Artificial Intelligence Options</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/study-smarter-not-harder-top-5-student-friendly-chatgpt-applications/"><u>Study Smarter, Not Harder: Top 5 Student-Friendly ChatGPT Applications</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/subtle-archiving-concealing-your-chatgpt-journey/"><u>Subtle Archiving: Concealing Your ChatGPT Journey</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/tailored-talk-tech-enhancing-gpt-conversation-with-10-tweaks/"><u>Tailored Talk Tech: Enhancing GPT Conversation with 10 Tweaks</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-art-of-chuckles-by-code-from-laptops-to-vpn-safeguarding/"><u>The Art of Chuckles by Code: From Laptops to VPN Safeguarding</u></a></li>
<li><a href="https://screen-activity-recording.techidaily.com/the-ultimate-alternative-review-to-sharex/"><u>The Ultimate Alternative Review to ShareX</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/top-5-ai-driven-counseling-bots-for-emotional-wellness/"><u>Top 5 AI-Driven Counseling Bots for Emotional Wellness</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/transforming-physical-training-through-gpt-interaction/"><u>Transforming Physical Training Through GPT Interaction</u></a></li>
<li><a href="https://some-tips.techidaily.com/unlock-the-potential-tutorial-on-enabling-speech-transcription-in-powerpoint-for-2024/"><u>Unlock the Potential  Tutorial on Enabling Speech Transcription in PowerPoint for 2024</u></a></li>
</ul></div>
