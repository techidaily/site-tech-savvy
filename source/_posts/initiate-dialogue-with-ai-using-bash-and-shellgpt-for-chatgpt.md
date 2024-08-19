---
title: "Initiate Dialogue with AI: Using Bash and ShellGPT for ChatGPT"
date: 2024-08-18T09:56:32.350Z
updated: 2024-08-19T09:56:32.350Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Initiate Dialogue with AI: Using Bash and ShellGPT for ChatGPT"
excerpt: "This Article Describes Initiate Dialogue with AI: Using Bash and ShellGPT for ChatGPT"
thumbnail: https://thmb.techidaily.com/25e355cfe41e9e10950c631e4aa9da16590e30c123d991c0d3d8b6703e367f7f.png
---

## Initiate Dialogue with AI: Using Bash and ShellGPT for ChatGPT

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

## Step 2: Install and Set Up a Virtual Environment Using Python

 Now that Python and PIP are ready, you can set up Python's virtual environment to make the machine environment conducive for installing and running ShellGPT. Virtual environments are ideal for running isolated programs since they can avoid library conflicts.

 With a virtual environment in tow, you can limit the interactions between your system's and virtual environment's programs while performing different executions in silos.

 Using a virtual environment is an optional step, to avoid any unforeseen mishaps while installing and using Python libraries.

 To create a virtual environment using Python, you need to install the **venv** module:

`sudo apt install python3-venv -y`

![Ubuntu terminal window code snippets](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/install-virtual-environment-module-in-ubuntu.jpg)

<!-- affiliate ads begin -->
<a href="https://store.nero.com/order/checkout.php?PRODS=22889392&QTY=1&AFFILIATE=108875&CART=1"><img src="http://webstatic.nero.com/nero2015-com-wAssets/img/affiliate/media/banner728-90eng.jpg" border="0"></a>
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

 Do not share this key with anyone since the connection is private and should be used on your machine only.

 Copy the API key from the dialog box, and save it somewhere, since you won't be able to review the same key again.

![OpenAI's secret key website page with an open dialog box](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/generate-api-secret-key.jpg)

 To establish a connection on your Ubuntu machine, create an environment variable with the **export** command:

`export OPENAI_API_KEY=<paste key details here>`

<!-- affiliate ads begin -->
<a href="https://ursime.pxf.io/c/5597632/2048972/16384" target="_top" id="2048972"><img src="//a.impactradius-go.com/display-ad/16384-2048972" border="0" alt="" width="1200" height="900"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2048972/16384" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
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

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4709458&QTY=1&AFFILIATE=108875&CART=1"><img src="https://3d-kstudio.com/wp-content/uploads/2019/10/Project-Manager-version-3-1600x900-768x419.jpg" border="0">Project Manager - Asset Browser for 3Ds Max</a>
<!-- affiliate ads end -->
 Your **OPENAI\_API\_KEY** environment variable should be listed in the output.

<!-- affiliate ads begin -->
<a href="https://order.glarysoft.com/order/checkout.php?PRODS=4691139&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/6734fa703f6633ab896eecbdfad8953a/products/SU-200-1.png" border="0">Software Update Pro - Check and update software installed on your computer. </a>
<!-- affiliate ads end -->
## Step 5: Install ShellGPT on Ubuntu

 Once all the installation formalities are complete, you can simply move on to the best part, the ShellGPT installation. The installation steps are quite straightforward, and you can install the tool with the following command:

`pip3 install shell-gpt`

![Installation snippet on ubuntu's terminal screen](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/install-shell-gpt-on-ubuntu.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4940312&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/333ac5d90817d69113471fbb6e531bee/sps-partnership-728x90eng.png" border="0"></a>
<!-- affiliate ads end -->
 Let the installation finish; meanwhile, you can check out some interesting ways to use the AI tool via your terminal window.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=38729081&QTY=1&AFFILIATE=108875&CART=1"><img src="https://website-prod.cache.wpscdn.com/img/wps-spreadsheet-free-excel-editor-online-offline-1x.93e269d.png" border="0">
WPS Office Premium ( File Recovery, Photo Scanning, Convert PDF)--Yearly</a>
<!-- affiliate ads end -->
## Using ShellGPT for Running Queries via the Terminal

 The entire purpose of installing ShellGPT is to make your life easier. To use the terminal as a search engine and run some queries, you can use the **sgpt** command, followed by your query within quotes:

`sgpt "How many galaxies exist within the universe"`

![Ubuntu terminal interface with a query response](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/shellgpt-query-reponse.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.textstudio.com/order/checkout.php?PRODS=35633309&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/d6eb8222c9718486bdabce8b897380f7/products/3_premium-icon.png" border="0"> Take advantage of PREMIUM features for 12 months. 
Create your texts / logos without any limitation. 
No attribution required when downloading. 
No advertising on the website. 
 TextStudio.com  PREMIUM - Yearly Membership</a>
<!-- affiliate ads end -->
<!-- affiliate ads begin -->
<a href="https://turtlebeachus.sjv.io/c/5597632/1988416/23719" target="_top" id="1988416"><img src="//a.impactradius-go.com/display-ad/23719-1988416" border="0" alt="" width="600" height="600"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1988416/23719" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Using ShellGPT for Generating Code

 You can use your ShellGPT for generating code as well. You can do it by passing the right command with the **sgpt** command:

`sgpt --code "print the Fibonacci series"`

![Ubuntu terminal window with code snippets](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/shellgpt-code-reponse.jpg)

 The output consists of code you can execute within Python to generate the Fibonacci series.

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
<li><a href="https://youtube-blog.techidaily.com/024-approved-navigate-through-youtube-content-with-flexibility/"><u>[New] 2024 Approved  Navigate Through YouTube Content with Flexibility</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/new-in-2024-capture-attention-incorporating-borders-to-insta-videos/"><u>[New] In 2024, Capture Attention  Incorporating Borders to Insta-Videos</u></a></li>
<li><a href="https://eaxpv-info.techidaily.com/updated-2024-approved-flashglimpse-crafter/"><u>[Updated] 2024 Approved  FlashGlimpse Crafter</u></a></li>
<li><a href="https://twitter-videos.techidaily.com/updated-twitters-required-video-aspect-ratios-explained-for-2024/"><u>[Updated] Twitter's Required Video Aspect Ratios Explained for 2024</u></a></li>
<li><a href="https://extra-information.techidaily.com/2024-approved-audiovisual-harmony-music-integration-in-social-media/"><u>2024 Approved  Audiovisual Harmony  Music Integration in Social Media</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-powered-strategies-for-achieving-desired-career/"><u>AI-Powered Strategies for Achieving Desired Career</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/alert-on-mimicry-genuine-ai-apps-versus-fake-ones/"><u>Alert on Mimicry: Genuine AI Apps Versus Fake Ones</u></a></li>
<li><a href="https://techidaily.com/all-things-you-need-to-know-about-wipe-datafactory-reset-for-xiaomi-redmi-note-12-5g-drfone-by-drfone-reset-android-reset-android/"><u>All Things You Need to Know about Wipe Data/Factory Reset For Xiaomi Redmi Note 12 5G | Dr.fone</u></a></li>
<li><a href="https://tech-revival.techidaily.com/beyond-comparisons-the-intricate-differences-between-siri-and-chatgpt-revealed/"><u>Beyond Comparisons - The Intricate Differences Between Siri and ChatGPT Revealed</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/breaching-chatgpt-barriers-a-guide/"><u>Breaching ChatGPT Barriers: A Guide</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/breaking-barriers-dialogue-with-ai-chatgpt/"><u>Breaking Barriers: Dialogue With AI ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/building-skills-through-effort-not-chatgpt-replies/"><u>Building Skills Through Effort, Not ChatGPT Replies</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatbot-authenticity-beyond-plagiarism-fears/"><u>ChatBot Authenticity: Beyond Plagiarism Fears</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-evolved-discover-the-features-that-matter-most/"><u>ChatGPT Evolved: Discover the Features That Matter Most!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-meets-android-unleash-voicepower/"><u>ChatGPT Meets Android: Unleash VoicePower</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/choosing-language-bots-for-work-bing-chat-or-chatgpt-9-factors/"><u>Choosing Language Bots for Work: Bing Chat or ChatGPT? 9 Factors</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/coding-conversations-innovative-applications-of-chatgpt-in-game-writing/"><u>Coding Conversations: Innovative Applications of ChatGPT in Game Writing</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/complete-guide-for-recovering-contacts-files-on-lava-yuva-3-pro-by-fonelab-android-recover-contacts/"><u>Complete guide for recovering contacts files on Lava Yuva 3 Pro.</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/deciphering-the-risk-ai-and-the-perils-of-prompt-injection/"><u>Deciphering the Risk: AI and the Perils of Prompt Injection</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/deepen-relationships-with-emotional-intelligence-assistance/"><u>Deepen Relationships with Emotional Intelligence Assistance</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/end-your-gpt-engagement-instructions-here/"><u>End Your GPT Engagement: Instructions Here</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/envisioning-virtual-vigilance-projected-trends-in-security/"><u>Envisioning Virtual Vigilance: Projected Trends in Security</u></a></li>
<li><a href="https://change-location.techidaily.com/here-are-some-of-the-best-pokemon-discord-servers-to-join-on-vivo-y17s-drfone-by-drfone-virtual-android/"><u>Here are Some of the Best Pokemon Discord Servers to Join On Vivo Y17s | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-usechatgpts-co-pilot-expands-ai-capabilities-in-conversations/"><u>How UseChatGPT's Co-Pilot Expands AI Capabilities in Conversations</u></a></li>
<li><a href="https://review-topics.techidaily.com/in-2024-complete-tutorial-to-use-gps-joystick-to-fake-gps-location-on-infinix-hot-30i-drfone-by-drfone-virtual-android/"><u>In 2024, Complete Tutorial to Use GPS Joystick to Fake GPS Location On Infinix Hot 30i | Dr.fone</u></a></li>
<li><a href="https://screen-capture.techidaily.com/in-2024-comprehensive-list-top-screenshot-videography-tools/"><u>In 2024, Comprehensive List  Top Screenshot Videography Tools</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/in-2024-how-to-mirror-oppo-a1-5g-to-mac-drfone-by-drfone-android/"><u>In 2024, How to Mirror Oppo A1 5G to Mac? | Dr.fone</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/in-2024-launching-your-first-product-critique-network-a-step-by-step-guide/"><u>In 2024, Launching Your First Product Critique Network  A Step-by-Step Guide</u></a></li>
<li><a href="https://unlock-android.techidaily.com/in-2024-lock-your-vivo-v30-pro-phone-in-style-the-top-5-gesture-lock-screen-apps-by-drfone-android/"><u>In 2024, Lock Your Vivo V30 Pro Phone in Style The Top 5 Gesture Lock Screen Apps</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/in-2024-sim-unlock-tecno-spark-10-pro-phones-without-code-2-ways-to-remove-android-sim-lock-by-drfone-android/"><u>In 2024, Sim Unlock Tecno Spark 10 Pro Phones without Code 2 Ways to Remove Android Sim Lock</u></a></li>
<li><a href="https://youtube-help.techidaily.com/in-2024-speedy-transformation-from-pixels-to-polished-youtube-thumbnails/"><u>In 2024, Speedy Transformation  From Pixels to Polished YouTube Thumbnails</u></a></li>
<li><a href="https://android-unlock.techidaily.com/in-2024-unlocking-the-power-of-smart-lock-a-beginners-guide-for-samsung-users-by-drfone-android/"><u>In 2024, Unlocking the Power of Smart Lock A Beginners Guide for Samsung Users</u></a></li>
<li><a href="https://win11-tips.techidaily.com/learn-to-lead-teams-with-winning-strategies-free-style/"><u>Learn to Lead Teams with Winning Strategies, Free Style</u></a></li>
<li><a href="https://extra-approaches.techidaily.com/mastering-xstudio-complete-video-setup-analysis-for-2024/"><u>Mastering XStudio  Complete Video Setup Analysis for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-your-cover-letter-the-chatgpt-way/"><u>Mastering Your Cover Letter: The ChatGPT Way</u></a></li>
<li><a href="https://common-error.techidaily.com/overcoming-unstable-visual-glitches-in-your-windows-10-device/"><u>Overcoming Unstable Visual Glitches in Your Windows 10 Device</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/pioneering-customer-service-integrating-chatgpt-in-whatsapp/"><u>Pioneering Customer Service: Integrating ChatGPT in WhatsApp</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/redefining-smarts-outsmarting-a-machine-oracle/"><u>Redefining Smarts: Outsmarting a Machine Oracle</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/sign-up-simplified-bypassing-mobile-numbers-on-apps/"><u>Sign-Up Simplified: Bypassing Mobile Numbers on Apps</u></a></li>
<li><a href="https://win-blog.techidaily.com/step-by-step-troubleshooting-tips-for-restoring-compromised-pc-gaming-files/"><u>Step-by-Step Troubleshooting Tips for Restoring Compromised PC Gaming Files</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-art-and-science-of-paperclip-optimization-in-ais-ecosystem/"><u>The Art and Science of Paperclip Optimization in AI's Ecosystem</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-art-of-saving-chatgpt-messages-incognito/"><u>The Art of Saving ChatGPT Messages Incognito</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/top-7-virtual-gadgets-for-excelling-at-instruction-design/"><u>Top 7 Virtual Gadgets for Excelling at Instruction Design</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/transform-your-ideas-into-engaging-presentations-via-chatgpt/"><u>Transform Your Ideas Into Engaging Presentations via ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/transforming-industries-through-chatgpt-and-whisper-apis/"><u>Transforming Industries Through ChatGPT and Whisper APIs</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unleashing-potential-effective-chatgpt-use-on-macs/"><u>Unleashing Potential: Effective ChatGPT Use on Macs</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveil-ais-secrets-at-bing-simple-user-registration-path/"><u>Unveil AI's Secrets at Bing: Simple User Registration Path</u></a></li>
<li><a href="https://sound-tweaking.techidaily.com/updated-the-sound-engineers-approach-to-detaching-bass-from-mixed-tracks-for-2024/"><u>Updated The Sound Engineers Approach to Detaching Bass From Mixed Tracks for 2024</u></a></li>
<li><a href="https://video-ai-editor.techidaily.com/updated-transform-your-footage-a-beginners-guide-to-flipping-clips-in-fcp/"><u>Updated Transform Your Footage A Beginners Guide to Flipping Clips in FCP</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/ways-to-trade-pokemon-go-from-far-away-on-oneplus-11r-drfone-by-drfone-virtual-android/"><u>Ways to trade pokemon go from far away On OnePlus 11R? | Dr.fone</u></a></li>
<li><a href="https://apple-account.techidaily.com/why-apple-account-disabled-on-your-apple-iphone-15-pro-how-to-fix-by-drfone-ios/"><u>Why Apple Account Disabled On your Apple iPhone 15 Pro? How to Fix</u></a></li>
</ul></div>
