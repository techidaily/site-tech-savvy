---
title: Essential Steps to Install Llama 2 Locally
date: 2024-08-03T00:54:10.562Z
updated: 2024-08-04T00:54:10.562Z
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
<li><a href="https://screen-capture.techidaily.com/new-2024-approved-combating-an-unresponsive-obs-camera-input-stream/"><u>[New] 2024 Approved  Combating an Unresponsive OBS Camera Input Stream</u></a></li>
<li><a href="https://youtube-blog.techidaily.com/024-approved-unraveling-the-secrets-of-viral-content-creation/"><u>[New] 2024 Approved  Unraveling the Secrets of Viral Content Creation</u></a></li>
<li><a href="https://twitter-videos.techidaily.com/new-chuckles-and-cheers-top-tweets-saver-with-gif/"><u>[New] Chuckles & Cheers  Top Tweets Saver with GIF</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/new-ranking-moba-titles-exclusively-for-android-phones-for-2024/"><u>[New] Ranking MOBA Titles Exclusively for Android Phones for 2024</u></a></li>
<li><a href="https://snapchat-videos.techidaily.com/new-snap-income-trends-in-making-money-on-social-media-for-2024/"><u>[New] Snap Income  Trends in Making Money on Social Media for 2024</u></a></li>
<li><a href="https://facebook-video-content.techidaily.com/updated-2024-approved-maximizing-view-count-for-facebook-videos/"><u>[Updated] 2024 Approved  Maximizing View Count for Facebook Videos</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/updated-in-2024-innovative-approaches-to-powerpoint-video-capture/"><u>[Updated] In 2024, Innovative Approaches to PowerPoint Video Capture</u></a></li>
<li><a href="https://snapchat-videos.techidaily.com/updated-quick-start-to-engaging-in-face-to-face-conversations-on-snapchat/"><u>[Updated] Quick Start to Engaging in Face-to-Face Conversations on Snapchat</u></a></li>
<li><a href="https://fox-blue.techidaily.com/2024-approved-captivating-viewers-with-visuals-picture-upload-tips/"><u>2024 Approved  Captivating Viewers with Visuals  Picture Upload Tips</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/7-strategies-from-palm-2-for-a-better-bard-experience/"><u>7 Strategies From PaLM 2 for a Better Bard Experience</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-content-detectors-dont-work-and-thats-a-big-problem/"><u>AI Content Detectors Don’t Work, and That’s a Big Problem</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-rivalry-unique-approach-to-shared-creative-task/"><u>AI Rivalry: Unique Approach to Shared Creative Task</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-showdown-unveiling-the-powers-of-forefront-ai-vs-chatgpt/"><u>AI Showdown: Unveiling the Powers of Forefront AI vs ChatGPT</u></a></li>
<li><a href="https://mondly-stories.techidaily.com/beginners-insights-into-german-letter-forms/"><u>Beginners' Insights Into German Letter Forms</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/beware-generative-ais-disinformation-capabilities/"><u>Beware: Generative AI's Disinformation Capabilities</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/boost-well-being-8-cutting-edge-ai-fitness-tools/"><u>Boost Well-Being: 8 Cutting-Edge AI Fitness Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgptplus-revolutionary-tech-for-fluent-multilingualism/"><u>ChatGPT+: Revolutionary Tech for Fluent Multilingualism</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/counteracting-text-slyness-openais-anti-deception-ai/"><u>Counteracting Text Slyness: OpenAI's Anti-Deception AI</u></a></li>
<li><a href="https://fox-access.techidaily.com/cross-service-playlist-exchange-simplified-for-2024/"><u>Cross-Service Playlist Exchange Simplified for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/cutting-edge-image-design-mastering-microsofts-copilot-capabilities/"><u>Cutting-Edge Image Design: Mastering Microsoft's Copilot Capabilities</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/discovering-11-powerful-gpt-strategies-for-authenticity-in-fiction/"><u>Discovering 11 Powerful GPT Strategies for Authenticity in Fiction</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/enhance-your-reading-journey-top-5-ai-enhanced-book-platforms/"><u>Enhance Your Reading Journey - Top 5 AI-Enhanced Book Platforms</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/enhancing-employment-skills-with-these-6-chatgpt-uses/"><u>Enhancing Employment Skills with These 6 ChatGPT Uses</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/exploring-predictive-ai-techniques-and-processes-involved/"><u>Exploring Predictive AI: Techniques and Processes Involved</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-fix-the-chatgpt-is-at-capacity-right-now-error-on-windows/"><u>How to Fix the ChatGPT Is at Capacity Right Now Error on Windows</u></a></li>
<li><a href="https://android-location-track.techidaily.com/how-to-track-meizu-21-location-by-number-drfone-by-drfone-virtual-android/"><u>How to Track Meizu 21 Location by Number | Dr.fone</u></a></li>
<li><a href="https://youtube-help.techidaily.com/in-2024-stepwise-strategy-creating-effective-youtube-subscriber-buttons/"><u>In 2024, Stepwise Strategy  Creating Effective YouTube Subscriber Buttons</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/in-2024-the-complete-igtv-user-manual/"><u>In 2024, The Complete IGTV User Manual</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/openais-approach-to-advanced-arithmetic/"><u>OpenAI's Approach to Advanced Arithmetic</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/optimizing-dietary-habits-using-ai-insights/"><u>Optimizing Dietary Habits Using AI Insights</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/reimagining-ai-scrutiny-post-turing-test-paradigm-shift/"><u>Reimagining AI Scrutiny Post-Turing Test Paradigm Shift</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/streamlined-ai-for-optimal-results-with-bing-android-edition/"><u>Streamlined AI for Optimal Results with Bing, Android Edition</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-dual-edge-of-ai-on-mental-health-services/"><u>The Dual Edge of AI on Mental Health Services</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/top-5-uses-for-tailored-chatgpt-guidance/"><u>Top 5 Uses for Tailored ChatGPT Guidance</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unlocking-the-power-of-chatgpt-in-multiple-languages/"><u>Unlocking the Power of ChatGPT in Multiple Languages</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-the-five-mechanisms-ais-boost-to-malicious-online-activities/"><u>Unveiling the Five Mechanisms: AI's Boost to Malicious Online Activities</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/visual-expertise-on-demand-harnessing-chatgpts-ai-scope/"><u>Visual Expertise on Demand: Harnessing ChatGPT’s AI Scope</u></a></li>
</ul></div>
