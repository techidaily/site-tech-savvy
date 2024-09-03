---
title: Shell Command Guide to Engage with ChatGPT
date: 2024-09-02T20:40:49.511Z
updated: 2024-09-03T20:40:49.511Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Shell Command Guide to Engage with ChatGPT
excerpt: This Article Describes Shell Command Guide to Engage with ChatGPT
thumbnail: https://thmb.techidaily.com/dac11c6cc9fc4c74d0a91630c727d89a2865b8212237d761cabdd5e063687899.jpg
---

## Shell Command Guide to Engage with ChatGPT

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
<a href="https://ancheer.sjv.io/c/5597632/1657301/17326" target="_top" id="1657301"><img src="//a.impactradius-go.com/display-ad/17326-1657301" border="0" alt="" width="1920" height="933"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1657301/17326" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Step 2: Install and Set Up a Virtual Environment Using Python

 Now that Python and PIP are ready, you can set up Python's virtual environment to make the machine environment conducive for installing and running ShellGPT. Virtual environments are ideal for running isolated programs since they can avoid library conflicts.

 With a virtual environment in tow, you can limit the interactions between your system's and virtual environment's programs while performing different executions in silos.

 Using a virtual environment is an optional step, to avoid any unforeseen mishaps while installing and using Python libraries.

 To create a virtual environment using Python, you need to install the **venv** module:

`sudo apt install python3-venv -y`

![Ubuntu terminal window code snippets](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/install-virtual-environment-module-in-ubuntu.jpg)

<!-- affiliate ads begin -->
<a href="https://order.glarysoft.com/order/checkout.php?PRODS=35408920&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/6734fa703f6633ab896eecbdfad8953a/products/FR-200-1.png" border="0">Glarysoft File Recovery Pro - Helps to recover your lost file/data, even permanently deleted data. </a>
<!-- affiliate ads end -->
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

<!-- affiliate ads begin -->
<a href="https://uperfect.sjv.io/c/5597632/1246754/15155" target="_top" id="1246754"><img src="//a.impactradius-go.com/display-ad/15155-1246754" border="0" alt="" width="600" height="600"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1246754/15155" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
<!-- affiliate ads begin -->
<a href="https://shop.systoolsgroup.com/affiliate.php?ACCOUNT=SYSTOOBY&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.systoolsgroup.com%3FAFFILIATE%3D108875%26RESOURCE%3DSysTools%2BGmail%2BBackup"><img src="https://www.systoolsgroup.com/box/gmail-backup.png" border="0"></a>
<!-- affiliate ads end -->
## Step 3: Generate an OpenAPI Key

 Since the virtual environment is ready, you must connect the OpenAI services and your Ubuntu machine to run ShellGPT. For this purpose, you must navigate to [OpenAI's website](https://openai.com/) and create an account there.

 If you have an existing account, you can log in with your credentials and navigate to your profile image, located on the top right-hand side of the website.

 Click on **View API Keys**, followed by **Create new secret key**.

![OpenAI website interface showing a drop-down menu](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/view-api-keys-on-openai-website.jpg)

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2075461/7443" target="_top" id="2075461"><img src="//a.impactradius-go.com/display-ad/7443-2075461" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2075461/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 Do not share this key with anyone since the connection is private and should be used on your machine only.

 Copy the API key from the dialog box, and save it somewhere, since you won't be able to review the same key again.

![OpenAI's secret key website page with an open dialog box](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/generate-api-secret-key.jpg)

 To establish a connection on your Ubuntu machine, create an environment variable with the **export** command:

`export OPENAI_API_KEY=<paste key details here>`

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4721564&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/c14a8df1e1b4d5297e9cb30cb34d5a00/products/copy_power-tools-48.png" border="0">Power Tools add-on for Google Sheets, 12-month subscription</a>
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

 Your **OPENAI\_API\_KEY** environment variable should be listed in the output.

## Step 5: Install ShellGPT on Ubuntu

 Once all the installation formalities are complete, you can simply move on to the best part, the ShellGPT installation. The installation steps are quite straightforward, and you can install the tool with the following command:

`pip3 install shell-gpt`

![Installation snippet on ubuntu's terminal screen](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/install-shell-gpt-on-ubuntu.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4737285&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/b2f83c409ce63012229fb9cd465bdcfe/products/copy_reporting_system.png" border="0">  KoolReport Pro  is an advanced solution for creating data reports and dashboards in PHP. Equipped with all  extended packages , KoolReport Pro is able to connect to various datasources, perform advanced data analysis, construct stunning charts and graphs and export your beautiful work to PDF, Excel, JPG or other formats. Plus, it includes powerful built-in reports such as pivot report and drill-down report which will save your time in building ones. 

 It will help you to write dynamic data reports easily, to construct intuitive dashboards or to build a whole business intelligence cockpit. 

  KoolReport Pro  package goes with Full Source Code, Royal Free, ONE (1) Year Priority Support, ONE (1) Year Free Upgrade and 30-Days Money Back Guarantee. 

  Developer License  allows  Single Developer  to create Unlimited Reports, deploy on Unlimited Servers and able deliver the work to Unlimited Clients. </a>
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
<li><a href="https://desktop-recording.techidaily.com/new-2024-approved-high-ranking-nintendo-switch-brawlers-index-max-156/"><u>[New] 2024 Approved  High-Ranking Nintendo Switch Brawlers Index (Max 156)</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/new-travel-through-time-on-instagram-the-reverse-video-guide/"><u>[New] Travel Through Time on Instagram  The Reverse Video Guide</u></a></li>
<li><a href="https://facebook-clips.techidaily.com/updated-essential-tips-for-a-novice-using-facebook-analytics/"><u>[Updated] Essential Tips for a Novice Using Facebook Analytics</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-highpoint-masterpiece-suite/"><u>[Updated] Highpoint Masterpiece Suite</u></a></li>
<li><a href="https://facebook-video-recording.techidaily.com/updated-in-2024-easy-strategies-for-editing-social-media-banners/"><u>[Updated] In 2024, Easy Strategies for Editing Social Media Banners</u></a></li>
<li><a href="https://facebook-video-content.techidaily.com/updated-in-2024-leverage-your-xbox-gameplay-for-virtual-engagement-on-fb/"><u>[Updated] In 2024, Leverage Your Xbox Gameplay for Virtual Engagement on FB</u></a></li>
<li><a href="https://video-screen-grab.techidaily.com/updated-in-2024-unveiling-the-most-effective-zoom-recording-tools/"><u>[Updated] In 2024, Unveiling the Most Effective Zoom Recording Tools</u></a></li>
<li><a href="https://extra-support.techidaily.com/updated-lifetime-favorites-reddits-highly-endorsed-top-10/"><u>[Updated] Lifetime Favorites  Reddit's Highly-Endorsed Top 10</u></a></li>
<li><a href="https://video-capture.techidaily.com/updated-premium-android-screenshot-and-video-tools-ranked-five-for-2024/"><u>[Updated] Premium Android Screenshot & Video Tools - Ranked Five for 2024</u></a></li>
<li><a href="https://games-able.techidaily.com/1719163821039-10-hidden-gem-free-mobile-games-pure-fun/"><u>10 Hidden Gem Free Mobile Games - Pure Fun</u></a></li>
<li><a href="https://extra-information.techidaily.com/2024-approved-beginners-overview-of-animation-trends/"><u>2024 Approved  Beginner's Overview of Animation Trends</u></a></li>
<li><a href="https://remote-screen-capture.techidaily.com/2024-approved-enhance-gameplay-memories-win10-recording-methods/"><u>2024 Approved  Enhance Gameplay Memories  Win10 Recording Methods</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/advanced-rpg-strategies-using-ai-powered-chatgpt-help/"><u>Advanced RPG Strategies Using AI-Powered ChatGPT Help</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/avoiding-unoriginal-content-in-ai-dialogue/"><u>Avoiding Unoriginal Content in AI Dialogue</u></a></li>
<li><a href="https://desktop-recording.techidaily.com/best-of-the-best-top-12-tycoon-games-for-epic-victories/"><u>Best of the Best  Top 12 Tycoon Games for Epic Victories</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/china-dominates-with-local-processor-giant-behind-lenovos-latest-pc-lineup-plus-five-other-oems-embrace-zhoaxin-equipped-systems/"><u>China Dominates with Local Processor Giant Behind Lenovo's Latest PC Lineup; Plus, Five Other OEMs Embrace Zhoaxin-Equipped Systems</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/claudios-battle-for-productivity-gpt-vs-everyday-task-helper/"><u>Claudio's Battle for Productivity: GPT Vs. Everyday Task Helper</u></a></li>
<li><a href="https://fake-location.techidaily.com/does-life360-notify-when-you-log-out-on-vivo-v27e-drfone-by-drfone-virtual-android/"><u>Does Life360 Notify When You Log Out On Vivo V27e? | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/elevate-your-skycraft-copilot-pro-explained/"><u>Elevate Your Skycraft - Copilot Pro Explained</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ensuring-authenticity-reducing-ai-fabrications-with-specific-cues/"><u>Ensuring Authenticity: Reducing AI Fabrications with Specific Cues</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/excavate-new-reads-discover-these-5-leading-ai-powered-book-services/"><u>Excavate New Reads: Discover These 5 Leading AI-Powered Book Services</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/exploring-chatgpt-transforming-ideas-into-ai-generated-reality/"><u>Exploring ChatGPT: Transforming Ideas Into AI-Generated Reality</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/geminis-milestone-redefining-value-at-1m-tokens/"><u>Gemini's Milestone: Redefining Value at $1M Tokens</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/gpt-pluses-vs-perplexities-ais-top-contenders/"><u>GPT Pluses Vs. Perplexities: AI's Top Contenders</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/guide-to-flourishing-freeconversations-windows-edition/"><u>Guide to Flourishing FreeConversations: Windows Edition</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/guiding-audio-dimming-in-fl-studio-for-2024/"><u>Guiding Audio Dimming in FL Studio for 2024</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/in-2024-what-is-geo-blocking-and-how-to-bypass-it-on-apple-iphone-14-drfone-by-drfone-virtual-ios/"><u>In 2024, What is Geo-Blocking and How to Bypass it On Apple iPhone 14? | Dr.fone</u></a></li>
<li><a href="https://location-social.techidaily.com/in-2024-why-your-whatsapp-location-is-not-updating-and-how-to-fix-on-oppo-a1x-5g-drfone-by-drfone-virtual-android/"><u>In 2024, Why Your WhatsApp Location is Not Updating and How to Fix On Oppo A1x 5G | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/leaders-lens-on-ai-learning-ensuring-quality-with-4-checkpoints/"><u>Leader's Lens on AI Learning: Ensuring Quality with 4 Checkpoints</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/leveraging-links-for-your-ai-chat-experiences/"><u>Leveraging Links for Your AI Chat Experiences</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/love-in-a-digital-age-chatgpt-to-the-rescue/"><u>Love in a Digital Age: ChatGPT to the Rescue</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/navigating-wellness-wisely-top-7-uses-of-chatgpt/"><u>Navigating Wellness Wisely: Top 7 Uses of ChatGPT</u></a></li>
<li><a href="https://hardware-tips.techidaily.com/newly-launched-satechi-charger-stands-compatible-with-qi2-and-apples-magsafe/"><u>Newly Launched Satechi Charger Stands Compatible with Qi2 & Apple's MagSafe</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/numeric-excellence-excel-surpasses-gpt-in-complex-calculations/"><u>Numeric Excellence: Excel Surpasses GPT in Complex Calculations</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revolutionize-healthcare-and-nutrition-with-gpt-plugins/"><u>Revolutionize Healthcare & Nutrition with GPT Plugins</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revolutionizing-work-from-home-with-chatgpt-tactics/"><u>Revolutionizing Work From Home with ChatGPT Tactics</u></a></li>
<li><a href="https://win-solutions.techidaily.com/simple-troubleshooting-guide-resolve-pc-issues-with-deitch-looping-game/"><u>Simple Troubleshooting Guide: Resolve PC Issues with Deitch Looping Game</u></a></li>
<li><a href="https://extra-hints.techidaily.com/synchronized-system-apple-watch-and-mac-unlocking/"><u>Synchronized System  Apple Watch and Mac Unlocking</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/tech-tips-for-gamers-and-profitable-conversational-jobs/"><u>Tech Tips for Gamers & Profitable Conversational Jobs</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/terminate-chatgpt-connection-now/"><u>Terminate ChatGPT Connection Now</u></a></li>
<li><a href="https://program-issues.techidaily.com/the-ascent-software-fixed-and-ready-for-use-past-setbacks-addressed/"><u>The Ascent Software Fixed and Ready for Use – Past Setbacks Addressed</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-beginners-path-to-auto-gpt-installation-in-ubuntu/"><u>The Beginner's Path to Auto-GPT Installation in Ubuntu</u></a></li>
<li><a href="https://extra-information.techidaily.com/the-color-composers-toolkit-3-innovative-methods-for-photo-enhancement/"><u>The Color Composer's Toolkit  3 Innovative Methods for Photo Enhancement</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-future-of-pedagogy-top-8-advantages-of-embracing-artificial-intelligence/"><u>The Future of Pedagogy: Top 8 Advantages of Embracing Artificial Intelligence</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/top-5-virtual-therapists-the-bot-revolution/"><u>Top 5 Virtual Therapists: The Bot Revolution</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/understanding-ransomware-decode-on-the-go-tech-guide/"><u>Understanding Ransomware Decode - On-the-Go Tech Guide</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unleash-powerful-search-via-ai-at-bing-how-to-signup/"><u>Unleash Powerful Search via AI at Bing: How-To Signup</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unsubscribe-from-gpt-communication/"><u>Unsubscribe From GPT Communication</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/why-trusting-ai-for-windows-11-unlocks-is-risky-business/"><u>Why Trusting AI for Windows 11 Unlocks Is Risky Business</u></a></li>
</ul></div>
