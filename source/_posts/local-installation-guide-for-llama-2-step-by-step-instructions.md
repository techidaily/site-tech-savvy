---
title: "Local Installation Guide for Llama 2: Step-by-Step Instructions"
date: 2024-08-10T02:15:40.760Z
updated: 2024-08-11T02:15:40.760Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Local Installation Guide for Llama 2: Step-by-Step Instructions"
excerpt: "This Article Describes Local Installation Guide for Llama 2: Step-by-Step Instructions"
thumbnail: https://thmb.techidaily.com/93d0d2f898ab9f2aada0c8c4eae12b5163704e3e0107a7a0c827d88713775503.png
---

## Local Installation Guide for Llama 2: Step-by-Step Instructions

 Meta released Llama 2 in the summer of 2023\. The new version of Llama is fine-tuned with 40% more tokens than the original Llama model, doubling its context length and significantly outperforming other open-sourced models available. The fastest and easiest way to access Llama 2 is via an API through an online platform. However, if you want the best experience, installing and loading Llama 2 directly on your computer is best.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 With that in mind, we've created a step-by-step guide on how to use Text-Generation-WebUI to load a quantized Llama 2 LLM locally on your computer.

<!-- affiliate ads begin -->
<a href="https://zonlipartnershipprogram.pxf.io/c/5597632/1596691/17882" target="_top" id="1596691"><img src="//a.impactradius-go.com/display-ad/17882-1596691" border="0" alt="" width="728" height="90"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1596691/17882" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Why Install Llama 2 Locally

 There are many reasons why people choose to run Llama 2 directly. Some do it for privacy concerns, some for customization, and others for offline capabilities. If you're researching, fine-tuning, or integrating Llama 2 for your projects, then accessing Llama 2 via API might not be for you. The point of running an LLM locally on your PC is to reduce reliance on [third-party AI tools](https://www.makeuseof.com/best-ai-web-apps/) and use AI anytime, anywhere, without worrying about leaking potentially sensitive data to companies and other organizations.

 With that said, let's begin with the step-by-step guide to installing Llama 2 locally.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2087267/19272" target="_top" id="2087267"><img src="//a.impactradius-go.com/display-ad/19272-2087267" border="0" alt="" width="728" height="90"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2087267/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Step 1: Install Visual Studio 2019 Build Tool

 To simplify things, we will use a one-click installer for Text-Generation-WebUI (the program used to load Llama 2 with GUI). However, for this installer to work, you need to download the Visual Studio 2019 Build Tool and install the necessary resources.

**Download:**[Visual Studio 2019](https://learn.microsoft.com/en-us/visualstudio/releases/2019/release-notes) (Free)

1. Go ahead and download the community edition of the software.
2. Now install Visual Studio 2019, then open the software. Once opened, tick the box on **Desktop development with C++** and hit install.  
<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4940317&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/333ac5d90817d69113471fbb6e531bee/sps-partnership-728x90eng.png" border="0"></a>
<!-- affiliate ads end -->
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
4. A terminal will open and start the setup. Early on, the setup will pause and ask you what GPU you are using. Select the appropriate type of GPU installed on your computer and hit enter. For those without a dedicated graphics card, select **None (I want to run models in CPU mode)**. Keep in mind that running on CPU mode is much slower when compared to running the model with a dedicated GPU.  
![Selecting GPU hardware installed](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/5-select-gpu-settings.jpg)
5. Once the setup is complete, you can now launch Text-Generation-WebUI locally. You can do so by opening your preferred web browser and entering the provided IP address on the URL.  
![How to launch-Text-Generation-WebUI](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/6-launch-text-generation-webui.jpg)
6. The WebUI is now ready for use.  
<!-- affiliate ads begin -->
<a href="https://ukaidot.sjv.io/c/5597632/1793234/19578" target="_top" id="1793234"><img src="//a.impactradius-go.com/display-ad/19578-1793234" border="0" alt="" width="678" height="452"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1793234/19578" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![Text-Generation-WebUI](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/7-text-generation-webui-view.jpg)

 However, the program is only a model loader. Let's download Llama 2 for the model loader to launch.

<!-- affiliate ads begin -->
<a href="https://unicoeye.pxf.io/c/5597632/2084396/18498" target="_top" id="2084396"><img src="//a.impactradius-go.com/display-ad/18498-2084396" border="0" alt="" width="1920" height="700"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2084396/18498" style="position:absolute;visibility:hidden;" border="0" />
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
<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4728277&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/f7f07e7dab09533bc71247a5b29a7373/products/1_iDeviceMessageBox.png" border="0"></a>
<!-- affiliate ads end -->
![Setting model loader](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/10-select-model-loader.jpg)
4. To use the model, open the Chat tab and start testing the model.  
<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=174416&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.easygifanimator.net/images/gif-animator.png" border="0">Easy GIF Animator is a powerful animated GIF editor and the top tool for creating animated pictures, banners, buttons and GIF videos. You get extensive animation editing features, animation effects, unmatched image quality and optimization for the web. No other GIF animation software matches our features and ease of use, that's why Easy GIF Animator is so popular.</a>
<!-- affiliate ads end -->
![Testing Llama 2 locally](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/12-testing-llama-2-locally.jpg)

 Congratulations, you've successfully loaded Llama2 on your local computer!

<!-- affiliate ads begin -->
<a href="https://funwhole.sjv.io/c/5597632/1702887/17189" target="_top" id="1702887"><img src="//a.impactradius-go.com/display-ad/17189-1702887" border="0" alt="" width="1000" height="1000"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1702887/17189" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://twitter-videos.techidaily.com/new-crafting-winning-twitter-sponsored-content/"><u>[New] Crafting Winning Twitter Sponsored Content</u></a></li>
<li><a href="https://eaxpv-info.techidaily.com/new-guide-on-purging-stored-videos-from-youtube-watchlater-for-2024/"><u>[New] Guide on Purging Stored Videos From YouTube Watchlater for 2024</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/updated-2024-approved-the-ultimate-guide-to-understanding-and-leveraging-instagrams-reels/"><u>[Updated] 2024 Approved  The Ultimate Guide to Understanding and Leveraging Instagram's Reels</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/updated-from-novice-to-expert-perfecting-mac-audio-with-audacity-for-2024/"><u>[Updated] From Novice to Expert  Perfecting Mac Audio with Audacity for 2024</u></a></li>
<li><a href="https://twitter-clips.techidaily.com/updated-twitcast-audible-and-mp4-edition/"><u>[Updated] TwitCast  Audible & MP4 Edition</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/15-simple-ways-to-integrate-gpt-into-workflow/"><u>15 Simple Ways to Integrate GPT Into Workflow</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/5-integral-applications-of-ai-for-digital-criminals/"><u>5 Integral Applications of AI for Digital Criminals</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/6-chatgpt-prompt-mistakes-to-avoid/"><u>6 ChatGPT Prompt Mistakes to Avoid</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/6-hazards-to-consider-when-relying-on-ai-psychologists/"><u>6 Hazards to Consider When Relying on AI Psychologists</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/6-ways-to-make-chatgpt-your-perfect-dungeon-master-assistant/"><u>6 Ways to Make ChatGPT Your Perfect Dungeon Master Assistant</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/7-groundbreaking-tools-excluding-chatgpt-for-code-writing/"><u>7 Groundbreaking Tools Excluding ChatGPT for Code Writing</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/7-innovative-ways-chatgpt-elevates-cooking-experience/"><u>7 Innovative Ways ChatGPT Elevates Cooking Experience</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/7-modern-alternatives-matching-or-surpassing-gpts-mobile-feature-set/"><u>7 Modern Alternatives Matching or Surpassing GPT's Mobile Feature Set</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/7-online-tools-to-improve-your-prompt-engineering-skills/"><u>7 Online Tools to Improve Your Prompt Engineering Skills</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/7-pioneering-features-of-bard-excitingly-debuted-at-googles-2023-event/"><u>7 Pioneering Features of Bard, Excitingly Debuted at Google's 2023 Event</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/8-new-neural-network-wonders-beyond-chatgpts-horizon/"><u>8 New Neural Network Wonders Beyond ChatGPT’s Horizon</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/8-reasons-why-generative-ai-security-issues-will-only-worsen/"><u>8 Reasons Why Generative AI Security Issues Will Only Worsen</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/9-easy-steps-to-mend-your-mobile-minds-chatgpt-issues/"><u>9 Easy Steps to Mend Your Mobile Mind's ChatGPT Issues</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/9-keys-to-understanding-the-future-of-prompt-engineering-jobs/"><u>9 Keys to Understanding the Future of Prompt Engineering Jobs</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/9-superior-features-in-chatgpt-plus-membership/"><u>9 Superior Features in ChatGPT Plus Membership</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-clear-path-to-mastering-chatgpt/"><u>A Clear Path to Mastering ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-detailed-comparison-of-all-gpt-models/"><u>A Detailed Comparison of All GPT Models</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-guide-to-leveraging-chatgpt-in-your-companys-success/"><u>A Guide to Leveraging ChatGPT in Your Company's Success</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-guide-to-tranquility-with-gpt/"><u>A Guide to Tranquility with GPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721429893410-ballads-battleground-chatgpt-vs-shepherds-alpacas-unite/"><u>Ballads Battleground: ChatGPT vs Shepherds, Alpacas Unite</u></a></li>
<li><a href="https://extra-hints.techidaily.com/decoding-instagrams-music-copyright-doctrine/"><u>Decoding Instagram's Music Copyright Doctrine</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721427447705-emoji-cleared-tweets-linuss-leaks-revealed-trojan-truths-told-and-chatgpt-problems-unpacked/"><u>Emoji Cleared Tweets, Linus's Leaks Revealed, Trojan Truths Told, & ChatGPT Problems Unpacked</u></a></li>
<li><a href="https://twitter-videos.techidaily.com/fix-disruption-chromium-and-tweeted-videos/"><u>Fix Disruption  Chromium and Tweeted Videos</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721431297671-just-start-chatting-chatgpt-ready/"><u>Just Start Chatting - ChatGPT Ready</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721437336075-level-up-gaming-skills-with-these-top-chatgpt-games/"><u>Level Up Gaming Skills with These Top ChatGPT Games!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721430643520-pioneer-personal-text-artistry-with-openais-curated-gpt-shops/"><u>Pioneer Personal Text Artistry with OpenAI's Curated GPT Shops</u></a></li>
<li><a href="https://games-able.techidaily.com/quick-remedy-for-dxgierrordevicehunk-on-windows-1011/"><u>Quick Remedy for DXGI_ERROR_DEVICE_HUNK on Windows 10/11</u></a></li>
<li><a href="https://video-screen-grab.techidaily.com/rogelikes-past-present-and-emerging-futures/"><u>Rogelikes Past, Present, & Emerging Futures</u></a></li>
<li><a href="https://youtube-tips.techidaily.com/d-you-opt-for-a-compreayer-package-on-youtube-with-premium-features-in-2024/"><u>Should You Opt for a Compreayer Package on YouTube with Premium Features, In 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721424588761-streamline-your-search-with-bings-intelligent-ai-features/"><u>Streamline Your Search with Bing's Intelligent AI Features</u></a></li>
<li><a href="https://screen-recording.techidaily.com/unified-iptv-streaming-services/"><u>Unified IPTV Streaming Services</u></a></li>
</ul></div>
