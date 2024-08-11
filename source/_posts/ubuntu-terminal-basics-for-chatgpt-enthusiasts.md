---
title: Ubuntu Terminal Basics for ChatGPT Enthusiasts
date: 2024-08-10T02:06:14.948Z
updated: 2024-08-11T02:06:14.948Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Ubuntu Terminal Basics for ChatGPT Enthusiasts
excerpt: This Article Describes Ubuntu Terminal Basics for ChatGPT Enthusiasts
thumbnail: https://thmb.techidaily.com/94367d0839b4e8bd552f4ff0b46203c6692aa9dd549da1507965a6ba4039d0e6.png
---

## Ubuntu Terminal Basics for ChatGPT Enthusiasts

 Artificial intelligence has emerged as a new-age sensation, leaving everything behind in the dust. With new additions daily, there is a lot to look forward to.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 People use this multi-faceted, ubiquitous tool to crack jokes, write codes and even answer the most random questions. It’s easy to use ChatGPT on other OSes, so, as a Linux user, why should you stay behind?

 You too can enjoy ChatGPT’s Linux avatar, ShellGPT. Here's how to install and use the AI tool from your Ubuntu terminal in a few easy steps.

<!-- affiliate ads begin -->
<a href="https://zonlipartnershipprogram.pxf.io/c/5597632/1596691/17882" target="_top" id="1596691"><img src="//a.impactradius-go.com/display-ad/17882-1596691" border="0" alt="" width="728" height="90"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1596691/17882" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## What’s ShellGPT, ChatGPT’s Equivalent Linux Namesake?

 ShellGPT, as it is more commonly known, is ChatGPT’s command-line equivalent, through which users can use and engage with the AI chatbot via their Linux terminal. The chatbot draws power from OpenAI’s Large Language Model, providing intelligent user recommendations.

 Large Language Models (LLMs) are becoming a hot topic of discussion since you can easily [run LLM-enabled chatbots on your Raspberry Pi](https://www.makeuseof.com/raspberry-pi-large-language-model/).

 Sounds intriguing, doesn’t it?

 If you have experience interacting with ChatGPT, you will love this alternate Linux shell version.

 What’s the benefit of installing ShellGPT on your machine? It’s simple; you don’t need to type in unnecessary long commands or head to your browser. Instead, you can perform all possible tasks from the comfort of your Linux terminal.

 Before installing ShellGPT on your Ubuntu machine, here are a few prerequisites to take care of.

<!-- affiliate ads begin -->
<a href="https://united.elfm.net/c/5597632/517826/4704" target="_top" id="517826"><img src="//a.impactradius-go.com/display-ad/4704-517826" border="0" alt="" width="728" height="90"/></a><img height="0" width="0" src="https://united.elfm.net/i/5597632/517826/4704" style="position:absolute;visibility:hidden;" border="0" />
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

<!-- affiliate ads begin -->
<a href="https://shop.copernic.com/order/checkout.php?PRODS=41033101&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.2checkout.com/images/merchant/8d30aa96e72440759f74bd2306c1fa3d/Copernic-2023-Affiliate-728x90-Elite.png" border="0"></a>
<!-- affiliate ads end -->
![Ubuntu terminal window with code snippets with installation codes](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/install-pip-on-ubuntu.jpg)

 After installation, you can again use the **\--version** command to check if the installation was successful.

<!-- affiliate ads begin -->
<a href="https://cowinaudio.pxf.io/c/5597632/1116855/13794" target="_top" id="1116855"><img src="//a.impactradius-go.com/display-ad/13794-1116855" border="0" alt="" width="767" height="285"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1116855/13794" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Step 2: Install and Set Up a Virtual Environment Using Python

 Now that Python and PIP are ready, you can set up Python's virtual environment to make the machine environment conducive for installing and running ShellGPT. Virtual environments are ideal for running isolated programs since they can avoid library conflicts.

 With a virtual environment in tow, you can limit the interactions between your system's and virtual environment's programs while performing different executions in silos.

 Using a virtual environment is an optional step, to avoid any unforeseen mishaps while installing and using Python libraries.

 To create a virtual environment using Python, you need to install the **venv** module:

`sudo apt install python3-venv -y`

![Ubuntu terminal window code snippets](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/install-virtual-environment-module-in-ubuntu.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=40085955&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/f702defbc67edb455949f46babab0c18/products/2_logo9.png" border="0">FX PRO (Gold Robot + Silver Robot(Basic Package))</a>
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

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4737285&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/b2f83c409ce63012229fb9cd465bdcfe/products/copy_reporting_system.png" border="0">  KoolReport Pro  is an advanced solution for creating data reports and dashboards in PHP. Equipped with all  extended packages , KoolReport Pro is able to connect to various datasources, perform advanced data analysis, construct stunning charts and graphs and export your beautiful work to PDF, Excel, JPG or other formats. Plus, it includes powerful built-in reports such as pivot report and drill-down report which will save your time in building ones. 

 It will help you to write dynamic data reports easily, to construct intuitive dashboards or to build a whole business intelligence cockpit. 

  KoolReport Pro  package goes with Full Source Code, Royal Free, ONE (1) Year Priority Support, ONE (1) Year Free Upgrade and 30-Days Money Back Guarantee. 

  Developer License  allows  Single Developer  to create Unlimited Reports, deploy on Unlimited Servers and able deliver the work to Unlimited Clients. </a>
<!-- affiliate ads end -->
![OpenAI's secret key website page with an open dialog box](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/generate-api-secret-key.jpg)

 To establish a connection on your Ubuntu machine, create an environment variable with the **export** command:

`export OPENAI_API_KEY=<paste key details here>`

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2082541/7443" target="_top" id="2082541"><img src="//a.impactradius-go.com/display-ad/7443-2082541" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2082541/7443" style="position:absolute;visibility:hidden;" border="0" />
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

<!-- affiliate ads begin -->
<a href="https://order.glarysoft.com/order/checkout.php?PRODS=35504869&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/6734fa703f6633ab896eecbdfad8953a/products/1_FR-200-1.png" border="0">Glarysoft File Recovery Pro Annually -  Helps to recover your lost file/data, even permanently deleted data. 
</a>
<!-- affiliate ads end -->
![List of variables in a linux terminal](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/check-secret-key-in-env-list.jpg)

 Your **OPENAI\_API\_KEY** environment variable should be listed in the output.

## Step 5: Install ShellGPT on Ubuntu

 Once all the installation formalities are complete, you can simply move on to the best part, the ShellGPT installation. The installation steps are quite straightforward, and you can install the tool with the following command:

`pip3 install shell-gpt`

![Installation snippet on ubuntu's terminal screen](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/install-shell-gpt-on-ubuntu.jpg)

 Let the installation finish; meanwhile, you can check out some interesting ways to use the AI tool via your terminal window.

<!-- affiliate ads begin -->
<a href="https://otszone.ots7.com/order/checkout.php?PRODS=4713321&QTY=1&AFFILIATE=108875&CART=1"><img src="https://green.ots7.com/screenshots/OtsAV/OtsAVDJ1.90-300x188.jpg" border="0">OtsAV DJ Pro</a>
<!-- affiliate ads end -->
## Using ShellGPT for Running Queries via the Terminal

 The entire purpose of installing ShellGPT is to make your life easier. To use the terminal as a search engine and run some queries, you can use the **sgpt** command, followed by your query within quotes:

`sgpt "How many galaxies exist within the universe"`

![Ubuntu terminal interface with a query response](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/shellgpt-query-reponse.jpg)

## Using ShellGPT for Generating Code

 You can use your ShellGPT for generating code as well. You can do it by passing the right command with the **sgpt** command:

`sgpt --code "print the Fibonacci series"`

<!-- affiliate ads begin -->
<a href="https://store.revouninstaller.com/order/checkout.php?PRODS=27889512&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/4282ec8de8c9be897e7aff4aa231b1a4/728__90.jpg" border="0"></a>
<!-- affiliate ads end -->
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
<li><a href="https://screen-video-capture.techidaily.com/new-capture-king-review-the-screen-recorder-showdown/"><u>[New] Capture King Review  The Screen Recorder Showdown</u></a></li>
<li><a href="https://extra-support.techidaily.com/new-mastering-motion-blur-in-ps-a-step-by-step-guide/"><u>[New] Mastering Motion Blur in PS  A Step-by-Step Guide</u></a></li>
<li><a href="https://fox-boxes.techidaily.com/new-smarter-spending-on-cloud-data-services-insights-and-recommendations-for-2024/"><u>[New] Smarter Spending on Cloud Data Services  Insights & Recommendations for 2024</u></a></li>
<li><a href="https://screen-capture.techidaily.com/updated-2024-approved-elite-pace-setter-pc-titles/"><u>[Updated] 2024 Approved  Elite Pace-Setter PC Titles</u></a></li>
<li><a href="https://instagram-video-files.techidaily.com/updated-2024-approved-gif-galore-how-to-seamlessly-share-emojis-and-animations-on-instagram/"><u>[Updated] 2024 Approved  GIF Galore  How to Seamlessly Share Emojis & Animations on Instagram</u></a></li>
<li><a href="https://instagram-clips.techidaily.com/updated-2024-approved-unveiling-sources-instagram-pictures-inverse-search-guide/"><u>[Updated] 2024 Approved  Unveiling Sources  Instagram Pictures' Inverse Search Guide</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/updated-exploring-the-top-hashtags-for-a-boost-on-ig-for-2024/"><u>[Updated] Exploring the Top Hashtags for a Boost on IG for 2024</u></a></li>
<li><a href="https://facebook-video-content.techidaily.com/updated-hidden-gems-10-unique-facebook-meme-pages/"><u>[Updated] Hidden Gems  10 Unique Facebook Meme Pages</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1-million-mark-geminis-game-changing-leap-forward/"><u>$1 Million Mark: Gemini’s Game-Changing Leap Forward</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/10-custom-gpts-that-actually-make-chatgpt-better/"><u>10 Custom GPTs That Actually Make ChatGPT Better</u></a></li>
<li><a href="https://win-dash.techidaily.com/1970-two-mules-for-sister-sara-with-eastwood-as-hogan-a-mercenary-who-is-hired-to-protect-a-mexican-nun-from-bandits-and-revolutionaries-in-mexico-during-th133/"><u>1970 - Two Mules for Sister Sara, with Eastwood as Hogan, a Mercenary Who Is Hired to Protect a Mexican Nun From Bandits and Revolutionaries in Mexico During the French Intervention. The Film Was Based on B. Traven's Novel ''A Wave Across Hell''.</u></a></li>
<li><a href="https://fox-hovers.techidaily.com/2024-approved-calmly-quieten-your-computers-audio-output/"><u>2024 Approved  Calmly Quieten Your Computer's Audio Output</u></a></li>
<li><a href="https://some-guidance.techidaily.com/2024-approved-unleash-the-magic-of-videos-on-windows-mobile/"><u>2024 Approved  Unleash the Magic of Videos on Windows Mobile</u></a></li>
<li><a href="https://location-fake.techidaily.com/3-ways-to-fake-gps-without-root-on-honor-v-purse-drfone-by-drfone-virtual-android/"><u>3 Ways to Fake GPS Without Root On Honor V Purse | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/4-ai-story-generators-worth-trying/"><u>4 AI Story Generators Worth Trying</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/4-pioneering-ways-ai-elevates-study-habits/"><u>4 Pioneering Ways AI Elevates Study Habits</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/4-typical-slip-ups-when-deploying-chatgpt-for-articles/"><u>4 Typical Slip-Ups When Deploying ChatGPT for Articles</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/4-ways-ai-tools-enhance-your-academic-research/"><u>4 Ways AI Tools Enhance Your Academic Research</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/5-easy-chatgpt-strategies-for-finding-employment/"><u>5 Easy ChatGPT Strategies for Finding Employment</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/5-essential-warnings-before-choosing-ai-as-your-mental-health-companion/"><u>5 Essential Warnings Before Choosing AI as Your Mental Health Companion</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/5-pivotal-ways-ai-enhances-digital-deceit-operations/"><u>5 Pivotal Ways AI Enhances Digital Deceit Operations</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/5-revolutionary-tools-to-create-with-ai/"><u>5 Revolutionary Tools to Create with AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/5-ways-students-can-use-chatgpt-in-school/"><u>5 Ways Students Can Use ChatGPT in School</u></a></li>
<li><a href="https://win11-tips.techidaily.com/5-ways-to-access-the-startup-folder-in-windows/"><u>5 Ways to Access the Startup Folder in Windows</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/6-reasons-for-skepticism-toward-automated-decision-making/"><u>6 Reasons for Skepticism Toward Automated Decision-Making</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/7-indispensable-qualities-in-selecting-robot-based-support/"><u>7 Indispensable Qualities in Selecting Robot-Based Support</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/7-reasons-to-approach-generative-ai-with-caution-in-chat-apps/"><u>7 Reasons to Approach Generative AI with Caution in Chat Apps</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/7-reasons-to-consider-using-chatgpt-for-health-advice/"><u>7 Reasons to Consider Using ChatGPT for Health Advice</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/7-strategies-for-leveraging-chatgpts-visual-ai/"><u>7 Strategies for Leveraging ChatGPT's Visual AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/8-reasons-why-teachers-should-embrace-ai-instead-of-fearing-it/"><u>8 Reasons Why Teachers Should Embrace AI Instead of Fearing It</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-balanced-look-at-chatgpt-upgrade-plans/"><u>A Balanced Look at ChatGPT Upgrade Plans</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-beginners-guide-to-integrating-latest-chatgpt-add-ons/"><u>A Beginner's Guide to Integrating Latest ChatGPT Add-Ons</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-comparative-study-the-advantages-and-disadvantages-of-local-llms/"><u>A Comparative Study: The Advantages & Disadvantages of Local LLMs</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-complete-walkthrough-for-gpt-3s-beta-features/"><u>A Complete Walkthrough for GPT-3's Beta Features</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-guide-to-chatgpt-powered-poetic-compositions/"><u>A Guide to ChatGPT-Powered Poetic Compositions</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-linguistic-enigma-solved-interpreting-chatgpts-programming-puzzle/"><u>A Linguistic Enigma Solved: Interpreting ChatGPT's Programming Puzzle</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-new-era-for-ai-linguistics-with-googles-palm-2-model/"><u>A New Era for AI Linguistics with Google's PaLM 2 Model</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721364760663-alert-fake-gpt-programs-pose-threats-to-online-safety/"><u>Alert: Fake GPT Programs Pose Threats to Online Safety</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721402550569-earn-extra-cash-by-hunting-software-glitches-with-openai/"><u>Earn Extra Cash by Hunting Software Glitches with OpenAI!</u></a></li>
<li><a href="https://driver-download.techidaily.com/effortless-upgrade-how-to-update-drivers-for-microsofts-sculpt-ergonomic-keyboard/"><u>Effortless Upgrade: How to Update Drivers for Microsoft's Sculpt Ergonomic Keyboard</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721421451434-enhanced-accuracy-in-every-click-bings-ai-driven-search-on-devices/"><u>Enhanced Accuracy in Every Click: Bing’s AI-Driven Search on Devices.</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721371588262-everyone-enjoys-gpt-4-for-free-yet-6-advantages-of-premium/"><u>Everyone Enjoys GPT-4 for Free; Yet, 6 Advantages of Premium</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721413720208-exiting-the-gpt-world-now/"><u>Exiting the GPT World – Now</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721423072362-free-gpt-4-available-to-everyone-dont-overlook-the-6-platinum-perks/"><u>Free GPT-4 Available to Everyone! Don't Overlook the 6 Platinum Perks</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721432354798-gpt-4s-new-era-of-accessibility-for-all-at-no-cost-yet-platinum-still-offers-6-peculiar-benefits/"><u>GPT-4's New Era of Accessibility: For All at No Cost! Yet Platinum Still Offers 6 Peculiar Benefits</u></a></li>
<li><a href="https://vp-tips.techidaily.com/in-2024-instagram-guide-to-uploading-podcast-episodes/"><u>In 2024, Instagram Guide to Uploading Podcast Episodes</u></a></li>
<li><a href="https://extra-approaches.techidaily.com/instant-annotation-text-overlaying-on-images-and-videos-using-windows-photos-for-2024/"><u>Instant Annotation  Text Overlaying on Images & Videos Using Windows Photos for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721436566102-intelligent-browsing-made-simple-unleash-bing-ai-on-your-devices/"><u>Intelligent Browsing Made Simple: Unleash Bing AI on Your Devices</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721389502663-introducing-ai-search-access-bing-on-your-devices/"><u>Introducing AI Search: Access Bing on Your Devices!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721417752360-mastering-conversations-just-add-chatgpt-and-android/"><u>Mastering Conversations - Just Add ChatGPT & Android!</u></a></li>
<li><a href="https://facebook.techidaily.com/meta-verified-vs-twitter-blue-which-offers-more/"><u>Meta Verified Vs. Twitter Blue: Which Offers More?</u></a></li>
<li><a href="https://voice-adjusting.techidaily.com/new-in-2024-a-comprehensive-review-the-premier-audio-changers-for-smartphones/"><u>New In 2024, A Comprehensive Review The Premier Audio Changers for Smartphones</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721384309754-no-emoji-tweets-ahead-linuss-unveiled-secrets-trojan-analysis-and-chatgpt-shortfalls/"><u>No Emoji Tweets Ahead, Linus's Unveiled Secrets, Trojan Analysis, & ChatGPT Shortfalls.</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721416643292-no-emoji-tweets-linuss-disclosures-trojans-explained-and-chatgpt-faults-displayed/"><u>No Emoji Tweets, Linus's Disclosures, Trojans Explained, & ChatGPT Faults Displayed</u></a></li>
<li><a href="https://unlock-android.techidaily.com/still-using-pattern-locks-with-infinix-hot-30i-tips-tricks-and-helpful-advice-by-drfone-android/"><u>Still Using Pattern Locks with Infinix Hot 30i? Tips, Tricks and Helpful Advice</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721410547181-to-use-or-not-to-use-local-llm-heres-why/"><u>To Use or Not to Use Local LLM? Here's Why!</u></a></li>
<li><a href="https://sound-issues.techidaily.com/ultimate-guide-silencing-your-logitech-g-pro-x-microphone/"><u>Ultimate Guide: Silencing Your Logitech G Pro X Microphone</u></a></li>
</ul></div>
