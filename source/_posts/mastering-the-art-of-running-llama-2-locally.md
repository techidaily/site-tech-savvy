---
title: Mastering the Art of Running Llama 2 Locally
date: 2024-08-29T19:41:21.752Z
updated: 2024-08-30T19:41:21.752Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Mastering the Art of Running Llama 2 Locally
excerpt: This Article Describes Mastering the Art of Running Llama 2 Locally
thumbnail: https://thmb.techidaily.com/042cea82a1fcfb2242b9880aa52ff1cf0cb7e4c3cd3e6dc3d81f2870623c2d81.jpg
---

## Mastering the Art of Running Llama 2 Locally

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
<a href="https://store.massmailsoftware.com/order/checkout.php?PRODS=1300375&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/dc87c13749315c7217cdc4ac692e704c/banera_for_partners-15_%281%29.jpg" border="0"></a>
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
![Text-Generation-WebUI](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/7-text-generation-webui-view.jpg)

<!-- affiliate ads begin -->
<a href="https://natural-cycles.sjv.io/c/5597632/2072199/17885" target="_top" id="2072199"><img src="//a.impactradius-go.com/display-ad/17885-2072199" border="0" alt="" width="300" height="300"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2072199/17885" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
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

 After the download is finished, place the model in **text-generation-webui-main** \> **models**.

![Placing Llama 2 model to model folder](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/9-place-model-to-model-folder.jpg)

<!-- affiliate ads begin -->
<a href="https://ursime.pxf.io/c/5597632/2092236/16384" target="_top" id="2092236"><img src="//a.impactradius-go.com/display-ad/16384-2092236" border="0" alt="" width="1920" height="329"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2092236/16384" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=33729450&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/7f687767ccf20fcea1c9dc4a5adc2326/Digisigner_banner_728_x_90_color_version.png" border="0"></a>
<!-- affiliate ads end -->
![Testing Llama 2 locally](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/12-testing-llama-2-locally.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4693127&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.videosoftdev.com/images/video_editor/screenshots/1.jpg" border="0">
VSDC Pro Video Editor is a light professional non-linear video editing suite for creating a movie of any complexity. It supports the most popular video/audio formats and codecs, including 4K, HD and GoPro videos. Preconfigured profiles make the creation of videos for various multimedia and mobile devices absolutely hassle-free.

Key features:

•	Import from any devices and cams, including GoPro and drones. All formats supported. Сurrently the only free video editor that allows users to export in a new H265/HEVC codec, something essential for those working with 4K and HD.
•	Everything for hassle-free basic editing: cut, crop and merge files, add titles and favorite music
•	Visual effects, advanced color correction and trendy Instagram-like filters   
•	All multimedia processing done from one app: video editing capabilities reinforced by  a video converter, a screen capture, a video capture, a disc burner and a YouTube uploader
•	Non-linear editing: edit several files with simultaneously 
•	Easy export to social networks: special profiles for YouTube, Facebook, Vimeo, Twitter and Instagram
•	High quality export – no conversion quality loss, double export speed even of HD files due to hardware acceleration
•	Stabilization tool will turn shaky or jittery footage into a more stable video automatically. 
•	Essential toolset for professional video editing: blending modes, Mask tool, advanced multiple-color Chroma Key  
</a>
<!-- affiliate ads end -->
 Congratulations, you've successfully loaded Llama2 on your local computer!

<!-- affiliate ads begin -->
<a href="https://store.iobit.com/order/checkout.php?PRODS=4596923&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/184260348236f9554fe9375772ff966e/ascscan_468X60.png" border="0"></a>
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
<li><a href="https://vp-tips.techidaily.com/new-2024-approved-unveiling-how-to-activate-windows-11-written-for-high-dynamic-range-auto-hdr/"><u>[New] 2024 Approved  Unveiling How to Activate Windows 11' Written for High Dynamic Range (Auto HDR)</u></a></li>
<li><a href="https://vp-tips.techidaily.com/new-lunapic-essentials-starting-with-simple-edits/"><u>[New] LunaPic Essentials  Starting with Simple Edits</u></a></li>
<li><a href="https://vp-tips.techidaily.com/new-mastering-radial-blur-photoshop-edition/"><u>[New] Mastering Radial Blur  Photoshop Edition</u></a></li>
<li><a href="https://screen-capture.techidaily.com/new-top-ranked-mac-pro-video-maker-plus-audio/"><u>[New] Top-Ranked Mac Pro Video Maker Plus Audio</u></a></li>
<li><a href="https://screen-video-capture.techidaily.com/updated-2024-approved-minimalist-obs-adjustments-for-under-500-pcs/"><u>[Updated] 2024 Approved  Minimalist OBS Adjustments for Under-$500 PCs</u></a></li>
<li><a href="https://extra-support.techidaily.com/updated-photography-for-rookies-top-cameras-of-the-year-2024/"><u>[Updated] Photography for Rookies  Top Cameras of the Year 2024</u></a></li>
<li><a href="https://ios-unlock.techidaily.com/7-ways-to-lock-apps-on-apple-iphone-12-and-ipad-securely-by-drfone-ios/"><u>7 Ways to Lock Apps on Apple iPhone 12 and iPad Securely</u></a></li>
<li><a href="https://extra-hints.techidaily.com/accessing-disguised-user-responses-on-yt-for-2024/"><u>Accessing Disguised User Responses on YT for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ace-the-interview-with-chatgpt-training-tips/"><u>Ace the Interview with ChatGPT Training Tips</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-escapes-discover-these-7-free-chatgpt-apps-for-effortless-itineraries/"><u>AI Escapes: Discover These 7 Free ChatGPT Apps for Effortless Itineraries</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ais-shortfall-in-digital-guardianship/"><u>AI's Shortfall in Digital Guardianship</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/bards-versus-ai-can-woolly-sentinels-outmatch-digital-mind/"><u>Bards Versus AI: Can Woolly Sentinels Outmatch Digital Mind?</u></a></li>
<li><a href="https://extra-hints.techidaily.com/bring-to-life-the-dance-of-light-on-faces-employing-motion-blur-effects-in-picsart-for-2024/"><u>Bring to Life the Dance of Light on Faces  Employing Motion Blur Effects in Picsart for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-as-a-tool-for-effective-work-scheduling/"><u>ChatGPT as a Tool for Effective Work Scheduling</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/critical-examination-of-the-conceptual-parallels-between-traditional-libraries-and-online-information-systems/"><u>Critical Examination of the Conceptual Parallels Between Traditional Libraries and Online Information Systems</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/cutting-edge-ai-strategies-7-proven-tips-unveiled/"><u>Cutting-Edge AI Strategies: 7 Proven Tips Unveiled</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/digital-collaboration-redefined-with-6-chatgpt-techniques/"><u>Digital Collaboration Redefined with 6 ChatGPT Techniques</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/exploring-advanced-ai-forefronts-potential-versus-chatgpts-limits/"><u>Exploring Advanced AI: Forefront's Potential Versus ChatGPT's Limits</u></a></li>
<li><a href="https://win-answers.techidaily.com/fixing-relink-launch-problems-in-your-favorite-rpg-granblue-fantasy/"><u>Fixing Relink Launch Problems in Your Favorite RPG, Granblue Fantasy</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/frontiers-of-ai-technology-exploring-this-seasons-top-five-innovations/"><u>Frontiers of AI Technology: Exploring This Season's Top Five Innovations</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/gpt-versus-bing-battle-of-the-top-tier-ai-communicators/"><u>GPT Versus Bing: Battle of the Top-Tier AI Communicators</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/honest-scholarship-steering-clear-from-chatgpt-dependence/"><u>Honest Scholarship: Steering Clear From ChatGPT Dependence</u></a></li>
<li><a href="https://review-topics.techidaily.com/how-to-upgrade-iphone-8-to-the-latest-ios-version-drfone-by-drfone-ios-system-repair-ios-system-repair/"><u>How to Upgrade iPhone 8 to the Latest iOS Version? | Dr.fone</u></a></li>
<li><a href="https://android-transfer.techidaily.com/in-2024-easiest-guide-how-to-clone-honor-x9b-phone-drfone-by-drfone-transfer-from-android-transfer-from-android/"><u>In 2024, Easiest Guide How to Clone Honor X9b Phone? | Dr.fone</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/in-2024-how-to-use-allshare-cast-to-turn-on-screen-mirroring-on-nokia-g310-drfone-by-drfone-android/"><u>In 2024, How To Use Allshare Cast To Turn On Screen Mirroring On Nokia G310 | Dr.fone</u></a></li>
<li><a href="https://twitter-videos.techidaily.com/in-2024-social-media-synopsis-top-trending-twitvideos/"><u>In 2024, Social Media Synopsis  Top Trending TwitVideos</u></a></li>
<li><a href="https://youtube-webster.techidaily.com/24-tailored-thumbnails-aspect-ratios-for-maximum-clicks/"><u>In 2024, Tailored Thumbnails  Aspect Ratios for Maximum Clicks</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/in-2024-unlock-your-iphone-13-mini-in-minutes-with-iccid-code-everything-you-need-to-know-by-drfone-ios/"><u>In 2024, Unlock Your iPhone 13 mini in Minutes with ICCID Code Everything You Need to Know</u></a></li>
<li><a href="https://some-techniques.techidaily.com/innovative-image-editors-your-ultimate-text-companion-for-2024/"><u>Innovative Image Editors  Your Ultimate Text Companion for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/leveraging-gpt-to-enrich-your-imaginative-dungeon-quests/"><u>Leveraging GPT to Enrich Your Imaginative Dungeon Quests</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/machine-learning-meets-numbers-game/"><u>Machine Learning Meets Numbers Game</u></a></li>
<li><a href="https://hardware-help.techidaily.com/newest-tp-link-wireless-network-card-software-compatible-with-win-1187-systems/"><u>Newest TP-Link Wireless Network Card Software | Compatible with Win 11/8/7 Systems</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/openai-launches-custom-gpt-store-how-to-access-and-use-it-right-now/"><u>OpenAI Launches Custom GPT Store: How to Access and Use It Right Now</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/optimizing-team-collaboration-using-chatgpt-technology/"><u>Optimizing Team Collaboration Using ChatGPT Technology</u></a></li>
<li><a href="https://graphic-issues.techidaily.com/overcoming-unavailable-screen-options-barrier/"><u>Overcoming Unavailable Screen Options Barrier</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/pinnacle-of-generative-tech-notion-vs-chatgpt-analysis/"><u>Pinnacle of Generative Tech: Notion Vs. ChatGPT Analysis</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/pushing-boundaries-of-development-combining-chatgpt-and-vs-code/"><u>Pushing Boundaries of Development: Combining ChatGPT & VS Code</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/real-data-vs-fake-navigating-ai-generated-illusions-with-ease/"><u>Real Data vs Fake: Navigating AI-Generated Illusions with Ease</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revolutionize-office-tasks-combining-docspace-plus-chatgpt/"><u>Revolutionize Office Tasks: Combining DocSpace + ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/seamless-chatgpt-use-with-siri-enabled-iphones/"><u>Seamless ChatGPT Use with Siri-Enabled iPhones</u></a></li>
<li><a href="https://techtrends.techidaily.com/step-by-step-instructions-for-taking-off-and-replacing-your-phones-screen-safeguard/"><u>Step-by-Step Instructions for Taking Off & Replacing Your Phone's Screen Safeguard</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-art-of-verse-integrating-chatgpt-in-book-writing/"><u>The Art of Verse: Integrating ChatGPT in Book Writing</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-dark-side-of-seeking-help-from-artificial-intelligence/"><u>The Dark Side of Seeking Help From Artificial Intelligence</u></a></li>
<li><a href="https://extra-hints.techidaily.com/the-essential-meme-blueprint-building-impactful-gifs/"><u>The Essential Meme Blueprint  Building Impactful GIFs</u></a></li>
<li><a href="https://bypass-frp.techidaily.com/ultimate-guide-on-infinix-hot-40-pro-frp-bypass-by-drfone-android/"><u>Ultimate Guide on Infinix Hot 40 Pro FRP Bypass</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-ai-mirage-techniques-to-discern-real-insights-from-fake/"><u>Unveiling AI Mirage: Techniques to Discern Real Insights From Fake</u></a></li>
<li><a href="https://youtube-docs.techidaily.com/ant-portraits-professional-thumbnails-made-in-a-flash-in-2024/"><u>Valorant Portraits - Professional Thumbnails Made in a Flash, In 2024</u></a></li>
</ul></div>
