---
title: "Bypassing User Interface: Direct Engagement Through ShellGPT"
date: 2024-07-20T06:23:34.588Z
updated: 2024-07-21T06:23:34.588Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Bypassing User Interface: Direct Engagement Through ShellGPT"
excerpt: "This Article Describes Bypassing User Interface: Direct Engagement Through ShellGPT"
thumbnail: https://thmb.techidaily.com/51b5c705b272c6a35f26cbee92033b8d25124b814164fccb1a1f598c30e520f7.jpg
---

## Bypassing User Interface: Direct Engagement Through ShellGPT

 Artificial intelligence has emerged as a new-age sensation, leaving everything behind in the dust. With new additions daily, there is a lot to look forward to.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 People use this multi-faceted, ubiquitous tool to crack jokes, write codes and even answer the most random questions. It’s easy to use ChatGPT on other OSes, so, as a Linux user, why should you stay behind?

 You too can enjoy ChatGPT’s Linux avatar, ShellGPT. Here's how to install and use the AI tool from your Ubuntu terminal in a few easy steps.

<!-- affiliate ads begin -->
<a href="https://funwhole.sjv.io/c/5597632/1702887/17189" target="_top" id="1702887"><img src="//a.impactradius-go.com/display-ad/17189-1702887" border="0" alt="" width="1000" height="1000"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1702887/17189" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## What’s ShellGPT, ChatGPT’s Equivalent Linux Namesake?

 ShellGPT, as it is more commonly known, is ChatGPT’s command-line equivalent, through which users can use and engage with the AI chatbot via their Linux terminal. The chatbot draws power from OpenAI’s Large Language Model, providing intelligent user recommendations.

 Large Language Models (LLMs) are becoming a hot topic of discussion since you can easily [run LLM-enabled chatbots on your Raspberry Pi](https://www.makeuseof.com/raspberry-pi-large-language-model/).

 Sounds intriguing, doesn’t it?

 If you have experience interacting with ChatGPT, you will love this alternate Linux shell version.

 What’s the benefit of installing ShellGPT on your machine? It’s simple; you don’t need to type in unnecessary long commands or head to your browser. Instead, you can perform all possible tasks from the comfort of your Linux terminal.

 Before installing ShellGPT on your Ubuntu machine, here are a few prerequisites to take care of.

<!-- affiliate ads begin -->
<a href="https://order.glarysoft.com/order/checkout.php?PRODS=35504869&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/6734fa703f6633ab896eecbdfad8953a/products/1_FR-200-1.png" border="0">Glarysoft File Recovery Pro Annually -  Helps to recover your lost file/data, even permanently deleted data. 
</a>
<!-- affiliate ads end -->
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

<!-- affiliate ads begin -->
<a href="https://store.revouninstaller.com/order/checkout.php?PRODS=28010250&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/4282ec8de8c9be897e7aff4aa231b1a4/336__280a.jpg" border="0"></a>
<!-- affiliate ads end -->
![OpenAI website interface showing a drop-down menu](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/view-api-keys-on-openai-website.jpg)

 Do not share this key with anyone since the connection is private and should be used on your machine only.

 Copy the API key from the dialog box, and save it somewhere, since you won't be able to review the same key again.

![OpenAI's secret key website page with an open dialog box](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/generate-api-secret-key.jpg)

 To establish a connection on your Ubuntu machine, create an environment variable with the **export** command:

`export OPENAI_API_KEY=<paste key details here>`

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2087267/19272" target="_top" id="2087267"><img src="//a.impactradius-go.com/display-ad/19272-2087267" border="0" alt="" width="728" height="90"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2087267/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
### Add and Verify the API Key Into a Virtual Environment Variable

 When you execute the API key in this manner, Linux will use it only for a single instance. However, if you want to make the execution permanent, save it in the **.bashrc** file.

 All you have to do is type in the first command and enter the subsequent command within the text editor:

`nano ./bashrc  
export OPENAI_API_KEY=<paste key details here>`

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4665597&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.pcclean.io/wp-content/uploads/2018/03/winutilities-box-130521.png" border="0">WinUtilities Pro</a>
<!-- affiliate ads end -->
![Ubuntu terminal window with code snippets to create and save an environment variable](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/create-an-environment-variable-1.jpg)

 Save and exit the editor. Then, use the source command to enable the changes.

`source ./bashrc`

 Finally, verify the API key with the **env** command.

`env`

![List of variables in a linux terminal](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/check-secret-key-in-env-list.jpg)

 Your **OPENAI\_API\_KEY** environment variable should be listed in the output.

<!-- affiliate ads begin -->
<a href="https://twopages.pxf.io/c/5597632/2016067/18544" target="_top" id="2016067"><img src="//a.impactradius-go.com/display-ad/18544-2016067" border="0" alt="" width="1020" height="380"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2016067/18544" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Step 5: Install ShellGPT on Ubuntu

 Once all the installation formalities are complete, you can simply move on to the best part, the ShellGPT installation. The installation steps are quite straightforward, and you can install the tool with the following command:

`pip3 install shell-gpt`

<!-- affiliate ads begin -->
<a href="https://zebaoaffiliateprogram.pxf.io/c/5597632/1853659/21526" target="_top" id="1853659"><img src="//a.impactradius-go.com/display-ad/21526-1853659" border="0" alt="" width="1920" height="750"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1853659/21526" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![Installation snippet on ubuntu's terminal screen](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/install-shell-gpt-on-ubuntu.jpg)

 Let the installation finish; meanwhile, you can check out some interesting ways to use the AI tool via your terminal window.

<!-- affiliate ads begin -->
<a href="https://estore.winxdvd.com/order/checkout.php?PRODS=12653808&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.winxdvd.com/affiliate/new-banner/wt-500x500.jpg" border="0"></a>
<!-- affiliate ads end -->
## Using ShellGPT for Running Queries via the Terminal

 The entire purpose of installing ShellGPT is to make your life easier. To use the terminal as a search engine and run some queries, you can use the **sgpt** command, followed by your query within quotes:

`sgpt "How many galaxies exist within the universe"`

![Ubuntu terminal interface with a query response](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/shellgpt-query-reponse.jpg)

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
<li><a href="https://fox-glue.techidaily.com/new-2024-approved-8-best-free-mp3-downloader-for-android/"><u>[New] 2024 Approved  8 Best Free MP3 Downloader for Android</u></a></li>
<li><a href="https://article-tips.techidaily.com/new-pros-and-cons-of-inshot-is-it-the-ultimate-editor-for-2024/"><u>[New] Pros and Cons of InShot  Is It the Ultimate Editor for 2024</u></a></li>
<li><a href="https://facebook-video-footage.techidaily.com/new-understanding-satire-building-parodies-online/"><u>[New] Understanding Satire  Building Parodies Online</u></a></li>
<li><a href="https://twitter-clips.techidaily.com/new-youtube-like-audio-making-via-twitter/"><u>[New] YouTube-Like Audio Making via Twitter</u></a></li>
<li><a href="https://video-capture.techidaily.com/updated-2024-approved-nocostcam-the-infinite-gaming-screen-record-tool/"><u>[Updated] 2024 Approved  NoCostCam  The Infinite Gaming Screen Record Tool</u></a></li>
<li><a href="https://facebook-video-footage.techidaily.com/updated-in-2024-craft-stellar-channels-best-10-apps-for-artistic-banner-design/"><u>[Updated] In 2024, Craft Stellar Channels  Best 10 Apps for Artistic Banner Design</u></a></li>
<li><a href="https://facebook-clips.techidaily.com/2024-approved-supercharge-your-social-sagas-free-seamless-online-integration/"><u>2024 Approved  Supercharge Your Social Sagas  FREE, Seamless Online Integration</u></a></li>
<li><a href="https://screen-sharing-recording.techidaily.com/2024-approved-using-inbuilt-recorders-for-screen-capture-on-huaweis-mate-and-p-series-devices/"><u>2024 Approved  Using Inbuilt Recorders for Screen Capture on Huawei's Mate and P Series Devices</u></a></li>
<li><a href="https://location-fake.techidaily.com/a-detailed-guide-on-faking-your-location-in-mozilla-firefox-on-realme-narzo-n55-drfone-by-drfone-virtual-android/"><u>A Detailed Guide on Faking Your Location in Mozilla Firefox On Realme Narzo N55 | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/blizzards-new-chapter-with-microsoft-unveils-innovative-use-of-ai-in-gaming-and-artistry-audio-analysis/"><u>Blizzard's New Chapter with Microsoft Unveils Innovative Use of AI in Gaming & Artistry [Audio Analysis]</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/can-users-influence-chatgpts-learning-process/"><u>Can Users Influence ChatGPT's Learning Process?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-love-lines-a-modern-approach-to-mates/"><u>ChatGPT Love Lines: A Modern Approach to Mates</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-the-ai-thats-revolutionizing-video-content-crafting/"><u>ChatGPT: The AI That's Revolutionizing Video Content Crafting</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/claude-vs-chatgpt-the-4-innovative-improvements-that-redefine-interaction/"><u>Claude vs ChatGPT: The 4 Innovative Improvements that Redefine Interaction</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/cutting-edge-designs-top-8-popular-instagram-template-groups-for-2024/"><u>Cutting Edge Designs  Top 8 Popular Instagram Template Groups for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/decoding-5-key-reasons-companies-shy-away-from-gpt-applications/"><u>Decoding 5 Key Reasons Companies Shy Away From GPT Applications</u></a></li>
<li><a href="https://extra-resources.techidaily.com/elaborate-inspection-gopro-silver-hero4-unit-test/"><u>Elaborate Inspection  GoPro Silver HERO4 Unit Test</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/elevate-your-abodes-productivity-with-chatgpt-techniques/"><u>Elevate Your Abode's Productivity with ChatGPT Techniques</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/essential-overlooked-gpt-features-for-innovative-dialogue/"><u>Essential, Overlooked GPT Features for Innovative Dialogue</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/fostering-fiction-6-ways-to-harness-chatgpt/"><u>Fostering Fiction: 6 Ways to Harness ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721431815367-free-access-now-however-platinum-plans-6-benefits-are-still-compelling/"><u>Free Access Now! However, Platinum Plan's 6 Benefits Are Still Compelling.</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721423078139-from-bots-to-iphones-chatgpt-arrives/"><u>From Bots to iPhones: ChatGPT Arrives</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/gemini-elite-vs-powered-chatgpt/"><u>Gemini Elite Vs. Powered ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-create-user-personas-in-chatgpt-for-better-results/"><u>How to Create User Personas in ChatGPT for Better Results</u></a></li>
<li><a href="https://ios-location-track.techidaily.com/how-to-spy-on-text-messages-from-computer-and-apple-iphone-13-drfone-by-drfone-virtual-ios/"><u>How to Spy on Text Messages from Computer & Apple iPhone 13 | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/improving-blog-commentaries-with-ai-wisdom/"><u>Improving Blog Commentaries with AI Wisdom</u></a></li>
<li><a href="https://review-topics.techidaily.com/in-2024-how-can-i-use-a-fake-gps-without-mock-location-on-vivo-s18-pro-drfone-by-drfone-virtual-android/"><u>In 2024, How Can I Use a Fake GPS Without Mock Location On Vivo S18 Pro? | Dr.fone</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/in-2024-life360-learn-how-everything-works-on-asus-rog-phone-8-pro-drfone-by-drfone-virtual-android/"><u>In 2024, Life360 Learn How Everything Works On Asus ROG Phone 8 Pro | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/intellectual-frontier-can-computers-triumph/"><u>Intellectual Frontier: Can Computers Triumph?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/introducing-mac-friendly-communication-with-gpt/"><u>Introducing Mac-Friendly Communication with GPT</u></a></li>
<li><a href="https://audio-shaping.techidaily.com/linux-audio-cutting-edge-software-roundup-free-and-paid-options/"><u>Linux Audio Cutting-Edge Software Roundup Free & Paid Options</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/methodology-saving-the-dialogue-history-of-gpt-chat/"><u>Methodology: Saving the Dialogue History of GPT-Chat</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/navigating-the-features-of-llama-2-with-ease/"><u>Navigating the Features of Llama 2 with Ease</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/navigating-the-world-of-public-gpt-conversations/"><u>Navigating the World of Public GPT Conversations</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/optimal-communication-with-9-advantages-in-chatgptplus/"><u>Optimal Communication with 9 Advantages in ChatGPT+</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/optimizing-corporate-correspondence-via-ai-practical-tips-and-tricks/"><u>Optimizing Corporate Correspondence via AI: Practical Tips & Tricks</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/personalize-health-and-exercise-with-choosing-8-gpts/"><u>Personalize Health & Exercise with Choosing 8 GPTs</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/reality-assurance-no-gpt-windows-isnt-harmful-app/"><u>Reality Assurance: No, GPT-Windows Isn't Harmful App</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/six-budget-friendly-artificial-intelligence-options/"><u>Six Budget-Friendly Artificial Intelligence Options</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/study-smarter-not-harder-top-5-student-friendly-chatgpt-applications/"><u>Study Smarter, Not Harder: Top 5 Student-Friendly ChatGPT Applications</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/subtle-archiving-concealing-your-chatgpt-journey/"><u>Subtle Archiving: Concealing Your ChatGPT Journey</u></a></li>
<li><a href="https://some-approaches.techidaily.com/tactical-approach-for-finalizing-a-dormant-linkedin-profile-for-2024/"><u>Tactical Approach for Finalizing a Dormant LinkedIn Profile for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/tailored-talk-tech-enhancing-gpt-conversation-with-10-tweaks/"><u>Tailored Talk Tech: Enhancing GPT Conversation with 10 Tweaks</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/top-5-ai-driven-counseling-bots-for-emotional-wellness/"><u>Top 5 AI-Driven Counseling Bots for Emotional Wellness</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/transforming-physical-training-through-gpt-interaction/"><u>Transforming Physical Training Through GPT Interaction</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/virtual-emotional-support-guidelines-for-chatgpt-use/"><u>Virtual Emotional Support: Guidelines for ChatGPT Use</u></a></li>
</ul></div>
