---
title: "Engage GPT: Leveraging Bash for OpenAI's Chatbot"
date: 2024-08-25T17:39:26.578Z
updated: 2024-08-26T17:39:26.578Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Engage GPT: Leveraging Bash for OpenAI's Chatbot"
excerpt: "This Article Describes Engage GPT: Leveraging Bash for OpenAI's Chatbot"
thumbnail: https://thmb.techidaily.com/a362218194355c666b0860326aa79761dfe27d2518f12f424f4610cd1ffe517b.jpg
---

## Engage GPT: Leveraging Bash for OpenAI's Chatbot

 Artificial intelligence has emerged as a new-age sensation, leaving everything behind in the dust. With new additions daily, there is a lot to look forward to.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 People use this multi-faceted, ubiquitous tool to crack jokes, write codes and even answer the most random questions. It’s easy to use ChatGPT on other OSes, so, as a Linux user, why should you stay behind?

 You too can enjoy ChatGPT’s Linux avatar, ShellGPT. Here's how to install and use the AI tool from your Ubuntu terminal in a few easy steps.

## What’s ShellGPT, ChatGPT’s Equivalent Linux Namesake?

 ShellGPT, as it is more commonly known, is ChatGPT’s command-line equivalent, through which users can use and engage with the AI chatbot via their Linux terminal. The chatbot draws power from OpenAI’s Large Language Model, providing intelligent user recommendations.

 Large Language Models (LLMs) are becoming a hot topic of discussion since you can easily [run LLM-enabled chatbots on your Raspberry Pi](https://www.makeuseof.com/raspberry-pi-large-language-model/).

 Sounds intriguing, doesn’t it?

 If you have experience interacting with ChatGPT, you will love this alternate Linux shell version.

 What’s the benefit of installing ShellGPT on your machine? It’s simple; you don’t need to type in unnecessary long commands or head to your browser. Instead, you can perform all possible tasks from the comfort of your Linux terminal.

 Before installing ShellGPT on your Ubuntu machine, here are a few prerequisites to take care of.

## Step 1: Install Python and PIP on Your Machine

 Like most artificial intelligence-enabled tools, even ShellGPT runs on Python. While Python is usually installed by default on most Linux distros, you can check its installation via its version information. If Python isn’t available on your machine, you must install it before moving on to the next steps.

 Open a terminal and type in the following commands to check Python’s version:

`python3 --version`

 If the command returns a numeric version output, you can safely assume you’re rearing and ready to go. However, if you encounter any errors, you should [install Python on Ubuntu](https://www.makeuseof.com/install-python-ubuntu/), before installing PIP.

 Now that you have Python installed on your machine, it’s time to install PIP, Python’s native package manager.

 Even though PIP is usually pre-installed with the Python bundle, it’s best to check the version beforehand to know its installation status. Run the following command to check if it is installed on your machine:

`pip --version`

 If you get the following error post-execution, you need to install the package manager:

`Command 'pip' not found, but can be installed with:  
`

 You can use the following command to install it:

`sudo apt install python3-pip`

![Ubuntu terminal window with code snippets with installation codes](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/install-pip-on-ubuntu.jpg)

 After installation, you can again use the **\--version** command to check if the installation was successful.

<!-- affiliate ads begin -->
<a href="https://estore.winxdvd.com/order/checkout.php?PRODS=4081991&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.winxdvd.com/affiliate/new-banner/wt-500x500.jpg" border="0"></a>
<!-- affiliate ads end -->
## Step 2: Install and Set Up a Virtual Environment Using Python

 Now that Python and PIP are ready, you can set up Python's virtual environment to make the machine environment conducive for installing and running ShellGPT. Virtual environments are ideal for running isolated programs since they can avoid library conflicts.

 With a virtual environment in tow, you can limit the interactions between your system's and virtual environment's programs while performing different executions in silos.

 Using a virtual environment is an optional step, to avoid any unforeseen mishaps while installing and using Python libraries.

 To create a virtual environment using Python, you need to install the **venv** module:

`sudo apt install python3-venv -y`

![Ubuntu terminal window code snippets](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/install-virtual-environment-module-in-ubuntu.jpg)

<!-- affiliate ads begin -->
<a href="https://turtlebeachus.sjv.io/c/5597632/1988416/23719" target="_top" id="1988416"><img src="//a.impactradius-go.com/display-ad/23719-1988416" border="0" alt="" width="600" height="600"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1988416/23719" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
### Set Up the Virtual Environment

 Once you've installed the virtual environment, you can set it up, so that it can facilitate ShellGPT's commands seamlessly.

 First, create a new directory to organize and host the files. You can use the **mkdir** command, followed by the directory name, as follows:

`mkdir cli-shellgpt`

 Navigate to this newly created directory with [the cd command](https://www.makeuseof.com/cd-command-in-linux/):

`cd cli-shellgpt`

 Then, create a new virtual environment with the **venv** command, followed by an environment name:

`python3 -m venv cli-shellgpt`

 Since the virtual environment isn't enabled by default, you must enable it manually with the **activate** script:

`source cli-shellgpt/bin/activate`

 As soon as you execute the above command, you will notice the default Linux shell prompt changes, as shown below:

`(cli-shellgpt) sahil@vm:`

![Ubuntu terminal window with code snippets](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/enable-virtual-environment-for-shellgpt-in-ubuntu-1.jpg)

## Step 3: Generate an OpenAPI Key

 Since the virtual environment is ready, you must connect the OpenAI services and your Ubuntu machine to run ShellGPT. For this purpose, you must navigate to [OpenAI's website](https://openai.com/) and create an account there.

 If you have an existing account, you can log in with your credentials and navigate to your profile image, located on the top right-hand side of the website.

 Click on **View API Keys**, followed by **Create new secret key**.

![OpenAI website interface showing a drop-down menu](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/view-api-keys-on-openai-website.jpg)

<!-- affiliate ads begin -->
<a href="https://estore.zonealarm.com/order/checkout.php?PRODS=36245101&QTY=1&AFFILIATE=108875&CART=1"><img src="https://sc1.checkpoint.com/sc1/za/images/boxes/zang_box_trust.png" border="0">ZoneAlarm Extreme Security NextGen</a>
<!-- affiliate ads end -->
 Do not share this key with anyone since the connection is private and should be used on your machine only.

 Copy the API key from the dialog box, and save it somewhere, since you won't be able to review the same key again.

![OpenAI's secret key website page with an open dialog box](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/generate-api-secret-key.jpg)

 To establish a connection on your Ubuntu machine, create an environment variable with the **export** command:

`export OPENAI_API_KEY=<paste key details here>`

### Add and Verify the API Key Into a Virtual Environment Variable

 When you execute the API key in this manner, Linux will use it only for a single instance. However, if you want to make the execution permanent, save it in the **.bashrc** file.

 All you have to do is type in the first command and enter the subsequent command within the text editor:

`nano ./bashrc  
export OPENAI_API_KEY=<paste key details here>`

![Ubuntu terminal window with code snippets to create and save an environment variable](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/create-an-environment-variable-1.jpg)

 Save and exit the editor. Then, use the source command to enable the changes.

`source ./bashrc`

 Finally, verify the API key with the **env** command.

`env`

![List of variables in a linux terminal](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/check-secret-key-in-env-list.jpg)

 Your **OPENAI\_API\_KEY** environment variable should be listed in the output.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=30901369&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/ce9a6fb2becc2d235e62b125e9260102/products/1_copy_vMixCallScreenshot1-large.jpg" border="0"> vMix 4K - Software based live production. vMix 4K includes everything in vMix HD plus 4K support, PTZ control, External/Fullscreen output, 4 Virtual Outputs, 1 Replay, 4 vMix Call, and 2 Recorders. 
This bundle includes Studio 200 for vMix from Virtualsetworks, HTTP Matrix 1.0 automation scheduler, and 4 introductory training videos from the Udemy vMix Basic to Amazing course. </a>
<!-- affiliate ads end -->
## Step 5: Install ShellGPT on Ubuntu

 Once all the installation formalities are complete, you can simply move on to the best part, the ShellGPT installation. The installation steps are quite straightforward, and you can install the tool with the following command:

`pip3 install shell-gpt`

![Installation snippet on ubuntu's terminal screen](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/install-shell-gpt-on-ubuntu.jpg)

<!-- affiliate ads begin -->
<a href="https://vapordna.pxf.io/c/5597632/1496243/17238" target="_top" id="1496243"><img src="//a.impactradius-go.com/display-ad/17238-1496243" border="0" alt="" width="1000" height="1221"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1496243/17238" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 Let the installation finish; meanwhile, you can check out some interesting ways to use the AI tool via your terminal window.

<!-- affiliate ads begin -->
<a href="https://mushroom-supplies.sjv.io/c/5597632/1692242/18134" target="_top" id="1692242"><img src="//a.impactradius-go.com/display-ad/18134-1692242" border="0" alt="" width="834" height="592"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1692242/18134" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Using ShellGPT for Running Queries via the Terminal

 The entire purpose of installing ShellGPT is to make your life easier. To use the terminal as a search engine and run some queries, you can use the **sgpt** command, followed by your query within quotes:

`sgpt "How many galaxies exist within the universe"`

![Ubuntu terminal interface with a query response](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/shellgpt-query-reponse.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4718730&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/ce9a6fb2becc2d235e62b125e9260102/products/copy_vMixCallScreenshot1-large.jpg" border="0">vMix HD - Software based live production. vMix HD includes everything in vMix Basic HD plus 1000 inputs, Video List, 4 Overlay Channels, and 1 vMix Call 
This bundle includes Studio 200 for vMix from Virtualsetworks, HTTP Matrix 1.0 automation scheduler, and 4 introductory training videos from the Udemy vMix Basic to Amazing course. </a>
<!-- affiliate ads end -->
## Using ShellGPT for Generating Code

 You can use your ShellGPT for generating code as well. You can do it by passing the right command with the **sgpt** command:

`sgpt --code "print the Fibonacci series"`

![Ubuntu terminal window with code snippets](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/shellgpt-code-reponse.jpg)

 The output consists of code you can execute within Python to generate the Fibonacci series.

<!-- affiliate ads begin -->
<a href="https://shop.systoolsgroup.com/affiliate.php?ACCOUNT=SYSTOOBY&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.systoolsgroup.com%3FAFFILIATE%3D108875%26RESOURCE%3DSysTools%2BSQL%2BRecovery"><img src="https://www.systoolsgroup.com/box/sql-recovery.png" border="0"></a>
<!-- affiliate ads end -->
## Using ShellGPT Within Ubuntu’s Terminal

 Linux commands become easy, especially when everything is available within your terminal window. From running shell commands to using your terminal as a search engine, you can do it all with ShellGPT.

 But since ShellGPT is based on the same concept as ChatGPT, it has its own set of problems, which might take a while to perfect. Until you can download the new bug-free version, it's best to continue working with the tool's imperfections and make your life easier with ShellGPT's automated commands.

**SCROLL TO CONTINUE WITH CONTENT**

 People use this multi-faceted, ubiquitous tool to crack jokes, write codes and even answer the most random questions. It’s easy to use ChatGPT on other OSes, so, as a Linux user, why should you stay behind?

 You too can enjoy ChatGPT’s Linux avatar, ShellGPT. Here's how to install and use the AI tool from your Ubuntu terminal in a few easy steps.

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
<li><a href="https://youtube-tips.techidaily.com/024-approved-elevate-your-content-game-on-youtube-top-11-video-seo-insights/"><u>[New] 2024 Approved  Elevate Your Content Game on YouTube  Top 11 Video SEO Insights</u></a></li>
<li><a href="https://youtube-blog.techidaily.com/024-approved-enhancing-video-soundtracks-on-digital-platforms/"><u>[New] 2024 Approved  Enhancing Video Soundtracks on Digital Platforms</u></a></li>
<li><a href="https://facebook-video-share.techidaily.com/new-2024-approved-explore-top-7-live-streaming-iosandroid-apps-perfect-for-youtube-channel-creators/"><u>[New] 2024 Approved  Explore Top 7 Live Streaming iOS/Android Apps Perfect for YouTube Channel Creators</u></a></li>
<li><a href="https://extra-tips.techidaily.com/new-apple-music-enhancement-for-exquisite-videos/"><u>[New] Apple Music Enhancement for Exquisite Videos</u></a></li>
<li><a href="https://facebook-video-share.techidaily.com/updated-wealth-wave-on-your-screen-monetizing-as-a-streamer/"><u>[Updated] Wealth Wave on Your Screen  Monetizing as a Streamer</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/achieving-holistic-health-setting-clear-targets-with-chatgpt/"><u>Achieving Holistic Health: Setting Clear Targets with ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-supercharge-your-task-management-with-top-8-chrome-plug-ins/"><u>AI Supercharge Your Task Management with Top 8 Chrome Plug-Ins</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/apples-guide-to-authentic-chatgpt-software/"><u>Apple's Guide to Authentic ChatGPT Software</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatbot-showdown-gpt-plus-against-perplexity/"><u>ChatBot Showdown: GPT Plus Against Perplexity</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgptplus-your-guide-to-language-proficiency-journey/"><u>ChatGPT+: Your Guide to Language Proficiency Journey</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/dall-e-3-webp-to-jpegpng-optimization-tips/"><u>DALL-E 3 WebP to JPEG/PNG Optimization Tips</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/decoding-ai-for-everyone/"><u>Decoding AI for Everyone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/enhance-your-gpt-experience-with-a-well-chosen-vpn/"><u>Enhance Your GPT Experience with a Well-Chosen VPN?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/explore-the-best-4-ai-tools-for-dynamic-story-creation/"><u>Explore the Best 4 AI Tools for Dynamic Story Creation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/exploring-the-potential-of-ai-chatgpt-for-commercial-growth/"><u>Exploring the Potential of AI: ChatGPT for Commercial Growth</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-does-openais-shap-enhance-model-insight/"><u>How Does OpenAI's SHAP Enhance Model Insight?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/immediate-effect-why-does-italy-ban-chatgpt/"><u>Immediate Effect: Why Does Italy Ban ChatGPT?</u></a></li>
<li><a href="https://iphone-unlock.techidaily.com/in-2024-easy-steps-on-how-to-create-a-new-apple-id-account-on-iphone-14-pro-drfone-by-drfone-ios/"><u>In 2024, Easy Steps on How To Create a New Apple ID Account On iPhone 14 Pro | Dr.fone</u></a></li>
<li><a href="https://review-topics.techidaily.com/in-2024-how-can-i-use-a-fake-gps-without-mock-location-on-vivo-y78plus-t1-edition-drfone-by-drfone-virtual-android/"><u>In 2024, How Can I Use a Fake GPS Without Mock Location On Vivo Y78+ (T1) Edition? | Dr.fone</u></a></li>
<li><a href="https://some-approaches.techidaily.com/in-2024-the-best-8-screenshot-and-video-editing-tools-for-phones/"><u>In 2024, The Best 8 Screenshot & Video Editing Tools for Phones</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/outpacing-chatgpt-10-ai-wonders-unleashed/"><u>Outpacing ChatGPT: 10 AI Wonders Unleashed</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/rapid-italian-crackdown-on-chatgpt-usage-explored/"><u>Rapid Italian Crackdown on ChatGPT Usage Explored</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/reimagine-the-kitchen-7-chatgpt-assisted-cooking-strategies/"><u>Reimagine the Kitchen: 7 ChatGPT-Assisted Cooking Strategies</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revelatory-information-talking-to-the-chatgpt-bot/"><u>Revelatory Information: Talking to the ChatGPT Bot</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revolutionizing-interview-preparation-with-ai-chatgpt/"><u>Revolutionizing Interview Preparation with AI: ChatGPT</u></a></li>
<li><a href="https://desktop-recording.techidaily.com/safedrive-backup-specialists-take/"><u>SafeDrive Backup Specialists' Take</u></a></li>
<li><a href="https://technical-tips.techidaily.com/step-by-step-guide-repairing-and-restoring-functionality-to-your-xbox-series-console-headphones/"><u>Step-by-Step Guide: Repairing and Restoring Functionality to Your Xbox Series Console Headphones</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/tackling-service-interruptions-in-chatgpt-plugin-relationships/"><u>Tackling Service Interruptions in ChatGPT-Plugin Relationships</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-8-best-crypto-chatgpt-plugins/"><u>The 8 Best Crypto ChatGPT Plugins</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-quintet-of-artifice-how-ai-ushers-in-cybercrime-innovation/"><u>The Quintet of Artifice: How AI Ushers in Cybercrime Innovation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unlocking-ai-potential-insights-into-vector-databases/"><u>Unlocking AI Potential: Insights Into Vector Databases</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unraveling-openais-pioneering-advancements/"><u>Unraveling OpenAI's Pioneering Advancements</u></a></li>
</ul></div>
