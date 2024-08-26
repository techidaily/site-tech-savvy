---
title: "OpenAI's Chatbot at Your Fingertips: Using Ubuntu Bash and ShellGPT"
date: 2024-08-25T17:37:16.571Z
updated: 2024-08-26T17:37:16.571Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes OpenAI's Chatbot at Your Fingertips: Using Ubuntu Bash and ShellGPT"
excerpt: "This Article Describes OpenAI's Chatbot at Your Fingertips: Using Ubuntu Bash and ShellGPT"
thumbnail: https://thmb.techidaily.com/50e7f76f2c8c66324cf56beba95ae0c6f844a64c10ab3c9dc2a6921d3a267281.jpg
---

## OpenAI's Chatbot at Your Fingertips: Using Ubuntu Bash and ShellGPT

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
<a href="https://store.bitdefender.com/affiliate.php?ACCOUNT=BITLATIN&AFFILIATE=108875&PATH=http%3A%2F%2Fwww.bitdefender.com%2Fbusiness%3FAFFILIATE%3D108875%26RESOURCE%3D30%2525%2BOff%2Ball%2BGravityZone%2BProducts"><img src="https://www.bitdefender.com/content/dam/bitdefender/business/campaign/1200X628.png" border="0"></a>
<!-- affiliate ads end -->
## Step 2: Install and Set Up a Virtual Environment Using Python

 Now that Python and PIP are ready, you can set up Python's virtual environment to make the machine environment conducive for installing and running ShellGPT. Virtual environments are ideal for running isolated programs since they can avoid library conflicts.

 With a virtual environment in tow, you can limit the interactions between your system's and virtual environment's programs while performing different executions in silos.

 Using a virtual environment is an optional step, to avoid any unforeseen mishaps while installing and using Python libraries.

 To create a virtual environment using Python, you need to install the **venv** module:

`sudo apt install python3-venv -y`

![Ubuntu terminal window code snippets](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/install-virtual-environment-module-in-ubuntu.jpg)

<!-- affiliate ads begin -->
<a href="https://ursime.pxf.io/c/5597632/2048972/16384" target="_top" id="2048972"><img src="//a.impactradius-go.com/display-ad/16384-2048972" border="0" alt="" width="1200" height="900"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2048972/16384" style="position:absolute;visibility:hidden;" border="0" />
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

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4631056&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/997e65474a248252883b485717f7d098/products/buy-windows.png" border="0">Allavsoft Batch Download Online Videos, Music Offline to MP4, MP3, MOV, etc format </a>
<!-- affiliate ads end -->
## Step 3: Generate an OpenAPI Key

 Since the virtual environment is ready, you must connect the OpenAI services and your Ubuntu machine to run ShellGPT. For this purpose, you must navigate to [OpenAI's website](https://openai.com/) and create an account there.

 If you have an existing account, you can log in with your credentials and navigate to your profile image, located on the top right-hand side of the website.

 Click on **View API Keys**, followed by **Create new secret key**.

![OpenAI website interface showing a drop-down menu](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/view-api-keys-on-openai-website.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=194977&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.blumentals.net/scrfactory/images/screensaver-software.png" border="0">Screensaver Factory, Create stunning professional screensavers within minutes. Create screensavers for yourself, for marketing or unlimited royalty-free commercial distribution. Make screensavers from images, video and swf flash, add background music and smooth sprite and transition effects. Screensaver Factory is very easy to use, and it enables you to make self-installing screensaver files and CDs for easy setup and distribution. Screensaver Factory is the most advanced software of its kind.</a>
<!-- affiliate ads end -->
 Do not share this key with anyone since the connection is private and should be used on your machine only.

 Copy the API key from the dialog box, and save it somewhere, since you won't be able to review the same key again.

![OpenAI's secret key website page with an open dialog box](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/generate-api-secret-key.jpg)

 To establish a connection on your Ubuntu machine, create an environment variable with the **export** command:

`export OPENAI_API_KEY=<paste key details here>`

<!-- affiliate ads begin -->
<a href="https://aidotcom.pxf.io/c/5597632/2086436/19576" target="_top" id="2086436"><img src="//a.impactradius-go.com/display-ad/19576-2086436" border="0" alt="" width="1500" height="400"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2086436/19576" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
### Add and Verify the API Key Into a Virtual Environment Variable

 When you execute the API key in this manner, Linux will use it only for a single instance. However, if you want to make the execution permanent, save it in the **.bashrc** file.

 All you have to do is type in the first command and enter the subsequent command within the text editor:

`nano ./bashrc  
export OPENAI_API_KEY=<paste key details here>`

![Ubuntu terminal window with code snippets to create and save an environment variable](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/create-an-environment-variable-1.jpg)

<!-- affiliate ads begin -->
<a href="https://martinic.evyy.net/c/5597632/1422856/4482" target="_top" id="1422856"><img src="//a.impactradius-go.com/display-ad/4482-1422856" border="0" alt="" width="580" height="309"/></a>
<!-- affiliate ads end -->
 Save and exit the editor. Then, use the source command to enable the changes.

`source ./bashrc`

 Finally, verify the API key with the **env** command.

`env`

![List of variables in a linux terminal](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/check-secret-key-in-env-list.jpg)

 Your **OPENAI\_API\_KEY** environment variable should be listed in the output.

## Step 5: Install ShellGPT on Ubuntu

 Once all the installation formalities are complete, you can simply move on to the best part, the ShellGPT installation. The installation steps are quite straightforward, and you can install the tool with the following command:

`pip3 install shell-gpt`

![Installation snippet on ubuntu's terminal screen](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/install-shell-gpt-on-ubuntu.jpg)

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2087389/7443" target="_top" id="2087389"><img src="//a.impactradius-go.com/display-ad/7443-2087389" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2087389/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 Let the installation finish; meanwhile, you can check out some interesting ways to use the AI tool via your terminal window.

## Using ShellGPT for Running Queries via the Terminal

 The entire purpose of installing ShellGPT is to make your life easier. To use the terminal as a search engine and run some queries, you can use the **sgpt** command, followed by your query within quotes:

`sgpt "How many galaxies exist within the universe"`

![Ubuntu terminal interface with a query response](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/shellgpt-query-reponse.jpg)

## Using ShellGPT for Generating Code

 You can use your ShellGPT for generating code as well. You can do it by passing the right command with the **sgpt** command:

`sgpt --code "print the Fibonacci series"`

![Ubuntu terminal window with code snippets](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/shellgpt-code-reponse.jpg)

 The output consists of code you can execute within Python to generate the Fibonacci series.

<!-- affiliate ads begin -->
<a href="https://order.glarysoft.com/order/checkout.php?PRODS=4691139&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/6734fa703f6633ab896eecbdfad8953a/products/SU-200-1.png" border="0">Software Update Pro - Check and update software installed on your computer. </a>
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
<li><a href="https://tech-savvy.techidaily.com/ais-new-gear-the-chatgpt-plus-plan-20-mo-just-for-the-usa/"><u>AI's New Gear: The ChatGPT Plus Plan ($20 Mo), Just for the USA</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/breaking-free-setting-up-gpt-on-windows/"><u>Breaking Free: Setting Up GPT on Windows</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpts-impact-on-writing-quality/"><u>ChatGPT's Impact on Writing Quality</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/decoding-the-puzzle-the-interplay-between-paperclips-and-artificial-intelligence/"><u>Decoding the Puzzle: The Interplay Between Paperclips & Artificial Intelligence</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/demonstrating-gpts-real-world-value/"><u>Demonstrating GPT's Real-World Value</u></a></li>
<li><a href="https://techtrends.techidaily.com/discover-12-fantastic-free-streamers-for-your-favorite-films/"><u>Discover 12 Fantastic Free Streamers for Your Favorite Films</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/elites-take-the-future-of-global-ai-technology/"><u>Elite's Take: The Future of Global AI Technology</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/enterprises-evolve-with-open-access-to-chatgpt-whisper-apis/"><u>Enterprises Evolve with Open Access to ChatGPT, Whisper APIs</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/essential-tips-for-overcoming-chatgpt-logout-issues/"><u>Essential Tips for Overcoming ChatGPT Logout Issues</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/examining-chatgpts-privacy-concerns/"><u>Examining ChatGPT's Privacy Concerns</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/false-chatbots-spotted-potential-hackers-lurk-in-disguise/"><u>False ChatBots Spotted: Potential Hackers Lurk in Disguise</u></a></li>
<li><a href="https://youtube-clips.techidaily.com/flash-share-sharing-playlists-in-a-snap/"><u>Flash-Share  Sharing Playlists in a Snap</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/gpt-4s-revolutionary-path-to-everyone/"><u>GPT-4's Revolutionary Path to Everyone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/hacked-heroes-the-activision-incident/"><u>Hacked Heroes: The Activision Incident</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/how-to-mirror-oppo-reno-11-5g-to-mac-drfone-by-drfone-android/"><u>How to Mirror Oppo Reno 11 5G to Mac? | Dr.fone</u></a></li>
<li><a href="https://blog-min.techidaily.com/how-to-remove-remote-management-from-iphone-8-plus-by-drfone-ios-unlock-ios-unlock/"><u>How to Remove remote management from iPhone 8 Plus?</u></a></li>
<li><a href="https://some-techniques.techidaily.com/ideal-iphoneandroid-faceshaping-software-for-2024/"><u>Ideal iPhone/Android Faceshaping Software for 2024</u></a></li>
<li><a href="https://location-social.techidaily.com/in-2024-how-to-change-location-on-tiktok-to-see-more-content-on-your-poco-m6-5g-drfone-by-drfone-virtual-android/"><u>In 2024, How to Change Location on TikTok to See More Content On your Poco M6 5G | Dr.fone</u></a></li>
<li><a href="https://unlock-android.techidaily.com/in-2024-how-to-unlock-honor-magic-6-phone-without-google-account-by-drfone-android/"><u>In 2024, How to Unlock Honor Magic 6 Phone without Google Account?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/leveraging-conversational-tech-to-boost-work-output/"><u>Leveraging Conversational Tech to Boost Work Output</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/maximizing-chatgpt-potential-via-apples-siri/"><u>Maximizing ChatGPT Potential via Apple's Siri</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/navigating-the-digital-age-why-teachers-should-become-ai-allies-8-reasons/"><u>Navigating the Digital Age: Why Teachers Should Become AI Allies (8 Reasons)</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/pioneering-ai-how-vector-databases-make-a-difference/"><u>Pioneering AI: How Vector Databases Make a Difference</u></a></li>
<li><a href="https://facebook.techidaily.com/safety-first-selecting-a-secure-site/"><u>Safety First: Selecting a Secure Site</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/script-synergy-6-creative-uses-for-chatgpt-in-video-games/"><u>Script Synergy: 6 Creative Uses for ChatGPT in Video Games</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/spotting-bogus-ai-in-conversations-via-gpt-notation/"><u>Spotting Bogus AI in Conversations via GPT Notation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/strong-vs-weak-ai-decoding-the-distinction/"><u>Strong Vs. Weak AI: Decoding the Distinction</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-great-ai-debate-whos-best-gpt-vs-microsoftgoogles-innovations/"><u>The Great AI Debate: Who's Best? GPT Vs. Microsoft/Google's Innovations</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/the-magnificent-art-of-pokemon-go-streaming-on-tecno-pop-8-drfone-by-drfone-virtual-android/"><u>The Magnificent Art of Pokemon Go Streaming On Tecno Pop 8? | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/transform-your-mobile-experience-with-bings-smart-search-technology/"><u>Transform Your Mobile Experience with Bing's Smart Search Technology</u></a></li>
<li><a href="https://tech-revival.techidaily.com/unveiling-6-capabilities-with-gpts-code-conductor/"><u>Unveiling 6 Capabilities with GPT's Code Conductor</u></a></li>
</ul></div>
