---
title: The Offline Operation Blueprint for Llama 2 Software
date: 2024-08-29T19:40:51.984Z
updated: 2024-08-30T19:40:51.984Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes The Offline Operation Blueprint for Llama 2 Software
excerpt: This Article Describes The Offline Operation Blueprint for Llama 2 Software
thumbnail: https://thmb.techidaily.com/3322edcb2b3700ce4baa5c0677a8f300e23dbf74c5228f8bd6ca0d33294791ed.png
---

## The Offline Operation Blueprint for Llama 2 Software

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
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4726960&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/5f4f7141b65a730b4efb0e0d51f63e94/products/forexrobotronbox.gif" border="0">Forex Robotron Basic Package</a>
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
<!-- affiliate ads begin -->
<a href="https://ephamedtechinc.pxf.io/c/5597632/2097467/26400?prodsku=B700" target="_top" id="2097467"><img src="//a.impactradius-go.com/display-ad/26400-2097467" border="0" alt="" width="640" height="640"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2097467/26400" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
4. A terminal will open and start the setup. Early on, the setup will pause and ask you what GPU you are using. Select the appropriate type of GPU installed on your computer and hit enter. For those without a dedicated graphics card, select **None (I want to run models in CPU mode)**. Keep in mind that running on CPU mode is much slower when compared to running the model with a dedicated GPU.  
![Selecting GPU hardware installed](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/5-select-gpu-settings.jpg)
5. Once the setup is complete, you can now launch Text-Generation-WebUI locally. You can do so by opening your preferred web browser and entering the provided IP address on the URL.  
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

![HuggingFace model naming convention](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/wm/2023/10/huggingface-model-naming-convention-1.jpg)

 In this example, the model can be identified as a medium-sized Llama 2 model trained on 13 billion parameters optimized for chat inferencing using a dedicated CPU.

 For those running on a dedicated GPU, choose a **GPTQ** model, while for those using a CPU, choose **GGML**. If you want to chat with the model like you would with ChatGPT, choose **chat**, but if you want to experiment with the model with its full capabilities, use the **standard** model. As for parameters, know that using bigger models will provide better results at the expense of performance. I would personally recommend you start with a 7B model. As for quantization, use q4, as it's only for inferencing.

**Download:**[GGML](https://huggingface.co/localmodels/Llama-2-7B-ggml/tree/main) (Free)

**Download:**[GPTQ](https://huggingface.co/localmodels/Llama-2-7B-Chat-GPTQ/tree/main) (Free)

 Now that you know what iteration of Llama 2 you need, go ahead and download the model you want.

 In my case, since I'm running this on an ultrabook, I'll be using a GGML model fine-tuned for chat, **llama-2-7b-chat-ggmlv3.q4\_K\_S.bin.**

![Downloading Llama 2 model of your preference](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/8-download-llama-2-model.jpg)

<!-- affiliate ads begin -->
<a href="https://united.elfm.net/c/5597632/517826/4704" target="_top" id="517826"><img src="//a.impactradius-go.com/display-ad/4704-517826" border="0" alt="" width="728" height="90"/></a><img height="0" width="0" src="https://united.elfm.net/i/5597632/517826/4704" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 After the download is finished, place the model in **text-generation-webui-main** \> **models**.

![Placing Llama 2 model to model folder](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/9-place-model-to-model-folder.jpg)

Now that you have your model downloaded and placed in the model folder, it's time to configure the model loader.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=45152810&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/842ca578342915ccb8ae069595ba7233/products/copy_bootit-ss1_178x139.jpg" border="0">The BootIt Collection covers multi-booting, partitioning, and disk imaging on traditional PC's using the standard BIOS and  newer PC's using UEFI.   The collection includes BootIt Bare Metal (BIBM) for standard BIOS systems and BootIt UEFI (BIU) for UEFI system. 
</a>
<!-- affiliate ads end -->
## Step 4: Configure Text-Generation-WebUI

 Now, let's begin the configuration phase.

1. Once again, open Text-Generation-WebUI by running the **start\_(your OS)** file (see the previous steps above).
2. On the tabs located above the GUI, click **Model.** Click the refresh button at the model dropdown menu and select your model.
3. Now click on the dropdown menu of the **Model loader** and select **AutoGPTQ** for those using a GTPQ model and **ctransformers** for those using a GGML model. Finally, click on **Load** to load your model.  
![Setting model loader](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/10-select-model-loader.jpg)
4. To use the model, open the Chat tab and start testing the model.  
<!-- affiliate ads begin -->
<a href="https://zonlipartnershipprogram.pxf.io/c/5597632/1821134/17882" target="_top" id="1821134"><img src="//a.impactradius-go.com/display-ad/17882-1821134" border="0" alt="" width="320" height="250"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1821134/17882" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![Testing Llama 2 locally](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/12-testing-llama-2-locally.jpg)

 Congratulations, you've successfully loaded Llama2 on your local computer!

<!-- affiliate ads begin -->
<a href="https://25home.pxf.io/c/5597632/2090698/16836" target="_top" id="2090698"><img src="//a.impactradius-go.com/display-ad/16836-2090698" border="0" alt="" width="720" height="300"/></a>
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
<li><a href="https://youtube-tips.techidaily.com/024-approved-turbocharge-your-youtube-videos-swift-render-and-transfer-strategies/"><u>[New] 2024 Approved  Turbocharge Your YouTube Videos  Swift Render & Transfer Strategies</u></a></li>
<li><a href="https://fox-boxes.techidaily.com/new-in-2024-access-all-movies-ioss-no1-freepluspaid-film-apps-guide/"><u>[New] In 2024, Access All Movies  IOS's No.1, FREE+Paid Film Apps Guide</u></a></li>
<li><a href="https://facebook-video-files.techidaily.com/new-mastering-automatic-youtube-playback-on-social-media-hubs-for-2024/"><u>[New] Mastering Automatic YouTube Playback on Social Media Hubs for 2024</u></a></li>
<li><a href="https://video-screen-grab.techidaily.com/new-personalize-where-mac-pics-save-for-2024/"><u>[New] Personalize Where Mac Pics Save for 2024</u></a></li>
<li><a href="https://facebook-clips.techidaily.com/updated-in-2024-prolific-performance-our-picks-for-top-8-workflow-planners/"><u>[Updated] In 2024, Prolific Performance  Our Picks for Top 8 Workflow Planners</u></a></li>
<li><a href="https://vimeo-videos.techidaily.com/updated-vimeo-star-moment-analysis/"><u>[Updated] Vimeo Star Moment Analysis</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/accelerate-compatibility-with-simple-intel-nuc-driver-instructions/"><u>Accelerate Compatibility with Simple Intel NUC Driver Instructions</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-leader-replaced-impact-on-gpts-future/"><u>AI Leader Replaced: Impact on GPT's Future</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-driven-bing-unveiled-by-microsoft/"><u>AI-Driven Bing Unveiled by Microsoft</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/bypassing-the-allure-of-a-chatgpt-app-factor/"><u>Bypassing the Allure of a ChatGPT App Factor</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/clearing-your-conversations-with-chatgpt/"><u>Clearing Your Conversations with ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/content-reinvention-with-chatgpts-innovations/"><u>Content Reinvention with ChatGPT's Innovations</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/content-writing-made-simple-top-8-ai-tools-reviewed/"><u>Content Writing Made Simple: Top 8 AI Tools Reviewed</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/default-plugins-for-chatgpt-explored/"><u>Default Plugins for ChatGPT Explored</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/here-are-some-pro-tips-for-pokemon-go-pvp-battles-on-infinix-smart-8-drfone-by-drfone-virtual-android/"><u>Here are Some Pro Tips for Pokemon Go PvP Battles On Infinix Smart 8 | Dr.fone</u></a></li>
<li><a href="https://ios-pokemon-go.techidaily.com/how-do-you-get-sun-stone-evolutions-in-pokemon-for-apple-iphone-6-drfone-by-drfone-virtual-ios/"><u>How Do You Get Sun Stone Evolutions in Pokémon For Apple iPhone 6? | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/i-gave-the-same-creative-prompt-to-3-different-chatbots-which-one-did-it-best/"><u>I Gave the Same Creative Prompt to 3 Different Chatbots: Which One Did It Best?</u></a></li>
<li><a href="https://some-approaches.techidaily.com/in-2024-the-ultimate-roadmap-to-unearth-gorgeous-pexel-pictures/"><u>In 2024, The Ultimate Roadmap to Unearth Gorgeous Pexel Pictures</u></a></li>
<li><a href="https://android-location-track.techidaily.com/in-2024-ways-to-stop-parent-tracking-your-samsung-galaxy-z-fold-5-drfone-by-drfone-virtual-android/"><u>In 2024, Ways to stop parent tracking your Samsung Galaxy Z Fold 5 | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/is-using-gpt-plugins-secure/"><u>Is Using GPT Plugins Secure?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/quintuple-facilitators-ais-acceleration-of-cybercriminal-endeavors/"><u>Quintuple Facilitators: AI's Acceleration of Cybercriminal Endeavors</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/skepticism-towards-zerogpt-and-detectors-rises/"><u>Skepticism Towards ZeroGPT & Detectors Rises</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-hidden-applications-where-gpt-shines/"><u>The Hidden Applications Where GPT Shines</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-quora-poe-blueprint-for-ai-conversation/"><u>The Quora PoE Blueprint for AI Conversation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/tracing-the-origins-and-aims-of-nlp-and-ml/"><u>Tracing the Origins and Aims of NLP & ML</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/transform-your-kitchen-skills-with-7-ai-powered-steps/"><u>Transform Your Kitchen Skills with 7 AI-Powered Steps</u></a></li>
<li><a href="https://sound-issues.techidaily.com/troubleshooting-silent-pc-speakers-fixing-audio-issues-in-windows-11/"><u>Troubleshooting Silent PC Speakers: Fixing Audio Issues in Windows 11</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/understanding-the-censorship-mechanisms-in-your-virtual-assistants/"><u>Understanding the Censorship Mechanisms in Your Virtual Assistants</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unleashing-ai-potential-5-free-graphic-makers/"><u>Unleashing AI Potential: 5 Free Graphic Makers</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unlocking-vs-code-potential-with-codegpt/"><u>Unlocking VS Code Potential with CodeGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/winning-job-applications-with-advanced-ai-for-resumes/"><u>Winning Job Applications with Advanced AI for Resumes</u></a></li>
</ul></div>
