---
title: "Launching ChatGPT: Bash Scripts and ShellGPT Tactics"
date: 2024-08-15T02:35:52.726Z
updated: 2024-08-16T02:35:52.726Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Launching ChatGPT: Bash Scripts and ShellGPT Tactics"
excerpt: "This Article Describes Launching ChatGPT: Bash Scripts and ShellGPT Tactics"
thumbnail: https://thmb.techidaily.com/cd61def31c266f510e96724b2a8477792657278ca4fb179ccb3f421fcf0aa55a.jpg
---

## Launching ChatGPT: Bash Scripts and ShellGPT Tactics

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
<!-- affiliate ads begin -->
<a href="https://secure.textstudio.com/order/checkout.php?PRODS=35633281&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/d6eb8222c9718486bdabce8b897380f7/products/2_premium-icon.png" border="0"> Take advantage of PREMIUM features. 
Create your texts / logos without any limitation. 
No attribution required when downloading. 
No advertising on the website. 
 TextStudio.com  PREMIUM - Monthly Membership</a>
<!-- affiliate ads end -->

 After installation, you can again use the **\--version** command to check if the installation was successful.

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
<a href="https://shop.mondly.com/affiliate.php?ACCOUNT=ATISTUDI&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.mondly.com%3FAFFILIATE%3D108875%26RESOURCE%3D%2BEducational%2B970x90%2B"><img src="https://secure.avangate.com/images/merchant/69c418c33ec2e1a4267fa9bb77fa1428/educational-970x90.gif" border="0"></a>
<!-- affiliate ads end -->

## Step 3: Generate an OpenAPI Key

 Since the virtual environment is ready, you must connect the OpenAI services and your Ubuntu machine to run ShellGPT. For this purpose, you must navigate to [OpenAI's website](https://openai.com/) and create an account there.

 If you have an existing account, you can log in with your credentials and navigate to your profile image, located on the top right-hand side of the website.

 Click on **View API Keys**, followed by **Create new secret key**.

![OpenAI website interface showing a drop-down menu](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/view-api-keys-on-openai-website.jpg)

 Do not share this key with anyone since the connection is private and should be used on your machine only.

 Copy the API key from the dialog box, and save it somewhere, since you won't be able to review the same key again.

![OpenAI's secret key website page with an open dialog box](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/generate-api-secret-key.jpg)
<!-- affiliate ads begin -->
<a href="https://getlyla.pxf.io/c/5597632/1455723/15391" target="_top" id="1455723"><img src="//a.impactradius-go.com/display-ad/15391-1455723" border="0" alt="" width="336" height="280"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1455723/15391" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 To establish a connection on your Ubuntu machine, create an environment variable with the **export** command:

`export OPENAI_API_KEY=<paste key details here>`

### Add and Verify the API Key Into a Virtual Environment Variable

 When you execute the API key in this manner, Linux will use it only for a single instance. However, if you want to make the execution permanent, save it in the **.bashrc** file.

 All you have to do is type in the first command and enter the subsequent command within the text editor:

`nano ./bashrc  
export OPENAI_API_KEY=<paste key details here>`

![Ubuntu terminal window with code snippets to create and save an environment variable](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/create-an-environment-variable-1.jpg)
<!-- affiliate ads begin -->
<a href="https://aofit.pxf.io/c/5597632/1399701/16396" target="_top" id="1399701"><img src="//a.impactradius-go.com/display-ad/16396-1399701" border="0" alt="" width="960" height="300"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1399701/16396" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Save and exit the editor. Then, use the source command to enable the changes.

`source ./bashrc`

 Finally, verify the API key with the **env** command.

`env`

![List of variables in a linux terminal](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/check-secret-key-in-env-list.jpg)
<!-- affiliate ads begin -->
<a href="https://cowinaudio.pxf.io/c/5597632/1116855/13794" target="_top" id="1116855"><img src="//a.impactradius-go.com/display-ad/13794-1116855" border="0" alt="" width="767" height="285"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1116855/13794" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Your **OPENAI\_API\_KEY** environment variable should be listed in the output.

## Step 5: Install ShellGPT on Ubuntu

 Once all the installation formalities are complete, you can simply move on to the best part, the ShellGPT installation. The installation steps are quite straightforward, and you can install the tool with the following command:

`pip3 install shell-gpt`

![Installation snippet on ubuntu's terminal screen](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/install-shell-gpt-on-ubuntu.jpg)

 Let the installation finish; meanwhile, you can check out some interesting ways to use the AI tool via your terminal window.

## Using ShellGPT for Running Queries via the Terminal

 The entire purpose of installing ShellGPT is to make your life easier. To use the terminal as a search engine and run some queries, you can use the **sgpt** command, followed by your query within quotes:

`sgpt "How many galaxies exist within the universe"`

![Ubuntu terminal interface with a query response](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/shellgpt-query-reponse.jpg)
<!-- affiliate ads begin -->
<a href="https://thefitville.pxf.io/c/5597632/1526796/15852" target="_top" id="1526796"><img src="//a.impactradius-go.com/display-ad/15852-1526796" border="0" alt="" width="1200" height="628"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1526796/15852" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4620780&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/07dd4d5a72f5740ef0f035f201951476/728__90banner.jpg" border="0"></a>
<!-- affiliate ads end -->
## Using ShellGPT for Generating Code

 You can use your ShellGPT for generating code as well. You can do it by passing the right command with the **sgpt** command:

`sgpt --code "print the Fibonacci series"`

![Ubuntu terminal window with code snippets](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/shellgpt-code-reponse.jpg)
<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4715391&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/7f687767ccf20fcea1c9dc4a5adc2326/Digisigner_banner_728_x_90_color_version.png" border="0"></a>
<!-- affiliate ads end -->

 The output consists of code you can execute within Python to generate the Fibonacci series.

<!-- affiliate ads begin -->
<a href="https://store.iobit.com/order/checkout.php?PRODS=1468905&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/184260348236f9554fe9375772ff966e/ascscan_728x90.png" border="0"></a>
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
<li><a href="https://visual-screen-recording.techidaily.com/new-in-2024-native-chrome-os-screen-replay-app/"><u>[New] In 2024, Native Chrome OS Screen Replay App</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/updated-2024-approved-unveiling-ipads-full-potential-a-timelapse-journey-begins-here/"><u>[Updated] 2024 Approved  Unveiling iPad's Full Potential  A Timelapse Journey Begins Here</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-innovations-showdown-dissecting-forefront-and-chatgpts-features/"><u>AI Innovations Showdown: Dissecting Forefront and ChatGPT's Features</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/artists-claim-vindication-against-openaimeta-in-court/"><u>Artists Claim Vindication: Against OpenAI/Meta in Court</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/bank-data-at-risk-the-role-of-gpt-in-todays-cyber-threats/"><u>Bank Data at Risk? The Role of GPT in Today's Cyber Threats</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/beyond-the-turing-emerging-evaluation-methods/"><u>Beyond The Turing: Emerging Evaluation Methods</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/bing-the-brainiac-search-engine/"><u>Bing, The Brainiac Search Engine</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-powered-guide-to-youtube-video-script-creation/"><u>ChatGPT-Powered Guide to YouTube Video Script Creation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/code-mastery-for-effective-gpt-3-integration/"><u>Code Mastery for Effective GPT-3 Integration</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/deciphering-the-turing-tests-implications-and-future-victors/"><u>Deciphering The Turing Test's Implications & Future Victors</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/designing-balanced-dietary-patterns-with-gpt-aid/"><u>Designing Balanced Dietary Patterns with GPT Aid</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/dodging-ai-crafted-windows-11-keys-a-good-practice/"><u>Dodging AI-Crafted Windows 11 Keys: A Good Practice</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/enhancing-analytical-prowess-in-excel-through-chatgpt-integration/"><u>Enhancing Analytical Prowess in Excel Through ChatGPT Integration</u></a></li>
<li><a href="https://vp-tips.techidaily.com/from-novice-to-vlogger-top-tips-to-enhance-your-tiktok-videos-for-2024/"><u>From Novice to Vlogger  Top Tips to Enhance Your TikTok Videos for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/global-relevance-of-latest-chatgpt-info/"><u>Global Relevance of Latest ChatGPT Info</u></a></li>
<li><a href="https://android-transfer.techidaily.com/how-to-transfer-data-from-oppo-reno-8t-to-blackberry-drfone-by-drfone-transfer-from-android-transfer-from-android/"><u>How to Transfer Data from Oppo Reno 8T to BlackBerry | Dr.fone</u></a></li>
<li><a href="https://ai-editing-video.techidaily.com/in-2024-kdenlive-is-a-free-open-source-video-editing-software-application-kdenlive-is-a-powerful-video-editor-that-can-be-used-to-create-professional-qualit/"><u>In 2024, Kdenlive Is a Free, Open-Source Video Editing Software Application. Kdenlive Is a Powerful Video Editor that Can Be Used to Create Professional-Quality Videos</u></a></li>
<li><a href="https://tiktok-video-recordings.techidaily.com/in-2024-step-by-step-guide-to-creating-viral-tiktok-videos-at-home/"><u>In 2024, Step-by-Step Guide to Creating Viral TikTok Videos at Home</u></a></li>
<li><a href="https://some-approaches.techidaily.com/in-2024-strategy-unveiled-masterful-box-opening-tactics/"><u>In 2024, Strategy Unveiled  Masterful Box-Opening Tactics</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/innovative-programming-enhancements-without-chatgpt/"><u>Innovative Programming Enhancements Without ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-chatgpt-a-guide-to-academic-writing/"><u>Mastering ChatGPT: A Guide to Academic Writing</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-chatgpt-an-openai-guide/"><u>Mastering ChatGPT: An OpenAI Guide</u></a></li>
<li><a href="https://ai-driven-video-production.techidaily.com/new-2024-approved-expert-approved-ipad-video-editors-top-5-for/"><u>New 2024 Approved Expert-Approved iPad Video Editors Top 5 For</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/pilot-progressions-understanding-copilot-enhancements/"><u>Pilot Progressions: Understanding CoPilot Enhancements</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/proton-vpn-browser-extension-how-to-change-your-email-address-and-the-chatgpt-windows-app-is-fake/"><u>Proton VPN Browser Extension, How to Change Your Email Address, and the ChatGPT Windows App Is Fake</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/quick-fixes-for-stuck-chatgpt-apps-on-iphones/"><u>Quick Fixes for Stuck ChatGPT Apps on iPhones</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/script-revolution-unlocking-creativity-with-chatgpt-in-gaming/"><u>Script Revolution: Unlocking Creativity with ChatGPT in Gaming</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/skepticism-grows-over-zerogpt-and-detection-tools/"><u>Skepticism Grows Over ZeroGPT & Detection Tools</u></a></li>
<li><a href="https://youtube-webster.techidaily.com/-modification-youtube-aspect-ratio-on-mac/"><u>Swift Modification  YouTube Aspect Ratio on MAC</u></a></li>
<li><a href="https://extra-information.techidaily.com/the-entrepreneurial-roadmap-for-starting-an-online-product-critique-site/"><u>The Entrepreneurial Roadmap for Starting an Online Product Critique Site</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-future-unfolds-top-features-of-newest-gpt-release/"><u>The Future Unfolds: Top Features of Newest GPT Release</u></a></li>
<li><a href="https://android-unlock.techidaily.com/top-10-password-cracking-tools-for-samsung-galaxy-s23plus-by-drfone-android/"><u>Top 10 Password Cracking Tools For Samsung Galaxy S23+</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-the-potential-of-gpt-with-android/"><u>Unveiling the Potential of GPT with Android</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/your-guide-to-understanding-and-using-claude-3/"><u>Your Guide to Understanding and Using Claude 3</u></a></li>
</ul></div>
