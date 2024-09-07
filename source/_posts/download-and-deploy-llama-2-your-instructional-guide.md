---
title: "Download & Deploy Llama 2: Your Instructional Guide"
date: 2024-09-06T23:36:08.913Z
updated: 2024-09-07T23:36:08.913Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Download & Deploy Llama 2: Your Instructional Guide"
excerpt: "This Article Describes Download & Deploy Llama 2: Your Instructional Guide"
thumbnail: https://thmb.techidaily.com/bf4e1b249b524363ca4352e12c7abcbd71ae226692000b54256157e02075b501.jpg
---

<!-- affiliate ads begin -->
<a href="https://bluettiit.sjv.io/c/5597632/2114267/17093" target="_top" id="2114267">
  <img src="//a.impactradius-go.com/display-ad/17093-2114267" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://bluettiit.sjv.io/i/5597632/2114267/17093" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Download & Deploy Llama 2: Your Instructional Guide

 Meta released Llama 2 in the summer of 2023\. The new version of Llama is fine-tuned with 40% more tokens than the original Llama model, doubling its context length and significantly outperforming other open-sourced models available. The fastest and easiest way to access Llama 2 is via an API through an online platform. However, if you want the best experience, installing and loading Llama 2 directly on your computer is best.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 With that in mind, we've created a step-by-step guide on how to use Text-Generation-WebUI to load a quantized Llama 2 LLM locally on your computer.

<!-- affiliate ads begin -->
<a href="https://bluettius.sjv.io/c/5597632/2139120/17108" target="_top" id="2139120">
  <img src="//a.impactradius-go.com/display-ad/17108-2139120" border="0" alt="https://techidaily.com" width="250" height="90"/>
</a>
<img height="0" width="0" src="https://bluettius.sjv.io/i/5597632/2139120/17108" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
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
<span id="1542129">
					<video width="864" height="1152" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1542129.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/16836-1542129">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1542129.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:540px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2F25home.pxf.io%2Fc%2F5597632%2F1542129%2F16836'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1542129/16836" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
4. A terminal will open and start the setup. Early on, the setup will pause and ask you what GPU you are using. Select the appropriate type of GPU installed on your computer and hit enter. For those without a dedicated graphics card, select **None (I want to run models in CPU mode)**. Keep in mind that running on CPU mode is much slower when compared to running the model with a dedicated GPU.  
![Selecting GPU hardware installed](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/5-select-gpu-settings.jpg)
5. Once the setup is complete, you can now launch Text-Generation-WebUI locally. You can do so by opening your preferred web browser and entering the provided IP address on the URL.  
<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2135353/19272" target="_top" id="2135353">
  <img src="//a.impactradius-go.com/display-ad/19272-2135353" border="0" alt="https://techidaily.com" width="180" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135353/19272" style="position:absolute;visibility:hidden;" border="0" />
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

 In this example, the model can be identified as a medium-sized Llama 2 model trained on 13 billion parameters optimized for chat inferencing using a dedicated CPU.

 For those running on a dedicated GPU, choose a **GPTQ** model, while for those using a CPU, choose **GGML**. If you want to chat with the model like you would with ChatGPT, choose **chat**, but if you want to experiment with the model with its full capabilities, use the **standard** model. As for parameters, know that using bigger models will provide better results at the expense of performance. I would personally recommend you start with a 7B model. As for quantization, use q4, as it's only for inferencing.

**Download:**[GGML](https://huggingface.co/localmodels/Llama-2-7B-ggml/tree/main) (Free)

**Download:**[GPTQ](https://huggingface.co/localmodels/Llama-2-7B-Chat-GPTQ/tree/main) (Free)

 Now that you know what iteration of Llama 2 you need, go ahead and download the model you want.

 In my case, since I'm running this on an ultrabook, I'll be using a GGML model fine-tuned for chat, **llama-2-7b-chat-ggmlv3.q4\_K\_S.bin.**

![Downloading Llama 2 model of your preference](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/8-download-llama-2-model.jpg)

<!-- affiliate ads begin -->
<a href="https://wigfever.sjv.io/c/5597632/2014850/22899" target="_top" id="2014850">
  <img src="//a.impactradius-go.com/display-ad/22899-2014850" border="0" alt="https://techidaily.com" width="320" height="90"/>
</a>
<img height="0" width="0" src="https://wigfever.sjv.io/i/5597632/2014850/22899" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 After the download is finished, place the model in **text-generation-webui-main** \> **models**.

![Placing Llama 2 model to model folder](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/9-place-model-to-model-folder.jpg)

<!-- affiliate ads begin -->
<a href="https://ephamedtechinc.pxf.io/c/5597632/2120866/26400?prodsku=mars" target="_top" id="2120866">
  <img src="//a.impactradius-go.com/display-ad/26400-2120866" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://ephamedtechinc.pxf.io/i/5597632/2120866/26400?prodsku=mars" style="position:absolute;visibility:hidden;" border="0" />
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
<span id="1982570">
					<video width="576" height="240" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1982570.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/22993-1982570">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1982570.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:360px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fhomestyler.sjv.io%2Fc%2F5597632%2F1982570%2F22993'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1982570/22993" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![Testing Llama 2 locally](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/12-testing-llama-2-locally.jpg)

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2118306/7443" target="_top" id="2118306">
  <img src="//a.impactradius-go.com/display-ad/7443-2118306" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2118306/7443" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://on-screen-recording.techidaily.com/new-elevate-your-recording-game-with-nvidias-tools/"><u>[New] Elevate Your Recording Game with NVIDIA's Tools</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-fine-tuning-your-fly-top-tips-for-choosing-drone-propellers/"><u>[New] Fine-Tuning Your Fly Top Tips for Choosing Drone Propellers</u></a></li>
<li><a href="https://youtube-clips.techidaily.com/2024-approved-a-comprehensive-guide-to-using-youtubes-cc-licensing/"><u>2024 Approved A Comprehensive Guide to Using YouTube's CC Licensing</u></a></li>
<li><a href="https://facebook-video-content.techidaily.com/2024-approved-personalizing-your-feed-with-soundtracks-android-and-ios-tips/"><u>2024 Approved Personalizing Your Feed with Soundtracks - Android & iOS Tips</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/adapting-careers-in-an-ai-driven-world/"><u>Adapting Careers in an AI-Driven World</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-unveiled-the-basics-simplified/"><u>AI Unveiled: The Basics Simplified</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/avoid-data-sharing-by-opting-out-of-chatgpt/"><u>Avoid Data Sharing by Opting Out of ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/boosting-efficiency-the-ultimate-guide-to-using-chatgpt-effectively/"><u>Boosting Efficiency: The Ultimate Guide to Using ChatGPT Effectively</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/code-strategies-for-effective-gpt-3-usage/"><u>Code Strategies for Effective GPT-3 Usage</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/collaborative-content-creation-responsible-use-of-ai-tools/"><u>Collaborative Content Creation: Responsible Use of AI Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/dream-trip-no-hurdles-choose-from-the-7-best-free-chatgpt-planning-tools/"><u>Dream Trip, No Hurdles - Choose From the 7 Best Free ChatGPT Planning Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/elevate-writing-workflow-with-8-advanced-ai-tools/"><u>Elevate Writing Workflow with 8 Advanced AI Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/embark-on-a-venture-into-dialogue-system-crafting/"><u>Embark on a Venture Into Dialogue System Crafting</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/explore-data-depths-like-never-before-select-perplexity-ai/"><u>Explore Data Depths Like Never Before - Select Perplexity AI</u></a></li>
<li><a href="https://youtube-blog.techidaily.com/-time-streamers-unite-learn-obs-and-broadcast-to-youtube-for-2024/"><u>First-Time Streamers Unite Learn OBS & Broadcast to Youtube for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/from-conversation-to-creativity-4-reasons-for-claude-3-preference/"><u>From Conversation to Creativity: 4 Reasons for Claude 3 Preference</u></a></li>
<li><a href="https://mondly-stories.techidaily.com/from-latin-to-iberia-spanish-vs-portuguese-phonetic-study/"><u>From Latin to Iberia: Spanish Vs. Portuguese Phonetic Study</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/gpt-3-alerts-staying-ahead-with-its-operating-status/"><u>GPT-3 Alerts: Staying Ahead with Its Operating Status</u></a></li>
<li><a href="https://change-location.techidaily.com/how-to-fix-android-app-not-installed-error-on-infinix-gt-10-pro-quickly-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>How to Fix Android App Not Installed Error on Infinix GT 10 Pro Quickly? | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-save-gpt-3-data-for-future-use/"><u>How to Save GPT-3 Data for Future Use</u></a></li>
<li><a href="https://youtube-stream.techidaily.com/in-2024-global-sensations-surpassing-100-million-views-on-youtube-the-yearly-countdown/"><u>In 2024, Global Sensations Surpassing 100 Million Views on YouTube (The Yearly Countdown)</u></a></li>
<li><a href="https://review-topics.techidaily.com/in-2024-how-to-fix-life360-shows-wrong-location-on-apple-iphone-14-pro-max-drfone-by-drfone-virtual-ios/"><u>In 2024, How to Fix Life360 Shows Wrong Location On Apple iPhone 14 Pro Max? | Dr.fone</u></a></li>
<li><a href="https://iphone-unlock.techidaily.com/in-2024-how-to-unlock-a-found-apple-iphone-8-plus-drfone-by-drfone-ios/"><u>In 2024, How To Unlock A Found Apple iPhone 8 Plus? | Dr.fone</u></a></li>
<li><a href="https://tiktok-video-recordings.techidaily.com/in-2024-tiktok-stitching-demos-for-beginners/"><u>In 2024, TikTok Stitching Demos for Beginners</u></a></li>
<li><a href="https://fox-info.techidaily.com/in-2024-unlock-the-full-potential-of-pixiz-in-video-making/"><u>In 2024, Unlock the Full Potential of Pixiz in Video Making</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/leveraging-chatgpts-plugin-for-wolfram-alpha-triad/"><u>Leveraging ChatGPT's Plugin for Wolfram Alpha Triad</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/maximizing-business-value-with-7-innovative-uses-of-chatgpt/"><u>Maximizing Business Value with 7 Innovative Uses of ChatGPT</u></a></li>
<li><a href="https://smart-video-creator.techidaily.com/new-2024-approved-the-professionals-choice-for-mac-adobe-premiere-pro-video-editor/"><u>New 2024 Approved The Professionals Choice for Mac Adobe Premiere Pro Video Editor</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/recipe-renovation-with-a-digital-master-chef-chatgpt/"><u>Recipe Renovation with a Digital Master Chef (ChatGPT)</u></a></li>
<li><a href="https://digital-screen-recording.techidaily.com/revolutionize-your-videos-essential-obs-edits-at-hand-for-2024/"><u>Revolutionize Your Videos Essential OBS Edits at Hand for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revolutionizing-work-through-ai-breakthroughs/"><u>Revolutionizing Work Through AI Breakthroughs</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/safeguarding-digital-realms-pushing-limits-with-7-trends/"><u>Safeguarding Digital Realms: Pushing Limits with 7 Trends</u></a></li>
<li><a href="https://youtube-sure.techidaily.com/inizing-tseries-earnings-from-digital-viewership-on-youtube/"><u>Scrutinizing TSeries’ Earnings From Digital Viewership on YouTube</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/share-across-platforms-instagram-meets-facebook/"><u>Share Across Platforms Instagram Meets Facebook</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/simplifying-clean-up-the-route-to-fresh-gpt-dialogues/"><u>Simplifying Clean-Up: The Route to Fresh GPT Dialogues</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/steps-to-ensure-obs-captures-sound-effectively-for-2024/"><u>Steps to Ensure OBS Captures Sound Effectively for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-best-4-ai-writing-companions-for-every-wordsmith/"><u>The Best 4 AI Writing Companions for Every Wordsmith</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-editors-guide-to-responsible-ai-engagement/"><u>The Editor's Guide to Responsible AI Engagement</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-mechanisms-behind-claude-2s-use/"><u>The Mechanisms Behind Claude 2'S Use</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/toms-tech-gear-comprehensive-hardware-reviews/"><u>Tom's Tech Gear - Comprehensive Hardware Reviews</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/top-6-frequent-gpt-missteps-and-corrections-guide/"><u>Top 6 Frequent GPT Missteps & Corrections Guide</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/transforming-job-hunting-with-smart-ai/"><u>Transforming Job Hunting with Smart AI</u></a></li>
<li><a href="https://twitter-videos.techidaily.com/twitch-out-streaming-twitters-hd-visuals-seamlessly-for-2024/"><u>Twitch Out Streaming Twitter's HD Visuals Seamlessly for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unlocking-chatgpt-potential-with-intelligent-folder-systems/"><u>Unlocking ChatGPT Potential with Intelligent Folder Systems</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unlocking-potential-with-quoras-poe-access/"><u>Unlocking Potential with Quora's POE Access</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-ai-the-ultimate-guide-by-openai/"><u>Unveiling AI: The Ultimate Guide by OpenAI</u></a></li>
</ul></div>
