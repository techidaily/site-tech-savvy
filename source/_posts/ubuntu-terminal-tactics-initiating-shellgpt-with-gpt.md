---
title: "Ubuntu Terminal Tactics: Initiating ShellGPT with GPT"
date: 2024-07-20T06:22:49.933Z
updated: 2024-07-21T06:22:49.933Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Ubuntu Terminal Tactics: Initiating ShellGPT with GPT"
excerpt: "This Article Describes Ubuntu Terminal Tactics: Initiating ShellGPT with GPT"
thumbnail: https://thmb.techidaily.com/5101a256be44324944567b3cdefbcb470dad072a31cdc714305925ec88d3af54.jpg
---

## Ubuntu Terminal Tactics: Initiating ShellGPT with GPT

 Artificial intelligence has emerged as a new-age sensation, leaving everything behind in the dust. With new additions daily, there is a lot to look forward to.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 People use this multi-faceted, ubiquitous tool to crack jokes, write codes and even answer the most random questions. It’s easy to use ChatGPT on other OSes, so, as a Linux user, why should you stay behind?

 You too can enjoy ChatGPT’s Linux avatar, ShellGPT. Here's how to install and use the AI tool from your Ubuntu terminal in a few easy steps.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4940317&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/333ac5d90817d69113471fbb6e531bee/sps-partnership-728x90eng.png" border="0"></a>
<!-- affiliate ads end -->
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

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4699091&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/bccefcc1b1eee9eca3ae4f5c1a281482/products/1_jutoh-logo-1200x1600.jpg" border="0">Jutoh Plus -  Jutoh is an ebook creator for Epub, Kindle and more. It's fast, runs on Windows, Mac, and Linux, comes with a cover design editor, and allows book variations to be created with alternate text, style sheets and cover designs. Jutoh Plus adds scripting so you can automate ebook import and creation operations. It also allows customisation of ebook HTML via templates and source code documents; and you can create Windows CHM and wxWidgets HTB help files. </a>
<!-- affiliate ads end -->
![Ubuntu terminal window code snippets](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/install-virtual-environment-module-in-ubuntu.jpg)

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

<!-- affiliate ads begin -->
<a href="https://twopages.pxf.io/c/5597632/2016067/18544" target="_top" id="2016067"><img src="//a.impactradius-go.com/display-ad/18544-2016067" border="0" alt="" width="1020" height="380"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2016067/18544" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![Ubuntu terminal window with code snippets](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/enable-virtual-environment-for-shellgpt-in-ubuntu-1.jpg)

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2068411/7443" target="_top" id="2068411"><img src="//a.impactradius-go.com/display-ad/7443-2068411" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2068411/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Step 3: Generate an OpenAPI Key

 Since the virtual environment is ready, you must connect the OpenAI services and your Ubuntu machine to run ShellGPT. For this purpose, you must navigate to [OpenAI's website](https://openai.com/) and create an account there.

 If you have an existing account, you can log in with your credentials and navigate to your profile image, located on the top right-hand side of the website.

 Click on **View API Keys**, followed by **Create new secret key**.

<!-- affiliate ads begin -->
<a href="https://dhgate.sjv.io/c/5597632/1678785/12108" target="_top" id="1678785"><img src="//a.impactradius-go.com/display-ad/12108-1678785" border="0" alt="" width="300" height="250"/></a>
<!-- affiliate ads end -->
![OpenAI website interface showing a drop-down menu](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/view-api-keys-on-openai-website.jpg)

 Do not share this key with anyone since the connection is private and should be used on your machine only.

 Copy the API key from the dialog box, and save it somewhere, since you won't be able to review the same key again.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2087394/7443" target="_top" id="2087394"><img src="//a.impactradius-go.com/display-ad/7443-2087394" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2087394/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
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
<a href="https://estore.winxdvd.com/order/checkout.php?PRODS=12653853&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/bcb41ccdc4363c6848a1d760f26c28a0/products/14_videoproc-converter-ai-box.png" border="0"></a>
<!-- affiliate ads end -->
## Step 5: Install ShellGPT on Ubuntu

 Once all the installation formalities are complete, you can simply move on to the best part, the ShellGPT installation. The installation steps are quite straightforward, and you can install the tool with the following command:

`pip3 install shell-gpt`

![Installation snippet on ubuntu's terminal screen](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/install-shell-gpt-on-ubuntu.jpg)

 Let the installation finish; meanwhile, you can check out some interesting ways to use the AI tool via your terminal window.

## Using ShellGPT for Running Queries via the Terminal

 The entire purpose of installing ShellGPT is to make your life easier. To use the terminal as a search engine and run some queries, you can use the **sgpt** command, followed by your query within quotes:

`sgpt "How many galaxies exist within the universe"`

<!-- affiliate ads begin -->
<a href="https://imp.i110150.net/c/5597632/924299/11305" target="_top" id="924299"><img src="//a.impactradius-go.com/display-ad/11305-924299" border="0" alt="" width="520" height="100"/></a>
<!-- affiliate ads end -->
![Ubuntu terminal interface with a query response](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/shellgpt-query-reponse.jpg)

## Using ShellGPT for Generating Code

 You can use your ShellGPT for generating code as well. You can do it by passing the right command with the **sgpt** command:

`sgpt --code "print the Fibonacci series"`

![Ubuntu terminal window with code snippets](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/shellgpt-code-reponse.jpg)

 The output consists of code you can execute within Python to generate the Fibonacci series.

<!-- affiliate ads begin -->
<a href="https://thefitville.pxf.io/c/5597632/1526796/15852" target="_top" id="1526796"><img src="//a.impactradius-go.com/display-ad/15852-1526796" border="0" alt="" width="1200" height="628"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1526796/15852" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://visual-screen-recording.techidaily.com/new-2024-approved-pcs-prime-screen-capture-software-ranked-1-5/"><u>[New] 2024 Approved  PC's Prime Screen Capture Software Ranked #1-#5</u></a></li>
<li><a href="https://screen-activity-recording.techidaily.com/new-2024-approved-top-windows-11-capture-tools-win-edition/"><u>[New] 2024 Approved  Top Windows 11 Capture Tools  Win Edition</u></a></li>
<li><a href="https://extra-hints.techidaily.com/new-beyond-reality-boundaries-the-vr-journey-continues/"><u>[New] Beyond Reality Boundaries  The VR Journey Continues</u></a></li>
<li><a href="https://instagram-video-files.techidaily.com/new-boost-cash-flow-with-these-5-instagram-hacks-for-2024/"><u>[New] Boost Cash Flow with These 5 Instagram Hacks for 2024</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/new-expert-take-on-camstudios-recorder-efficacy-for-2024/"><u>[New] Expert Take on CamStudio's Recorder Efficacy for 2024</u></a></li>
<li><a href="https://youtube-blog.techidaily.com/our-path-to-youtube-studio-the-editors-command-center/"><u>[New] Your Path to YouTube Studio  The Editor's Command Center</u></a></li>
<li><a href="https://vp-tips.techidaily.com/updated-mastering-your-adventures-with-top-6-head-mounted-cameras-by-gopro-for-2024/"><u>[Updated] Mastering Your Adventures with Top 6 Head-Mounted Cameras by GoPro for 2024</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/updated-open-access-mindful-harmonies/"><u>[Updated] Open Access Mindful Harmonies</u></a></li>
<li><a href="https://video-screen-grab.techidaily.com/updated-top-strategies-capturing-saving-and-sharing-ps4-experiences-for-2024/"><u>[Updated] Top Strategies  Capturing, Saving & Sharing PS4 Experiences for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/10-new-age-conversational-apps-outshining-gpt/"><u>10 New Age Conversational Apps Outshining GPT</u></a></li>
<li><a href="https://article-files.techidaily.com/2024-approved-ideal-starter-accessories-for-gopro-newbies/"><u>2024 Approved  Ideal Starter Accessories for GoPro Newbies</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/30-free-ai-services-revamp-your-email-strategy-today/"><u>30 Free AI Services: Revamp Your Email Strategy Today</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/7-exciting-bard-ai-features-announced-at-google-io-2023/"><u>7 Exciting Bard AI Features Announced at Google I/O 2023</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/8-challenges-can-gpt-enhance-your-side-hustle/"><u>8 Challenges: Can GPT Enhance Your Side Hustle?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-new-reality-crafted-by-machine-minds/"><u>A New Reality Crafted by Machine Minds</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-ethics-and-legal-responsibility/"><u>AI Ethics & Legal Responsibility</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-your-sidekick-crafting-epic-stories-through-chatgpts-aid/"><u>AI Your Sidekick: Crafting Epic Stories Through ChatGPT's Aid</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ais-influence-on-fake-news-proliferation/"><u>AI's Influence on Fake News Proliferation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ais-talent-at-mixing-the-chatgpt-challenge/"><u>AI’s Talent at Mixing: The ChatGPT Challenge</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/android-unlock-code-sim-unlock-your-oneplus-ace-2-phone-and-remove-locked-screen-by-drfone-android/"><u>Android Unlock Code Sim Unlock Your OnePlus Ace 2 Phone and Remove Locked Screen</u></a></li>
<li><a href="https://android-location-track.techidaily.com/best-anti-tracker-software-for-infinix-note-30-vip-drfone-by-drfone-virtual-android/"><u>Best Anti Tracker Software For Infinix Note 30 VIP | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/beyond-standard-the-top-10-customizations-for-chatgpt/"><u>Beyond Standard: The Top 10 Customizations for ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/choosing-the-right-llm-unraveling-the-pros-and-cons-quickly/"><u>Choosing the Right LLM: Unraveling the Pros & Cons Quickly</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/debunking-chatgpts-wisdom-remains-unaltered/"><u>Debunking: ChatGPT's Wisdom Remains Unaltered</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/demystifying-nlp-mastery-comparing-gpt-and-bert-systems/"><u>Demystifying NLP Mastery: Comparing GPT and BERT Systems</u></a></li>
<li><a href="https://youtube-webster.techidaily.com/te-views-premium-hashtags-to-spark-virality-in-video-snippets/"><u>Elevate Views  Premium Hashtags to Spark Virality in Video Snippets</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/everyday-language-on-ai/"><u>Everyday Language on AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/free-gpt-4-for-everyone-nonetheless-select-plus-membership-continues-to-provide-unique-services/"><u>Free GPT-4 for Everyone; Nonetheless, Select Plus Membership Continues to Provide Unique Services</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/freelancers-guide-to-mastering-ai-assistantsbing-chat-vs-chatgpt/"><u>Freelancer's Guide to Mastering AI Assistants—Bing Chat Vs. ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/from-words-to-waves-mastering-sound-synthesis-via-ai/"><u>From Words to Waves: Mastering Sound Synthesis via AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721425749303-gpt-4-unlocked-for-all-yet-6-chatgpt-plus-advantages-remain/"><u>GPT-4: Unlocked For All, Yet 6 ChatGPT Plus Advantages Remain</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/harness-the-power-of-ai-the-best-pdf-extensions-ranked/"><u>Harness the Power of AI: The Best PDF Extensions Ranked</u></a></li>
<li><a href="https://easy-unlock-android.techidaily.com/how-to-change-lock-screen-wallpaper-on-nubia-red-magic-9-proplus-by-drfone-android/"><u>How to Change Lock Screen Wallpaper on Nubia Red Magic 9 Pro+</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-fix-the-chatgpt-is-at-capacity-right-now-error-on-windows/"><u>How to Fix the ChatGPT Is at Capacity Right Now Error on Windows</u></a></li>
<li><a href="https://review-topics.techidaily.com/how-to-leave-a-life360-group-on-xiaomi-redmi-a2plus-without-anyone-knowing-drfone-by-drfone-virtual-android/"><u>How To Leave a Life360 Group On Xiaomi Redmi A2+ Without Anyone Knowing? | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-seamlessly-integrate-microsoft-copilot-on-a-macbook-pro/"><u>How to Seamlessly Integrate Microsoft Copilot on a MacBook Pro</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/important-8-gpt-advice-for-enhancing-concentration-in-a-digital-era/"><u>Important 8 GPT Advice for Enhancing Concentration in a Digital Era</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/in-2024-ways-to-find-unlocking-codes-for-oneplus-12r-phones-by-drfone-android/"><u>In 2024, Ways To Find Unlocking Codes For OnePlus 12R Phones</u></a></li>
<li><a href="https://extra-support.techidaily.com/mp4-reimagined-effortlessly-adding-srt-for-2024/"><u>MP4 Reimagined  Effortlessly Adding SRT for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/narrative-navigators-face-off-gpt-versus-google-bard/"><u>Narrative Navigators Face-Off: GPT Versus Google Bard</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/painting-with-purpose-mastering-ai-art-through-chatgpt/"><u>Painting with Purpose: Mastering AI Art Through ChatGPT</u></a></li>
<li><a href="https://extra-support.techidaily.com/premium-15-high-resolution-camcorders-reviewed-for-2024/"><u>Premium 15 High-Resolution Camcorders Reviewed for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/reimagine-your-note-taking-chatgpts-revolutionary-method/"><u>Reimagine Your Note Taking - ChatGPT's Revolutionary Method</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/reimagining-ai-scrutiny-post-turing-test-paradigm-shift/"><u>Reimagining AI Scrutiny Post-Turing Test Paradigm Shift</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/securing-data-amidst-tailored-chatgpt-models/"><u>Securing Data Amidst Tailored ChatGPT Models</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-ultimate-guide-resolving-chatgpt-login-obstructions/"><u>The Ultimate Guide: Resolving ChatGPT Login Obstructions</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/top-8-chrome-productivity-boosts-with-cutting-edge-ai-technology/"><u>Top 8 Chrome Productivity Boosts with Cutting-Edge AI Technology</u></a></li>
<li><a href="https://remote-screen-capture.techidaily.com/unleashing-the-full-potential-of-webcams/"><u>Unleashing the Full Potential of Webcams</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-the-facts-gpts-limitations-in-crypto-research/"><u>Unveiling the Facts: GPT's Limitations in Crypto Research</u></a></li>
<li><a href="https://audio-shaping.techidaily.com/updated-in-2024-how-to-record-voice-on-mac-easy-to-use-guide/"><u>Updated In 2024, How to Record Voice on Mac? Easy-to-Use Guide</u></a></li>
</ul></div>
