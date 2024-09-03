---
title: "Accessing AI Dialogue: BashScripting and ShellGPT Integration"
date: 2024-09-02T20:34:17.111Z
updated: 2024-09-03T20:34:17.111Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Accessing AI Dialogue: BashScripting and ShellGPT Integration"
excerpt: "This Article Describes Accessing AI Dialogue: BashScripting and ShellGPT Integration"
thumbnail: https://thmb.techidaily.com/58e5d972b07e7d47a47d775672521bb7b4d26dbdad2027a1e368bc81a0dd6f11.jpg
---

## Accessing AI Dialogue: BashScripting and ShellGPT Integration

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
<a href="https://parisrhonecom.sjv.io/c/5597632/1896607/21553" target="_top" id="1896607"><img src="//a.impactradius-go.com/display-ad/21553-1896607" border="0" alt="" width="750" height="422"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1896607/21553" style="position:absolute;visibility:hidden;" border="0" />
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

<!-- affiliate ads begin -->
<a href="https://turbotech.pxf.io/c/5597632/1450763/17212" target="_top" id="1450763"><img src="//a.impactradius-go.com/display-ad/17212-1450763" border="0" alt="" width="2560" height="1440"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1450763/17212" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Step 3: Generate an OpenAPI Key

 Since the virtual environment is ready, you must connect the OpenAI services and your Ubuntu machine to run ShellGPT. For this purpose, you must navigate to [OpenAI's website](https://openai.com/) and create an account there.

 If you have an existing account, you can log in with your credentials and navigate to your profile image, located on the top right-hand side of the website.

 Click on **View API Keys**, followed by **Create new secret key**.

![OpenAI website interface showing a drop-down menu](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/view-api-keys-on-openai-website.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4699091&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/bccefcc1b1eee9eca3ae4f5c1a281482/products/1_jutoh-logo-1200x1600.jpg" border="0">Jutoh Plus -  Jutoh is an ebook creator for Epub, Kindle and more. It's fast, runs on Windows, Mac, and Linux, comes with a cover design editor, and allows book variations to be created with alternate text, style sheets and cover designs. Jutoh Plus adds scripting so you can automate ebook import and creation operations. It also allows customisation of ebook HTML via templates and source code documents; and you can create Windows CHM and wxWidgets HTB help files. </a>
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

<!-- affiliate ads begin -->
<a href="https://twopages.pxf.io/c/5597632/2016067/18544" target="_top" id="2016067"><img src="//a.impactradius-go.com/display-ad/18544-2016067" border="0" alt="" width="1020" height="380"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2016067/18544" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 Save and exit the editor. Then, use the source command to enable the changes.

`source ./bashrc`

 Finally, verify the API key with the **env** command.

`env`

![List of variables in a linux terminal](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/check-secret-key-in-env-list.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=37540879&QTY=1&AFFILIATE=108875&CART=1"><img src="https://paperscan.orpalis.com/img/content/You_prefer_to_use.png" border="0">PaperScan Professional： PaperScan Scanner Software is a powerful TWAIN & WIA scanning application centered on one idea: making document acquisition an unparalleled easy task for anyone.</a>
<!-- affiliate ads end -->
 Your **OPENAI\_API\_KEY** environment variable should be listed in the output.

## Step 5: Install ShellGPT on Ubuntu

 Once all the installation formalities are complete, you can simply move on to the best part, the ShellGPT installation. The installation steps are quite straightforward, and you can install the tool with the following command:

`pip3 install shell-gpt`

![Installation snippet on ubuntu's terminal screen](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/install-shell-gpt-on-ubuntu.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4620780&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/07dd4d5a72f5740ef0f035f201951476/728__90banner.jpg" border="0"></a>
<!-- affiliate ads end -->
 Let the installation finish; meanwhile, you can check out some interesting ways to use the AI tool via your terminal window.

<!-- affiliate ads begin -->
<a href="https://shop.copernic.com/order/checkout.php?PRODS=41033101&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.2checkout.com/images/merchant/8d30aa96e72440759f74bd2306c1fa3d/Copernic-2023-Affiliate-728x90-Elite.png" border="0"></a>
<!-- affiliate ads end -->
## Using ShellGPT for Running Queries via the Terminal

 The entire purpose of installing ShellGPT is to make your life easier. To use the terminal as a search engine and run some queries, you can use the **sgpt** command, followed by your query within quotes:

`sgpt "How many galaxies exist within the universe"`

![Ubuntu terminal interface with a query response](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/shellgpt-query-reponse.jpg)

<!-- affiliate ads begin -->
<a href="https://shop.mondly.com/affiliate.php?ACCOUNT=ATISTUDI&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.mondly.com%3FAFFILIATE%3D108875%26RESOURCE%3D%2BEducational%2B970x90%2B"><img src="https://secure.avangate.com/images/merchant/69c418c33ec2e1a4267fa9bb77fa1428/educational-970x90.gif" border="0"></a>
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
<li><a href="https://extra-skills.techidaily.com/new-revolutionary-techniques-for-exceptional-android-time-lapses-2024/"><u>[New] Revolutionary Techniques for Exceptional Android Time-Lapses 2024</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/updated-simplifying-speech-integration-into-instagram-content/"><u>[Updated] Simplifying Speech Integration Into Instagram Content</u></a></li>
<li><a href="https://screen-activity-recording.techidaily.com/updated-sleight-of-mind-best-room-adventures-reviewed/"><u>[Updated] Sleight of Mind  Best Room Adventures Reviewed</u></a></li>
<li><a href="https://fox-info.techidaily.com/updated-swiftly-restore-working-airdrop-between-apple-gadgets-and-macs/"><u>[Updated] Swiftly Restore Working AirDrop Between Apple Gadgets & Macs</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/adaptable-assistants-launch-your-own-8-ai-experieninas/"><u>Adaptable Assistants: Launch Your Own 8 AI Experieninas</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-driven-productivity-in-onlyoffice-workspaces/"><u>AI-Driven Productivity in ONLYOFFICE Workspaces</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/artificial-intelligence-and-job-uncertainty/"><u>Artificial Intelligence and Job Uncertainty</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/beyond-bing-and-chatgpt-when-is-gpt-5-due/"><u>Beyond Bing and ChatGPT: When Is GPT-5 Due?</u></a></li>
<li><a href="https://sound-issues.techidaily.com/boost-your-gameplay-essential-tips-to-fix-the-non-functional-fortnite-microphone/"><u>Boost Your Gameplay: Essential Tips to Fix the Non-Functional Fortnite Microphone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-unleashed-10-innovative-modifications-revealed/"><u>ChatGPT Unleashed: 10 Innovative Modifications Revealed</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-unveiled-six-techniques-for-novelists/"><u>ChatGPT Unveiled: Six Techniques for Novelists</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpts-evolution-an-omen-for-search-engines/"><u>ChatGPT's Evolution: An Omen for Search Engines?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/content-creators-vs-computational-composition-six-winning-strategies/"><u>Content Creators Vs. Computational Composition: Six Winning Strategies</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ensuring-employee-data-security-with-chatgpt/"><u>Ensuring Employee Data Security with ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/exploring-the-transparency-of-openais-shap-explainer/"><u>Exploring the Transparency of OpenAI's SHAP Explainer</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/from-swindles-to-stamps-the-twitsignature-transition/"><u>From Swindles to Stamps: The TwitSignature Transition</u></a></li>
<li><a href="https://screen-sharing-recording.techidaily.com/in-2024-cutting-edge-top-11-list-of-soundscape-capturers/"><u>In 2024, Cutting-Edge Top 11 List of Soundscape Capturers</u></a></li>
<li><a href="https://iphone-unlock.techidaily.com/in-2024-detailed-review-of-doctorsim-unlock-service-for-iphone-6s-drfone-by-drfone-ios/"><u>In 2024, Detailed Review of doctorSIM Unlock Service For iPhone 6s | Dr.fone</u></a></li>
<li><a href="https://android-unlock.techidaily.com/in-2024-unlocking-made-easy-the-best-10-apps-for-unlocking-your-vivo-y02t-device-by-drfone-android/"><u>In 2024, Unlocking Made Easy The Best 10 Apps for Unlocking Your Vivo Y02T Device</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/investigating-truthgpts-tokens-validity/"><u>Investigating TruthGPT's Tokens Validity</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/leading-cryptocurrency-topics-for-chatai/"><u>Leading Cryptocurrency Topics for ChatAI</u></a></li>
<li><a href="https://ai-video-tools.techidaily.com/new-2024-approved-with-the-help-of-fcp-you-can-easily-create-various-changes-to-audio-file-with-time-one-can-adjust-volume-fading-and-apply-audio-enhancemen/"><u>New 2024 Approved With the Help of FCP You Can Easily Create Various Changes to Audio File with Time, One Can Adjust Volume Fading and Apply Audio Enhancement as per Need</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/open-the-doors-to-gpt-4-no-currency-required/"><u>Open the Doors to GPT-4, No Currency Required</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/professional-audit-chatgpts-ai-precision-examined/"><u>Professional Audit: ChatGPT's AI Precision Examined</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/speak-and-listen-androids-guide-to-chatgpt-voicecontrol/"><u>Speak and Listen: Android’s Guide to ChatGPT VoiceControl</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/streamline-your-use-of-gpt-3-with-practical-plugins/"><u>Streamline Your Use of GPT-3 With Practical Plugins</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-enthusiasts-handbook-for-openai-api-mastery/"><u>The Enthusiast’s Handbook for OpenAI API Mastery</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-hacking-art-of-romantic-ruses/"><u>The Hacking Art of Romantic Ruses</u></a></li>
<li><a href="https://win11.techidaily.com/the-ultimate-list-of-3d-paint-keys/"><u>The Ultimate List of 3D Paint Keys</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-underground-guide-5-unauthorized-uses-of-ai/"><u>The Underground Guide: 5 Unauthorized Uses of AI</u></a></li>
<li><a href="https://android-location-track.techidaily.com/top-6-appsservices-to-trace-any-vivo-y78-5g-location-by-mobile-number-drfone-by-drfone-virtual-android/"><u>Top 6 Apps/Services to Trace Any Vivo Y78 5G Location By Mobile Number | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/transform-your-vehicle-through-chatgpts-creative-assistance/"><u>Transform Your Vehicle Through ChatGPT's Creative Assistance</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/transforming-chatgpts-output-to-match-personal-nuance/"><u>Transforming ChatGPT's Output to Match Personal Nuance</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/why-not-rely-on-ai-for-chat-7-key-objections/"><u>Why Not Rely on AI for Chat? #7 Key Objections</u></a></li>
<li><a href="https://ai-video-apps.techidaily.com/windows-8-video-editor-edit-mp4-files-with-ease-for-2024/"><u>Windows 8 Video Editor Edit MP4 Files with Ease for 2024</u></a></li>
</ul></div>
