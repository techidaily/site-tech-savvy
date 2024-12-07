---
title: In-Depth Steps to Running Llama 2 Locally on Your Device
date: 2024-12-01T16:27:57.504Z
updated: 2024-12-06T18:22:51.862Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes In-Depth Steps to Running Llama 2 Locally on Your Device
excerpt: This Article Describes In-Depth Steps to Running Llama 2 Locally on Your Device
thumbnail: https://thmb.techidaily.com/66485902527c2f60d68ff1756c39d95b2b9ff2d6a92e3e5c77cff27210813f40.jpg
---

## In-Depth Steps to Running Llama 2 Locally on Your Device

 Meta released Llama 2 in the summer of 2023\. The new version of Llama is fine-tuned with 40% more tokens than the original Llama model, doubling its context length and significantly outperforming other open-sourced models available. The fastest and easiest way to access Llama 2 is via an API through an online platform. However, if you want the best experience, installing and loading Llama 2 directly on your computer is best.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 With that in mind, we've created a step-by-step guide on how to use Text-Generation-WebUI to load a quantized Llama 2 LLM locally on your computer.

>  Disclaimer: This post includes affiliate links
>
>  If you click on a link and make a purchase, I may receive a commission at no extra cost to you.
>

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
4. A terminal will open and start the setup. Early on, the setup will pause and ask you what GPU you are using. Select the appropriate type of GPU installed on your computer and hit enter. For those without a dedicated graphics card, select **None (I want to run models in CPU mode)**. Keep in mind that running on CPU mode is much slower when compared to running the model with a dedicated GPU.  
![Selecting GPU hardware installed](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/5-select-gpu-settings.jpg)
5. Once the setup is complete, you can now launch Text-Generation-WebUI locally. You can do so by opening your preferred web browser and entering the provided IP address on the URL.  

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/Iz2LYWd8EqI?si=G_3CqFRAmeVPczjj" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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

![HuggingFace model naming convention](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/wm/2023/10/huggingface-model-naming-convention-1.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/E3yY7lZ-FKA?si=g8VEuExP8GH59B69" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 In this example, the model can be identified as a medium-sized Llama 2 model trained on 13 billion parameters optimized for chat inferencing using a dedicated CPU.

 For those running on a dedicated GPU, choose a **GPTQ** model, while for those using a CPU, choose **GGML**. If you want to chat with the model like you would with ChatGPT, choose **chat**, but if you want to experiment with the model with its full capabilities, use the **standard** model. As for parameters, know that using bigger models will provide better results at the expense of performance. I would personally recommend you start with a 7B model. As for quantization, use q4, as it's only for inferencing.

**Download:**[GGML](https://huggingface.co/localmodels/Llama-2-7B-ggml/tree/main) (Free)

**Download:**[GPTQ](https://huggingface.co/localmodels/Llama-2-7B-Chat-GPTQ/tree/main) (Free)

 Now that you know what iteration of Llama 2 you need, go ahead and download the model you want.

 In my case, since I'm running this on an ultrabook, I'll be using a GGML model fine-tuned for chat, **llama-2-7b-chat-ggmlv3.q4\_K\_S.bin.**

![Downloading Llama 2 model of your preference](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/8-download-llama-2-model.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/HSFNIAYChbA?si=4TIlsUrYmY5vP2il" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 After the download is finished, place the model in **text-generation-webui-main** \> **models**.

![Placing Llama 2 model to model folder](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/9-place-model-to-model-folder.jpg)

Now that you have your model downloaded and placed in the model folder, it's time to configure the model loader.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/Rxyki8-Y630?si=dHLkIxG59zdlZeN0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## Step 4: Configure Text-Generation-WebUI

 Now, let's begin the configuration phase.

1. Once again, open Text-Generation-WebUI by running the **start\_(your OS)** file (see the previous steps above).
2. On the tabs located above the GUI, click **Model.** Click the refresh button at the model dropdown menu and select your model.
3. Now click on the dropdown menu of the **Model loader** and select **AutoGPTQ** for those using a GTPQ model and **ctransformers** for those using a GGML model. Finally, click on **Load** to load your model.  
![Setting model loader](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/10-select-model-loader.jpg)
4. To use the model, open the Chat tab and start testing the model.  

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/HMuxjTCMX2E?si=ylRTMJuUstpjLsZc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

![Testing Llama 2 locally](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/12-testing-llama-2-locally.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/LaWcXdTn5SE?si=QbxEkX-4a17J5RVs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://tech-revival.techidaily.com/android-version-of-gemini-introduces-updated-live-chat-functionality-and-improved-overlay-assistant-tools/"><u>Android Version of Gemini Introduces Updated Live Chat Functionality and Improved Overlay Assistant Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/beyond-the-spotlight-discover-apples-most-impactful-yet-subtle-ai-innovation-at-wwdc/"><u>Beyond the Spotlight: Discover Apple's Most Impactful, Yet Subtle AI Innovation at WWDC</u></a></li>
<li><a href="https://win-tricks.techidaily.com/brace-yourself-managers-microsofts-latest-plan-is-causing-stir-and-discontent/"><u>Brace Yourself, Managers: Microsoft’s Latest Plan Is Causing Stir and Discontent</u></a></li>
<li><a href="https://hardware-tips.techidaily.com/effortlessly-overcome-the-blizzards-with-top-tier-electric-snow-blower-reviewed-for-cleveland-climates-zdnet/"><u>Effortlessly Overcome the Blizzards with Top-Tier Electric Snow Blower Reviewed for Cleveland Climates | ZDNET</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/exploring-language-models-bert-and-gpt-unveiled/"><u>Exploring Language Models: BERT & GPT Unveiled</u></a></li>
<li><a href="https://unlock-android.techidaily.com/forgotten-the-voicemail-password-of-xiaomi-redmi-note-12-4g-try-these-fixes-by-drfone-android/"><u>Forgotten The Voicemail Password Of Xiaomi Redmi Note 12 4G? Try These Fixes</u></a></li>
<li><a href="https://win-amazing.techidaily.com/get-the-newest-geforce-940mx-gpu-driver-for-your-pc-free-download/"><u>Get the Newest GeForce 940MX GPU Driver for Your PC - Free Download</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/get-your-apple-watch-series-9ultra-at-unbeatable-prices-before-sale-ends-a-buyers-guide-zdnet/"><u>Get Your Apple Watch Series 9/Ultra at Unbeatable Prices Before Sale Ends: A Buyer's Guide | ZDNET</u></a></li>
<li><a href="https://vimeo-videos.techidaily.com/in-2024-unveiling-the-secrets-of-video-captioning-in-vimeo/"><u>In 2024, Unveiling the Secrets of Video Captioning in Vimeo</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/in-2024-will-the-ipogo-get-you-banned-and-how-to-solve-it-on-vivo-y36i-drfone-by-drfone-virtual-android/"><u>In 2024, Will the iPogo Get You Banned and How to Solve It On Vivo Y36i | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/privacy-in-dialogue-bot-safeguarding-strategies/"><u>Privacy in Dialogue: Bot Safeguarding Strategies</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/simplifying-life-comparing-everyday-conversational-bots/"><u>Simplifying Life: Comparing Everyday Conversational Bots</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/struggling-with-your-iphones-battery-performance-after-ios-19-discover-these-7-helpful-tips-to-improve-it/"><u>Struggling with Your iPhone's Battery Performance After iOS 19? Discover These 7 Helpful Tips to Improve It</u></a></li>
<li><a href="https://novels-ebooks.techidaily.com/209776658-9781420963083-the-zodiac-and-the-salts-of-salvation/"><u>The Zodiac and the Salts of Salvation | Free Book</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unlock-the-full-potential-of-craft-your-definitive-step-by-step-macos-document-tool-tutorial-on-zdnet/"><u>Unlock the Full Potential of Craft - Your Definitive Step-by-Step macOS Document Tool Tutorial on ZDNet</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unlocking-pdf-insights-with-chatgpt-four-methods/"><u>Unlocking PDF Insights with ChatGPT: Four Methods</u></a></li>
<li><a href="https://facebook.techidaily.com/1719152836104-zucks-goat-a-monetary-metaphor-in-animal-form/"><u>Zuck's Goat: A Monetary Metaphor in Animal Form.</u></a></li>
</ul></div>

