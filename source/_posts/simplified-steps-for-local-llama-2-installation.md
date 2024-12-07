---
title: Simplified Steps for Local Llama 2 Installation
date: 2024-11-29T20:08:18.267Z
updated: 2024-12-06T22:39:02.201Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Simplified Steps for Local Llama 2 Installation
excerpt: This Article Describes Simplified Steps for Local Llama 2 Installation
thumbnail: https://thmb.techidaily.com/be8ed6a4e78ad75b0aa927e5deab19fb5e1ff02b9f258c0a63e3b6ef48739db7.jpg
---

## Simplified Steps for Local Llama 2 Installation

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

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/BmegThMdrJE?si=rILo1FJb9DgnPljV" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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
<iframe width="560" height="315" src="https://www.youtube.com/embed/1KKovVi9epE?si=EF7KA7b4KsEpWA-M" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

![Text-Generation-WebUI](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/7-text-generation-webui-view.jpg)

 However, the program is only a model loader. Let's download Llama 2 for the model loader to launch.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/yDuvbv0QOYI?si=byottcEM_Rrvi4EL" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/-G7cU8dYvuI?si=JaKqRcW6qq9CDvty" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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
<iframe width="560" height="315" src="https://www.youtube.com/embed/LeKJBWb6Jhk?si=AnViizAPiIT1YCRA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

Now that you have your model downloaded and placed in the model folder, it's time to configure the model loader.

## Step 4: Configure Text-Generation-WebUI

 Now, let's begin the configuration phase.

1. Once again, open Text-Generation-WebUI by running the **start\_(your OS)** file (see the previous steps above).
2. On the tabs located above the GUI, click **Model.** Click the refresh button at the model dropdown menu and select your model.
3. Now click on the dropdown menu of the **Model loader** and select **AutoGPTQ** for those using a GTPQ model and **ctransformers** for those using a GGML model. Finally, click on **Load** to load your model.  
![Setting model loader](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/10-select-model-loader.jpg)
4. To use the model, open the Chat tab and start testing the model.  

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/5FWCFI3f_cs?si=Kt2Onr_E4c616tbH" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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
<li><a href="https://instagram-clips.techidaily.com/new-2024-approved-insiders-look-at-top-earning-instagram-tactics/"><u>[New] 2024 Approved Insider's Look at Top Earning Instagram Tactics</u></a></li>
<li><a href="https://fox-boxes.techidaily.com/updated-2024-approved-from-novice-to-pro-your-snapseed-journey-starts-here/"><u>[Updated] 2024 Approved From Novice to Pro Your Snapseed Journey Starts Here</u></a></li>
<li><a href="https://youtube-docs.techidaily.com/ed-2024-approved-top-4-marvel-intro-makers-online/"><u>[Updated] 2024 Approved Top 4 Marvel Intro Makers Online</u></a></li>
<li><a href="https://fox-friendly.techidaily.com/updated-sky-high-insights-comprehensive-phantom-4-breakdown-for-2024/"><u>[Updated] Sky-High Insights Comprehensive Phantom 4 Breakdown for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-comprehensive-guide-sending-and-receiving-imessage-on-windows-os-tips/"><u>A Comprehensive Guide: Sending & Receiving iMessage on Windows OS - Tips</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/creating-captivating-presentations-through-the-magic-of-chatgpt/"><u>Creating Captivating Presentations Through the Magic of ChatGPT</u></a></li>
<li><a href="https://screen-sharing-recording.techidaily.com/elite-multiplatform-recorder-for-pcs/"><u>Elite Multiplatform Recorder for PCs</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/exploring-the-ipad-pro-embracing-apples-top-tier-tablet-that-defies-macbook-comparison-zdnet-insights/"><u>Exploring the IPad Pro: Embracing Apple's Top-Tier Tablet That Defies MacBook Comparison - ZDNet Insights</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/flying-future-understanding-the-proco-pilot-edge/"><u>Flying Future: Understanding the Proco Pilot Edge</u></a></li>
<li><a href="https://smart-video-editing.techidaily.com/new-in-2024-how-to-get-filmora-for-free-with-the-proceeding-guide-you-can-now-get-the-full-version-of-filmora-for-free-on-your-device-without-crack-also-lea/"><u>New In 2024, How to Get Filmora for Free? With the Proceeding Guide, You Can Now Get the Full Version of Filmora for Free on Your Device without Crack. Also, Learn About some Wonderful Features of Filmora that Are a Must-Have</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/nutritionists-and-trainers-optimizing-ai-exchanges/"><u>Nutritionists and Trainers: Optimizing AI Exchanges</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/section-3b-five-factays-to-remember/"><u>Section 3B: Five Factays to Remember</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/top-10-social-media-tag-analyzers-fb-twt-and-insta/"><u>Top 10 Social Media Tag Analyzers FB, Twt & Insta</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/uncovering-genuine-chatbot-programming-on-ios/"><u>Uncovering Genuine ChatBot Programming on iOS</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unlock-the-secret-score-your-complimentary-macbook-air-m3-at-best-buy-with-these-steps-learn-more-inside/"><u>Unlock the Secret: Score Your Complimentary MacBook Air M3 at Best Buy with These Steps! Learn More Inside</u></a></li>
<li><a href="https://techno-recovery.techidaily.com/watch-the-matrix-franchise-properly-best-order-to-see-them/"><u>Watch The Matrix Franchise Properly: Best Order to See Them</u></a></li>
<li><a href="https://tech-haven.techidaily.com/why-the-leap-to-one-million-tokens-marks-a-pivotal-shift-in-gemini-turbocharged-performance/"><u>Why the Leap to One Million Tokens Marks a Pivotal Shift in Gemini Turbocharged Performance</u></a></li>
</ul></div>

