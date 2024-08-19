---
title: "Download & Deploy Llama 2: An Easy-to-Follow Manual"
date: 2024-08-18T09:58:41.382Z
updated: 2024-08-19T09:58:41.382Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Download & Deploy Llama 2: An Easy-to-Follow Manual"
excerpt: "This Article Describes Download & Deploy Llama 2: An Easy-to-Follow Manual"
thumbnail: https://thmb.techidaily.com/4cc1197e18d9544b2124a65bfec1efb521b06ec232353dd58129a9184ba8b76a.jpg
---

## Download & Deploy Llama 2: An Easy-to-Follow Manual

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
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4709458&QTY=1&AFFILIATE=108875&CART=1"><img src="https://3d-kstudio.com/wp-content/uploads/2019/10/Project-Manager-version-3-1600x900-768x419.jpg" border="0">Project Manager - Asset Browser for 3Ds Max</a>
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
<!-- affiliate ads begin -->
<a href="https://store.nero.com/order/checkout.php?PRODS=39694080&QTY=1&AFFILIATE=108875&CART=1"><img src="http://cdnwww.nero.com/nero-com-wAssets/img/banners/2023/nbr/fire/Screenshot_1red_gb.jpg" border="0">Nero Burning ROM:
The ultimate burning program for all your needs!</a>
<!-- affiliate ads end -->
![Text-Generation-WebUI](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/7-text-generation-webui-view.jpg)

<!-- affiliate ads begin -->
<a href="https://twopages.pxf.io/c/5597632/1873313/18544" target="_top" id="1873313"><img src="//a.impactradius-go.com/display-ad/18544-1873313" border="0" alt="" width="1080" height="1263"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1873313/18544" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 However, the program is only a model loader. Let's download Llama 2 for the model loader to launch.

<!-- affiliate ads begin -->
<a href="https://dhgate.sjv.io/c/5597632/1678785/12108" target="_top" id="1678785"><img src="//a.impactradius-go.com/display-ad/12108-1678785" border="0" alt="" width="300" height="250"/></a>
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

<!-- affiliate ads begin -->
<a href="https://engwe.pxf.io/c/5597632/2093504/25579" target="_top" id="2093504"><img src="//a.impactradius-go.com/display-ad/25579-2093504" border="0" alt="" width="1200" height="1200"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2093504/25579" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
Now that you have your model downloaded and placed in the model folder, it's time to configure the model loader.

## Step 4: Configure Text-Generation-WebUI

 Now, let's begin the configuration phase.

1. Once again, open Text-Generation-WebUI by running the **start\_(your OS)** file (see the previous steps above).
2. On the tabs located above the GUI, click **Model.** Click the refresh button at the model dropdown menu and select your model.
3. Now click on the dropdown menu of the **Model loader** and select **AutoGPTQ** for those using a GTPQ model and **ctransformers** for those using a GGML model. Finally, click on **Load** to load your model.  
![Setting model loader](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/10-select-model-loader.jpg)
4. To use the model, open the Chat tab and start testing the model.  
![Testing Llama 2 locally](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/12-testing-llama-2-locally.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.textstudio.com/order/checkout.php?PRODS=35633281&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/d6eb8222c9718486bdabce8b897380f7/products/2_premium-icon.png" border="0"> Take advantage of PREMIUM features. 
Create your texts / logos without any limitation. 
No attribution required when downloading. 
No advertising on the website. 
 TextStudio.com  PREMIUM - Monthly Membership</a>
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
<li><a href="https://facebook-video-footage.techidaily.com/new-2024-approved-earning-insights-from-viewing-data-on-youtube/"><u>[New] 2024 Approved  Earning Insights From Viewing Data on YouTube</u></a></li>
<li><a href="https://eaxpv-info.techidaily.com/new-2024-approved-from-chat-room-to-screen-step-by-step-google-meet-youtube-streams/"><u>[New] 2024 Approved  From Chat Room to Screen  Step-by-Step Google Meet YouTube Streams</u></a></li>
<li><a href="https://desktop-recording.techidaily.com/new-capturing-gaming-moments-look-beyond-xboxs-game-bar/"><u>[New] Capturing Gaming Moments  Look Beyond Xbox's Game Bar</u></a></li>
<li><a href="https://twitter-videos.techidaily.com/new-echoes-in-the-stream-full-year-tweet-video-analysis/"><u>[New] Echoes in the Stream - Full Year Tweet Video Analysis</u></a></li>
<li><a href="https://youtube-zero.techidaily.com/ed-2024-approved-unleashing-potential-the-ultimate-pathway-to-effective-youtube-banners/"><u>[Updated] 2024 Approved  Unleashing Potential  The Ultimate Pathway to Effective YouTube Banners</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/updated-chart-your-course-to-youtube-success-with-these-techniques-for-2024/"><u>[Updated] Chart Your Course to YouTube Success with These Techniques for 2024</u></a></li>
<li><a href="https://extra-lessons.techidaily.com/updated-crafting-professional-edits-including-sounds-in-premiere-projects/"><u>[Updated] Crafting Professional Edits  Including Sounds in Premiere Projects</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/updated-direct-to-your-library-simple-windows-and-mac-techniques-for-downloading-igtv-for-2024/"><u>[Updated] Direct to Your Library  Simple Windows & Mac Techniques for Downloading IGTV for 2024</u></a></li>
<li><a href="https://video-capture.techidaily.com/updated-in-2024-the-ultimate-guide-to-capturing-professional-quality-in-zoom-podcasts/"><u>[Updated] In 2024, The Ultimate Guide to Capturing Professional Quality in Zoom Podcasts</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/updated-in-2024-unveiling-the-mysteries-of-ig-metrics-an-essential-toolkit-for-marketers/"><u>[Updated] In 2024, Unveiling the Mysteries of IG Metrics  An Essential Toolkit for Marketers</u></a></li>
<li><a href="https://facebook-clips.techidaily.com/updated-seeking-entertainment-a-guide-to-watching-fb-videos-for-2024/"><u>[Updated] Seeking Entertainment  A Guide to Watching FB Videos for 2024</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/updated-straightforward-methods-to-save-insta-story-videos-for-2024/"><u>[Updated] Straightforward Methods to Save Insta Story Videos for 2024</u></a></li>
<li><a href="https://extra-skills.techidaily.com/2024-approved-stellar-stories-celebrating-youtubes-best-narratives/"><u>2024 Approved  Stellar Stories  Celebrating YouTube's Best Narratives</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-infused-harmonies-mastering-sounds-via-chatgpt/"><u>AI-Infused Harmonies: Mastering Sounds via ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/bank-data-at-risk-the-role-of-gpt-in-todays-cyber-threats/"><u>Bank Data at Risk? The Role of GPT in Today's Cyber Threats</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/bing-the-brainiac-search-engine/"><u>Bing, The Brainiac Search Engine</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-powered-guide-to-youtube-video-script-creation/"><u>ChatGPT-Powered Guide to YouTube Video Script Creation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/code-mastery-for-effective-gpt-3-integration/"><u>Code Mastery for Effective GPT-3 Integration</u></a></li>
<li><a href="https://ai-vdieo-software.techidaily.com/create-stunning-collages-best-web-based-photo-and-video-editors/"><u>Create Stunning Collages Best Web-Based Photo and Video Editors</u></a></li>
<li><a href="https://extra-tips.techidaily.com/cutting-edge-online-resources-for-glittering-3d-typography/"><u>Cutting-Edge Online Resources for Glittering 3D Typography</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/deciphering-the-turing-tests-implications-and-future-victors/"><u>Deciphering The Turing Test's Implications & Future Victors</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/designing-balanced-dietary-patterns-with-gpt-aid/"><u>Designing Balanced Dietary Patterns with GPT Aid</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/dodging-ai-crafted-windows-11-keys-a-good-practice/"><u>Dodging AI-Crafted Windows 11 Keys: A Good Practice</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/from-concept-to-creation-mastering-ai-image-generation-with-copilot/"><u>From Concept to Creation: Mastering AI Image Generation with Copilot</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/full-guide-on-mirroring-your-vivo-y78plus-to-your-pcmac-drfone-by-drfone-android/"><u>Full Guide on Mirroring Your Vivo Y78+ to Your PC/Mac | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/global-relevance-of-latest-chatgpt-info/"><u>Global Relevance of Latest ChatGPT Info</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/gpt-4-unlocked-innovative-no-cost-access-techniques/"><u>GPT-4 Unlocked: Innovative, No-Cost Access Techniques</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/harnessing-virtual-discussions-with-gpt-3-expertise/"><u>Harnessing Virtual Discussions with GPT-3 Expertise</u></a></li>
<li><a href="https://android-location-track.techidaily.com/how-to-check-distance-and-radius-on-google-maps-for-your-oppo-find-x7-drfone-by-drfone-virtual-android/"><u>How to Check Distance and Radius on Google Maps For your Oppo Find X7 | Dr.fone</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/how-to-screen-mirroring-oneplus-nord-n30-se-to-pc-drfone-by-drfone-android/"><u>How to Screen Mirroring OnePlus Nord N30 SE to PC? | Dr.fone</u></a></li>
<li><a href="https://bypass-frp.techidaily.com/in-2024-hassle-free-ways-to-remove-frp-lock-from-google-pixel-8-pro-phones-withwithout-a-pc-by-drfone-android/"><u>In 2024, Hassle-Free Ways to Remove FRP Lock from Google Pixel 8 Pro Phones with/without a PC</u></a></li>
<li><a href="https://review-topics.techidaily.com/in-2024-how-to-change-xiaomi-redmi-a2plus-location-on-skout-drfone-by-drfone-virtual-android/"><u>In 2024, How to Change Xiaomi Redmi A2+ Location on Skout | Dr.fone</u></a></li>
<li><a href="https://ai-vdieo-software.techidaily.com/in-2024-top-5-best-free-flv-video-editors/"><u>In 2024, Top 5 Best Free FLV Video Editors</u></a></li>
<li><a href="https://android-location-track.techidaily.com/in-2024-top-5-tracking-apps-to-track-samsung-galaxy-a15-4g-without-them-knowing-drfone-by-drfone-virtual-android/"><u>In 2024, Top 5 Tracking Apps to Track Samsung Galaxy A15 4G without Them Knowing | Dr.fone</u></a></li>
<li><a href="https://some-approaches.techidaily.com/in-2024-ultimate-acceleration-manual-boosting-fb-video-speed-with-top-tools/"><u>In 2024, Ultimate Acceleration Manual  Boosting FB Video Speed with Top Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/innovative-programming-enhancements-without-chatgpt/"><u>Innovative Programming Enhancements Without ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/is-trust-in-truthgpt-coin-justified/"><u>Is Trust in TruthGPT Coin Justified?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-chatgpt-a-guide-to-academic-writing/"><u>Mastering ChatGPT: A Guide to Academic Writing</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-chatgpt-an-openai-guide/"><u>Mastering ChatGPT: An OpenAI Guide</u></a></li>
<li><a href="https://extra-skills.techidaily.com/maximum-capacity-choices-ultimate-cloud-service-list-for-2024/"><u>Maximum Capacity Choices  Ultimate Cloud Service List for 2024</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/novices-path-to-professional-gopro-video-editing-for-2024/"><u>Novice's Path to Professional GoPro Video Editing for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/pilot-progressions-understanding-copilot-enhancements/"><u>Pilot Progressions: Understanding CoPilot Enhancements</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/proton-vpn-browser-extension-how-to-change-your-email-address-and-the-chatgpt-windows-app-is-fake/"><u>Proton VPN Browser Extension, How to Change Your Email Address, and the ChatGPT Windows App Is Fake</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/quick-fixes-for-stuck-chatgpt-apps-on-iphones/"><u>Quick Fixes for Stuck ChatGPT Apps on iPhones</u></a></li>
<li><a href="https://windows11.techidaily.com/resolving-boot-time-windows-audio-recovery-procedures/"><u>Resolving Boot-Time Windows Audio Recovery Procedures</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/script-revolution-unlocking-creativity-with-chatgpt-in-gaming/"><u>Script Revolution: Unlocking Creativity with ChatGPT in Gaming</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/skepticism-grows-over-zerogpt-and-detection-tools/"><u>Skepticism Grows Over ZeroGPT & Detection Tools</u></a></li>
<li><a href="https://printer-issues.techidaily.com/techniques-to-disable-networked-printers-in-windows/"><u>Techniques to Disable Networked Printers in Windows</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-anatomy-of-extraordinary-llm-systems/"><u>The Anatomy of Extraordinary LLM Systems</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-dawn-of-advanced-ai-googles-launch-of-palm-2-model/"><u>The Dawn of Advanced AI: Google's Launch of PaLM 2 Model</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-future-of-gaming-ais-role-in-game-development/"><u>The Future of Gaming: AI's Role in Game Development</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-future-unfolds-top-features-of-newest-gpt-release/"><u>The Future Unfolds: Top Features of Newest GPT Release</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-the-potential-of-gpt-with-android/"><u>Unveiling the Potential of GPT with Android</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/your-guide-to-understanding-and-using-claude-3/"><u>Your Guide to Understanding and Using Claude 3</u></a></li>
</ul></div>
