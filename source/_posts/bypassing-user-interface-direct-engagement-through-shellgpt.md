---
title: "Bypassing User Interface: Direct Engagement Through ShellGPT"
date: 2024-08-03T00:54:06.616Z
updated: 2024-08-04T00:54:06.616Z
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
<li><a href="https://facebook-video-recording.techidaily.com/new-direct-tweet-transfers-to-facebook-feed/"><u>[New] Direct Tweet Transfers to Facebook Feed</u></a></li>
<li><a href="https://screen-activity-recording.techidaily.com/new-premier-platforms-identifying-the-finest-ps2-emulation-tools-for-android/"><u>[New] Premier Platforms  Identifying the Finest PS2 Emulation Tools for Android</u></a></li>
<li><a href="https://extra-hints.techidaily.com/updated-basic-guide-to-modify-clown-voiceprint-in-windoze-pc/"><u>[Updated] Basic Guide to Modify Clown Voiceprint in Windoze PC</u></a></li>
<li><a href="https://screen-recording.techidaily.com/updated-deciphering-bandicams-latest-2023-capabilities/"><u>[Updated] Deciphering Bandicam's Latest 2023 Capabilities</u></a></li>
<li><a href="https://facebook-video-files.techidaily.com/updated-in-2024-making-waves-in-the-social-media-world-via-fb/"><u>[Updated] In 2024, Making Waves in the Social Media World via FB</u></a></li>
<li><a href="https://extra-skills.techidaily.com/updated-quick-collage-assembly-tips-for-instant-sharing/"><u>[Updated] Quick Collage Assembly Tips for Instant Sharing</u></a></li>
<li><a href="https://some-tips.techidaily.com/updated-unlock-your-fcp-potential-with-these-10-plugs/"><u>[Updated] Unlock Your FCP Potential with These 10 Plugs</u></a></li>
<li><a href="https://extra-support.techidaily.com/2024-approved-leading-directory-30-premier-websites-for-accessible-vector-design-tools/"><u>2024 Approved  Leading Directory  30 Premier Websites for Accessible Vector Design Tools</u></a></li>
<li><a href="https://article-tips.techidaily.com/2024-approved-transformative-approaches-to-engaging-with-online-video-reviews/"><u>2024 Approved  Transformative Approaches to Engaging with Online Video Reviews</u></a></li>
<li><a href="https://howto.techidaily.com/7-fixes-for-unfortunately-phone-has-stopped-on-vivo-s18-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>7 Fixes for Unfortunately, Phone Has Stopped on Vivo S18 | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-enhanced-resume-craftsmayer-with-chatgpt-innovations/"><u>AI-Enhanced Résume Craftsmayer with ChatGPT Innovations</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ais-premium-convo-boost-chatgpt-plus-unveiled-at-20mo-us-only/"><u>AI's Premium Convo Boost: ChatGPT Plus Unveiled at $20/Mo (US-Only)</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/archiving-made-simple-saving-chatgpt-talks/"><u>Archiving Made Simple: Saving ChatGPT Talks</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/artificial-intelligence-6-rise-of-creative-tools/"><u>Artificial Intelligence: 6 Rise of Creative Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/augmenting-hr-workloads-gpts-role/"><u>Augmenting HR Workloads: GPT's Role</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/can-i-recover-permanently-deleted-photos-from-nord-3-5g-by-stellar-photo-recovery-android-mobile-photo-recover/"><u>Can I recover permanently deleted photos from Nord 3 5G</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/comparing-creativity-in-3-bot-systems/"><u>Comparing Creativity in 3 Bot Systems</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/crafting-secure-customized-workout-routines-by-chatgpt/"><u>Crafting Secure, Customized Workout Routines by ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/demystifying-claude-2-an-in-depth-guide-to-its-capabilities/"><u>Demystifying Claude 2: An In-Depth Guide to Its Capabilities</u></a></li>
<li><a href="https://android-unlock.techidaily.com/downloading-samfw-frp-tool-30-for-huawei-nova-y71-by-drfone-android/"><u>Downloading SamFw FRP Tool 3.0 for Huawei Nova Y71</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/elevate-your-content-with-these-25-powerful-instagram-tags/"><u>Elevate Your Content with These 25 Powerful Instagram Tags</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/expert-advice-on-lifting-your-chatgpt-ban/"><u>Expert Advice on Lifting Your ChatGPT Ban</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/gemini-elite-vs-powered-chatgpt/"><u>Gemini Elite Vs. Powered ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-generative-ai-fails-in-humanized-text-conversations/"><u>How Generative AI Fails in Humanized Text Conversations</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ignite-creativity-unique-ai-art-with-the-power-of-microsofts-copilot/"><u>Ignite Creativity: Unique AI Art with the Power of Microsoft's Copilot</u></a></li>
<li><a href="https://ios-unlock.techidaily.com/in-2024-how-to-fix-apple-iphone-6s-plus-unavailable-issue-with-ease-by-drfone-ios/"><u>In 2024, How To Fix Apple iPhone 6s Plus Unavailable Issue With Ease</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/leveraging-gpt-to-streamline-home-device-operations/"><u>Leveraging GPT to Streamline Home Device Operations</u></a></li>
<li><a href="https://youtube-lab.techidaily.com/oming-the-invisible-screen-hurdle-youtube-fixes/"><u>Overcoming the Invisible Screen Hurdle  YouTube Fixes</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/prime-networks-for-collaborative-prompt-creation/"><u>Prime Networks for Collaborative Prompt Creation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/reality-assurance-no-gpt-windows-isnt-harmful-app/"><u>Reality Assurance: No, GPT-Windows Isn't Harmful App</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/safekeeping-for-chatgpt-dialogues/"><u>Safekeeping for ChatGPT Dialogues</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/securing-conversations-with-ai-tech/"><u>Securing Conversations with AI Tech</u></a></li>
<li><a href="https://easy-unlock-android.techidaily.com/top-4-sim-location-trackers-to-easily-find-your-lost-realme-11-5g-device-by-drfone-android/"><u>Top 4 SIM Location Trackers To Easily Find Your Lost Realme 11 5G Device</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/transform-written-work-with-gpt-4/"><u>Transform Written Work with GPT-4</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/transforming-traditional-gaming-with-innovative-ai-techniques/"><u>Transforming Traditional Gaming with Innovative AI Techniques</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unpacking-the-potential-perils-of-using-chatgpt-in-our-lives/"><u>Unpacking the Potential Perils of Using ChatGPT in Our Lives</u></a></li>
</ul></div>
