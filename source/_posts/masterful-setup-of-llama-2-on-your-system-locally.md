---
title: Masterful Setup of Llama 2 on Your System Locally
date: 2024-07-20T06:21:53.440Z
updated: 2024-07-21T06:21:53.440Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Masterful Setup of Llama 2 on Your System Locally
excerpt: This Article Describes Masterful Setup of Llama 2 on Your System Locally
thumbnail: https://thmb.techidaily.com/50ec9f96a3862eafb44f6037d6d07d4292a04cc1b5866ca0d81d1cb562971c20.jpg
---

## Masterful Setup of Llama 2 on Your System Locally

 Meta released Llama 2 in the summer of 2023\. The new version of Llama is fine-tuned with 40% more tokens than the original Llama model, doubling its context length and significantly outperforming other open-sourced models available. The fastest and easiest way to access Llama 2 is via an API through an online platform. However, if you want the best experience, installing and loading Llama 2 directly on your computer is best.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 With that in mind, we've created a step-by-step guide on how to use Text-Generation-WebUI to load a quantized Llama 2 LLM locally on your computer.

<!-- affiliate ads begin -->
<a href="https://ursime.pxf.io/c/5597632/2092236/16384" target="_top" id="2092236"><img src="//a.impactradius-go.com/display-ad/16384-2092236" border="0" alt="" width="1920" height="329"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2092236/16384" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://ephamedtechinc.pxf.io/c/5597632/2095369/26400" target="_top" id="2095369"><img src="//a.impactradius-go.com/display-ad/26400-2095369" border="0" alt="" width="1024" height="512"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2095369/26400" style="position:absolute;visibility:hidden;" border="0" />
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
<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2075471/7443" target="_top" id="2075471"><img src="//a.impactradius-go.com/display-ad/7443-2075471" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2075471/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
   ![Select operating system](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/4-select-operating-system.jpg)
3. Your anti-virus might create an alert; this is fine. The prompt is just an [antivirus false positive](https://www.makeuseof.com/what-is-antivirus-false-result/) for running a batch file or script. Click on **Run anyway**.
4. A terminal will open and start the setup. Early on, the setup will pause and ask you what GPU you are using. Select the appropriate type of GPU installed on your computer and hit enter. For those without a dedicated graphics card, select **None (I want to run models in CPU mode)**. Keep in mind that running on CPU mode is much slower when compared to running the model with a dedicated GPU.  
<!-- affiliate ads begin -->
<a href="https://purchase.swifdoo.com/order/checkout.php?PRODS=40002162&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/8b932759a5a04ddb34bf79e3f9072e4b/products/1_Product%20box%20white-1024x1024.png" border="0">SwifDoo PDF Perpetual (1 PC) Free upgrade. No monthly fees ever. 
</a>
<!-- affiliate ads end -->
![Selecting GPU hardware installed](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/5-select-gpu-settings.jpg)
5. Once the setup is complete, you can now launch Text-Generation-WebUI locally. You can do so by opening your preferred web browser and entering the provided IP address on the URL.  
<!-- affiliate ads begin -->
<a href="https://imp.i110150.net/c/5597632/924299/11305" target="_top" id="924299"><img src="//a.impactradius-go.com/display-ad/11305-924299" border="0" alt="" width="520" height="100"/></a>
<!-- affiliate ads end -->
![How to launch-Text-Generation-WebUI](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/6-launch-text-generation-webui.jpg)
6. The WebUI is now ready for use.  
![Text-Generation-WebUI](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/7-text-generation-webui-view.jpg)

 However, the program is only a model loader. Let's download Llama 2 for the model loader to launch.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2087389/7443" target="_top" id="2087389"><img src="//a.impactradius-go.com/display-ad/7443-2087389" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2087389/7443" style="position:absolute;visibility:hidden;" border="0" />
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

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=32667153&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.coolmuster.com/uploads/image/20201228/feature02.png" border="0"></a>
<!-- affiliate ads end -->
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
<li><a href="https://facebook-record-videos.techidaily.com/new-5-top-link-minimizers-transforming-youtube-watchability-for-2024/"><u>[New] 5-Top Link Minimizers Transforming YouTube Watchability for 2024</u></a></li>
<li><a href="https://digital-screen-recording.techidaily.com/new-expert-techniques-for-high-quality-xbox-screenshots-for-2024/"><u>[New] Expert Techniques for High-Quality Xbox Screenshots for 2024</u></a></li>
<li><a href="https://vimeo-videos.techidaily.com/new-in-2024-beyond-the-buzz-a-ranked-guide-to-non-vimeo-edits/"><u>[New] In 2024, Beyond the Buzz  A Ranked Guide to Non-Vimeo Edits</u></a></li>
<li><a href="https://snapchat-videos.techidaily.com/new-sonic-steps-to-better-snapchat-videos-for-2024/"><u>[New] Sonic Steps to Better Snapchat Videos for 2024</u></a></li>
<li><a href="https://extra-skills.techidaily.com/updated-reimagining-the-corporate-environment-to-maximize-employee-potential/"><u>[Updated] Reimagining the Corporate Environment to Maximize Employee Potential</u></a></li>
<li><a href="https://youtube-stream.techidaily.com/2024-approved-legality-check-taking-screencasts-of-youtube-videos/"><u>2024 Approved  Legality Check  Taking Screencasts of YouTube Videos</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ais-surge-the-quintessential-five-in-cybercrime-empowerment/"><u>AI's Surge: The Quintessential Five in Cybercrime Empowerment</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/assessing-machine-intelligence-beyond-traditional-trials/"><u>Assessing Machine Intelligence Beyond Traditional Trials</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/automated-prose-perfection-the-hix-way/"><u>Automated Prose Perfection: The HIX Way</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/balancing-ai-realism-six-key-cues-for-authentic-respitsonses/"><u>Balancing AI Realism: Six Key Cues for Authentic Respitsonses</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/bridge-to-everywheres-chatgpt-with-ease/"><u>Bridge to Everywhere's ChatGPT with Ease</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/enterprise-applications-of-chatgpt-explained/"><u>Enterprise Applications of ChatGPT Explained</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/harnessing-chatgpt-power-in-career-pursuits/"><u>Harnessing ChatGPT Power in Career Pursuits</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-generative-ai-fails-in-humanized-text-conversations/"><u>How Generative AI Fails in Humanized Text Conversations</u></a></li>
<li><a href="https://fake-location.techidaily.com/how-to-change-netflix-location-to-get-more-country-version-on-apple-iphone-12-mini-drfone-by-drfone-virtual-ios/"><u>How to Change Netflix Location to Get More Country Version On Apple iPhone 12 mini | Dr.fone</u></a></li>
<li><a href="https://location-social.techidaily.com/how-to-change-your-vivo-y27-5g-location-on-twitter-drfone-by-drfone-virtual-android/"><u>How to Change your Vivo Y27 5G Location on Twitter | Dr.fone</u></a></li>
<li><a href="https://fox-access.techidaily.com/in-2024-infuse-satire-and-smiles-kapwings-meme-builder/"><u>In 2024, Infuse Satire & Smiles - Kapwing's Meme Builder</u></a></li>
<li><a href="https://sound-tweaking.techidaily.com/in-2024-optimal-auto-tuneshop-with-mac-compatibility/"><u>In 2024, Optimal Auto Tuneshop with Mac Compatibility</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/inside-hugging-face-concept-and-applications/"><u>Inside Hugging Face: Concept & Applications</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/liberate-your-conversations-with-windows-freegpt/"><u>Liberate Your Conversations with Windows FreeGPT</u></a></li>
<li><a href="https://fake-location.techidaily.com/looking-for-a-location-changer-on-tecno-spark-10c-look-no-further-drfone-by-drfone-virtual-android/"><u>Looking For A Location Changer On Tecno Spark 10C? Look No Further | Dr.fone</u></a></li>
<li><a href="https://windows11.techidaily.com/neutralize-required-condition-red-flags-in-win11/"><u>Neutralize Required Condition Red Flags in Win11</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/protect-your-talking-secrets-the-top-3-bot-privacy-issues/"><u>Protect Your Talking Secrets: The Top 3 Bot Privacy Issues</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/restoring-full-chatgpt-functionality-fixing-key-obstacles/"><u>Restoring Full ChatGPT Functionality: Fixing Key Obstacles</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/talk-your-way-through-ai-mastering-chatgpt-via-vocal-commands/"><u>Talk Your Way Through AI: Mastering ChatGPT via Vocal Commands</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-ai-duel-assessing-notion-ai-against-openais-gpt-3/"><u>The AI Duel: Assessing Notion AI Against OpenAI's GPT-3</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-path-to-ingenious-visuals-mastery-over-microsofts-copilot/"><u>The Path to Ingenious Visuals: Mastery Over Microsoft's Copilot</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/triggering-gpt-alerts-for-detecting-con-art-ai-systems/"><u>Triggering GPT Alerts for Detecting Con Art AI Systems</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unleashing-ai-potential-browser-deployment-via-agentgpt/"><u>Unleashing AI Potential: Browser Deployment via AgentGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unlock-the-potential-of-your-cvs-use-chatgpt-for-cover-letters/"><u>Unlock the Potential of Your CVs: Use ChatGPT for Cover Letters</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unlocking-dall-es-potential-with-png-and-jpg-conversions/"><u>Unlocking DALL-E's Potential with PNG and JPG Conversions</u></a></li>
</ul></div>
