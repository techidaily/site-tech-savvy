---
title: A Step-By-Step Process for Local Llama 2 Setup
date: 2024-08-03T01:01:48.631Z
updated: 2024-08-04T01:01:48.631Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes A Step-By-Step Process for Local Llama 2 Setup
excerpt: This Article Describes A Step-By-Step Process for Local Llama 2 Setup
thumbnail: https://thmb.techidaily.com/4740430244a268b3ae9a4b1e15c683b234a7cf8bdf323c545591ca9aaa0e0818.jpg
---

## A Step-By-Step Process for Local Llama 2 Setup

 Meta released Llama 2 in the summer of 2023\. The new version of Llama is fine-tuned with 40% more tokens than the original Llama model, doubling its context length and significantly outperforming other open-sourced models available. The fastest and easiest way to access Llama 2 is via an API through an online platform. However, if you want the best experience, installing and loading Llama 2 directly on your computer is best.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 With that in mind, we've created a step-by-step guide on how to use Text-Generation-WebUI to load a quantized Llama 2 LLM locally on your computer.

<!-- affiliate ads begin -->
<a href="https://store.nero.com/order/checkout.php?PRODS=4729507&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.nero.com/nero-com-wAssets/img/banners/2023/TIU/Nero_TuneItUp_Screen_2.webp" border="0">/a>
<!-- affiliate ads end -->
## Why Install Llama 2 Locally

 There are many reasons why people choose to run Llama 2 directly. Some do it for privacy concerns, some for customization, and others for offline capabilities. If you're researching, fine-tuning, or integrating Llama 2 for your projects, then accessing Llama 2 via API might not be for you. The point of running an LLM locally on your PC is to reduce reliance on [third-party AI tools](https://www.makeuseof.com/best-ai-web-apps/) and use AI anytime, anywhere, without worrying about leaking potentially sensitive data to companies and other organizations.

 With that said, let's begin with the step-by-step guide to installing Llama 2 locally.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=194977&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.blumentals.net/scrfactory/images/screensaver-software.png" border="0">Screensaver Factory, Create stunning professional screensavers within minutes. Create screensavers for yourself, for marketing or unlimited royalty-free commercial distribution. Make screensavers from images, video and swf flash, add background music and smooth sprite and transition effects. Screensaver Factory is very easy to use, and it enables you to make self-installing screensaver files and CDs for easy setup and distribution. Screensaver Factory is the most advanced software of its kind.</a>
<!-- affiliate ads end -->
## Step 1: Install Visual Studio 2019 Build Tool

 To simplify things, we will use a one-click installer for Text-Generation-WebUI (the program used to load Llama 2 with GUI). However, for this installer to work, you need to download the Visual Studio 2019 Build Tool and install the necessary resources.

**Download:**[Visual Studio 2019](https://learn.microsoft.com/en-us/visualstudio/releases/2019/release-notes) (Free)

1. Go ahead and download the community edition of the software.
2. Now install Visual Studio 2019, then open the software. Once opened, tick the box on **Desktop development with C++** and hit install.  
<!-- affiliate ads begin -->
<a href="https://bluettide.pxf.io/c/5597632/2042332/17092" target="_top" id="2042332"><img src="//a.impactradius-go.com/display-ad/17092-2042332" border="0" alt="BLUETTI NEW LAUNCH AC180T" width="960" height="900"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2042332/17092" style="position:absolute;visibility:hidden;" border="0" />
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
![Text-Generation-WebUI](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/7-text-generation-webui-view.jpg)

 However, the program is only a model loader. Let's download Llama 2 for the model loader to launch.

<!-- affiliate ads begin -->
<a href="https://propmoneyinc.pxf.io/c/5597632/1803116/14559" target="_top" id="1803116"><img src="//a.impactradius-go.com/display-ad/14559-1803116" border="0" alt="" width="859" height="859"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1803116/14559" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://ukaidot.sjv.io/c/5597632/1793233/19578" target="_top" id="1793233"><img src="//a.impactradius-go.com/display-ad/19578-1793233" border="0" alt="" width="1200" height="1200"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1793233/19578" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![Downloading Llama 2 model of your preference](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/8-download-llama-2-model.jpg)

 After the download is finished, place the model in **text-generation-webui-main** \> **models**.

![Placing Llama 2 model to model folder](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/9-place-model-to-model-folder.jpg)

Now that you have your model downloaded and placed in the model folder, it's time to configure the model loader.

<!-- affiliate ads begin -->
<a href="https://shop.copernic.com/order/checkout.php?PRODS=41033091&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.2checkout.com/images/merchant/8d30aa96e72440759f74bd2306c1fa3d/Copernic-2023-Affiliate-728x90-Advanced.png" border="0"></a>
<!-- affiliate ads end -->
## Step 4: Configure Text-Generation-WebUI

 Now, let's begin the configuration phase.

1. Once again, open Text-Generation-WebUI by running the **start\_(your OS)** file (see the previous steps above).
2. On the tabs located above the GUI, click **Model.** Click the refresh button at the model dropdown menu and select your model.
3. Now click on the dropdown menu of the **Model loader** and select **AutoGPTQ** for those using a GTPQ model and **ctransformers** for those using a GGML model. Finally, click on **Load** to load your model.  
<!-- affiliate ads begin -->
<a href="https://ursime.pxf.io/c/5597632/2092236/16384" target="_top" id="2092236"><img src="//a.impactradius-go.com/display-ad/16384-2092236" border="0" alt="" width="1920" height="329"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2092236/16384" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![Setting model loader](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/10-select-model-loader.jpg)
4. To use the model, open the Chat tab and start testing the model.  
![Testing Llama 2 locally](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/12-testing-llama-2-locally.jpg)

 Congratulations, you've successfully loaded Llama2 on your local computer!

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4615471&QTY=1&AFFILIATE=108875&CART=1"><img src="https://images.wondershare.com/affiliate-image/affiliate_banners_en/max_782x90.png" border="0"></a>
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
<li><a href="https://extra-guidance.techidaily.com/new-laptop-perfection-10-coolest-downloadable-desktop-photos/"><u>[New] Laptop Perfection  10 Coolest Downloadable Desktop Photos</u></a></li>
<li><a href="https://vimeo-videos.techidaily.com/new-scalable-techniques-for-vimeo-broadcasting/"><u>[New] Scalable Techniques for Vimeo Broadcasting</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/new-the-pathway-to-pairing-perfection-obspluszoom-guide-for-2024/"><u>[New] The Pathway to Pairing Perfection  OBS+Zoom Guide for 2024</u></a></li>
<li><a href="https://on-screen-recording.techidaily.com/new-unveiling-the-techniques-behind-capturing-whatsapp-conversations-for-2024/"><u>[New] Unveiling the Techniques Behind Capturing WhatsApp Conversations for 2024</u></a></li>
<li><a href="https://remote-screen-capture.techidaily.com/updated-2024-approved-saving-the-ephemeral-a-guide-to-online-audio-recording/"><u>[Updated] 2024 Approved  Saving the Ephemeral  A Guide to Online Audio Recording</u></a></li>
<li><a href="https://screen-activity-recording.techidaily.com/updated-enhanced-google-chats-essential-techniques-4-ways-for-2024/"><u>[Updated] Enhanced Google Chats  Essential Techniques, 4 Ways for 2024</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/updated-fast-track-fun-turning-animated-art-into-sticky-messages-quickly/"><u>[Updated] Fast Track Fun  Turning Animated Art Into Sticky Messages Quickly</u></a></li>
<li><a href="https://facebook-video-footage.techidaily.com/updated-finalcut-pro-elevating-your-youtube-edits-from-good-to-great/"><u>[Updated] FinalCut Pro  Elevating Your YouTube Edits From Good to Great</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/updated-in-2024-uncover-the-past-advanced-methods-for-instagram-image-retrieval/"><u>[Updated] In 2024, Uncover the Past  Advanced Methods for Instagram Image Retrieval</u></a></li>
<li><a href="https://desktop-recording.techidaily.com/updated-the-definitive-guide-to-affordable-video-calls-online-for-2024/"><u>[Updated] The Definitive Guide to Affordable Video Calls Online for 2024</u></a></li>
<li><a href="https://facebook-video-recording.techidaily.com/2024-approved-feed-flourish-elevating-engagement-from-ordinary-posts/"><u>2024 Approved  Feed Flourish  Elevating Engagement From Ordinary Posts</u></a></li>
<li><a href="https://location-fake.techidaily.com/5-hassle-free-solutions-to-fake-location-on-find-my-friends-of-oppo-find-n3-drfone-by-drfone-virtual-android/"><u>5 Hassle-Free Solutions to Fake Location on Find My Friends Of Oppo Find N3 | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/7-exciting-bard-ai-features-announced-at-google-io-2023/"><u>7 Exciting Bard AI Features Announced at Google I/O 2023</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/advancing-crypto-discussions-via-gpt-innovations/"><u>Advancing Crypto Discussions via GPT Innovations</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-communicators-from-idea-to-interaction-using-gpt/"><u>AI Communicators: From Idea to Interaction - Using GPT</u></a></li>
<li><a href="https://extra-hints.techidaily.com/androids-pinnacle-podcast-platforms-your-essential-six-pack-for-2024/"><u>Android's Pinnacle Podcast Platforms  Your Essential Six-Pack for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/balancing-ai-realism-six-key-cues-for-authentic-respitsonses/"><u>Balancing AI Realism: Six Key Cues for Authentic Respitsonses</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/behind-chatgpt-revolutionizing-creativity-through-ai/"><u>Behind ChatGPT: Revolutionizing Creativity Through AI</u></a></li>
<li><a href="https://tech-haven.techidaily.com/chatgpt-plus-vs-perplexity-showdown-which-ai-powered-chatbot-takes-the-lead/"><u>ChatGPT Plus Vs. Perplexity Showdown: Which AI-Powered Chatbot Takes the Lead?</u></a></li>
<li><a href="https://win11-tips.techidaily.com/conquering-outlook-crashed-with-simple-solutions-windows-edition/"><u>Conquering Outlook Crashed with Simple Solutions, Windows Edition</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/deciphering-the-future-of-verification-on-twit/"><u>Deciphering the Future of Verification on Twit</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/deciphering-the-language-giants-bert-and-gpt-analysis/"><u>Deciphering the Language Giants: BERT & GPT Analysis</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/decoding-the-magic-how-does-predictive-ai-work/"><u>Decoding the Magic: How Does Predictive AI Work?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/elevating-ai-writing-making-chatgpt-write-like-you/"><u>Elevating AI Writing: Making ChatGPT Write Like You</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/exploring-career-trajectories-in-ai-driven-responsiveness-design/"><u>Exploring Career Trajectories in AI-Driven Responsiveness Design</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/future-employment-preparing-for-ai-driven-transformation/"><u>Future Employment: Preparing for AI-Driven Transformation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/harnessing-chatgpt-for-impressive-job-applications/"><u>Harnessing ChatGPT for Impressive Job Applications</u></a></li>
<li><a href="https://fake-location.techidaily.com/how-to-stop-google-chrome-from-tracking-your-location-on-lava-agni-2-5g-drfone-by-drfone-virtual-android/"><u>How to Stop Google Chrome from Tracking Your Location On Lava Agni 2 5G? | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/improving-blog-commentaries-with-ai-wisdom/"><u>Improving Blog Commentaries with AI Wisdom</u></a></li>
<li><a href="https://ios-unlock.techidaily.com/in-2024-what-does-jailbreaking-apple-iphone-7-i-do-get-answers-here-by-drfone-ios/"><u>In 2024, What Does Jailbreaking Apple iPhone 7 i Do? Get Answers here</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/leveraging-ai-for-poetic-excellence-the-chatgpt-method/"><u>Leveraging AI for Poetic Excellence: The ChatGPT Method</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/master-your-conversations-gpt-plus-a-premium-plan-for-us-citizens-20mth/"><u>Master Your Conversations: GPT-Plus, a Premium Plan for US Citizens ($20/Mth)</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-machine-talk-comparing-gpt-and-bingbot/"><u>Mastering Machine Talk: Comparing GPT and BingBot</u></a></li>
<li><a href="https://extra-hints.techidaily.com/moviemakermag-all-about-androvid-editor/"><u>MovieMakerMag  All About AndroVid Editor</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/streamlined-task-mastery-embracing-chatgpts-capabilities/"><u>Streamlined Task Mastery: Embracing ChatGPT's Capabilities</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-ai-hierarchy-strength-in-machines/"><u>The AI Hierarchy: Strength in Machines</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-route-to-reproduce-and-store-your-gpt-powered-talks/"><u>The Route to Reproduce and Store Your GPT-Powered Talks</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-ultimate-guide-to-crafting-ai-enhanced-prompts/"><u>The Ultimate Guide to Crafting AI-Enhanced Prompts</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unmasking-imitations-openais-new-gpt-verifier/"><u>Unmasking Imitations: OpenAI's New GPT Verifier</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-the-facts-gpts-limitations-in-crypto-research/"><u>Unveiling the Facts: GPT's Limitations in Crypto Research</u></a></li>
</ul></div>
