---
title: Utilizing ShellGPT for Efficient ChatGPT Experiences
date: 2024-08-29T19:44:59.489Z
updated: 2024-08-30T19:44:59.489Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Utilizing ShellGPT for Efficient ChatGPT Experiences
excerpt: This Article Describes Utilizing ShellGPT for Efficient ChatGPT Experiences
thumbnail: https://thmb.techidaily.com/55f69c473ce05e56332fdc0fd3becc5010779e559c1a26eb52ce7f94ac706c0b.jpg
---

## Utilizing ShellGPT for Efficient ChatGPT Experiences

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
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=33729450&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/7f687767ccf20fcea1c9dc4a5adc2326/Digisigner_banner_728_x_90_color_version.png" border="0"></a>
<!-- affiliate ads end -->
<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4620778&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/07dd4d5a72f5740ef0f035f201951476/300__250banner.jpg" border="0"></a>
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
<a href="https://caperobbin.sjv.io/c/5597632/2006118/18460" target="_top" id="2006118"><img src="//a.impactradius-go.com/display-ad/18460-2006118" border="0" alt="" width="300" height="250"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2006118/18460" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Step 3: Generate an OpenAPI Key

 Since the virtual environment is ready, you must connect the OpenAI services and your Ubuntu machine to run ShellGPT. For this purpose, you must navigate to [OpenAI's website](https://openai.com/) and create an account there.

 If you have an existing account, you can log in with your credentials and navigate to your profile image, located on the top right-hand side of the website.

 Click on **View API Keys**, followed by **Create new secret key**.

![OpenAI website interface showing a drop-down menu](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/view-api-keys-on-openai-website.jpg)

<!-- affiliate ads begin -->
<a href="https://printrendy.pxf.io/c/5597632/1453721/17020" target="_top" id="1453721"><img src="//a.impactradius-go.com/display-ad/17020-1453721" border="0" alt="" width="300" height="250"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1453721/17020" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 Do not share this key with anyone since the connection is private and should be used on your machine only.

 Copy the API key from the dialog box, and save it somewhere, since you won't be able to review the same key again.

![OpenAI's secret key website page with an open dialog box](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/generate-api-secret-key.jpg)

<!-- affiliate ads begin -->
<a href="https://ephamedtechinc.pxf.io/c/5597632/2095369/26400" target="_top" id="2095369"><img src="//a.impactradius-go.com/display-ad/26400-2095369" border="0" alt="" width="1024" height="512"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2095369/26400" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
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
<a href="https://store.iobit.com/order/checkout.php?PRODS=4596923&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/184260348236f9554fe9375772ff966e/ascscan_468X60.png" border="0"></a>
<!-- affiliate ads end -->
<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=3851655&QTY=1&AFFILIATE=108875&CART=1"><img src="http://www.aiseesoft.com/avangate/30p/banner.jpg" border="0"></a>
<!-- affiliate ads end -->
## Using ShellGPT for Generating Code

 You can use your ShellGPT for generating code as well. You can do it by passing the right command with the **sgpt** command:

`sgpt --code "print the Fibonacci series"`

![Ubuntu terminal window with code snippets](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/shellgpt-code-reponse.jpg)

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2075482/7443" target="_top" id="2075482"><img src="//a.impactradius-go.com/display-ad/7443-2075482" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2075482/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
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
<li><a href="https://network-issues.techidaily.com/resolved-bridging-the-online-gap-in-cod-cold-war-2024/"><u>[RESOLVED] Bridging the Online Gap in CoD Cold War 2024</u></a></li>
<li><a href="https://remote-screen-capture.techidaily.com/updated-best-price-to-performance-tablets-with-gaming-capabilities/"><u>[Updated] Best Price-to-Performance Tablets with Gaming Capabilities</u></a></li>
<li><a href="https://extra-resources.techidaily.com/updated-camera-enthusiasts-top-list-ultimate-6-4k-dslr-cameras/"><u>[Updated] Camera Enthusiasts' Top List  Ultimate 6 4K DSLR Cameras</u></a></li>
<li><a href="https://twitter-videos.techidaily.com/2024-approved-how-to-share-twitter-videos-on-facebook/"><u>2024 Approved  How to Share Twitter Videos on Facebook?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/automatic-pc-fix-solutions-on-windows-11/"><u>Automatic PC Fix Solutions on Windows 11</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/boost-your-eso-gaming-experience-ultimate-guide-to-solve-low-fps-issues/"><u>Boost Your ESO Gaming Experience: Ultimate Guide to Solve Low FPS Issues</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/boost-your-gameplay-perfecting-mouse-dpi-for-fortnite-players/"><u>Boost Your Gameplay: Perfecting Mouse DPI for Fortnite Players</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/comprehensive-tutorial-on-configuring-your-graphics-cards-using-nvidias-sli-technology/"><u>Comprehensive Tutorial on Configuring Your Graphics Cards Using Nvidia's SLI Technology</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1723808344194-cyberpunk-2077-display-problems-solved-achieve-crisp-visual-quality-now/"><u>Cyberpunk 2077 Display Problems Solved - Achieve Crisp Visual Quality Now</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/diagnosing-and-repairing-your-seagate-externals-invisibility-on-windows-11/"><u>Diagnosing and Repairing Your Seagate External's Invisibility on Windows 11</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/download-windows-11-rapidly-a-step-by-step-tutorial/"><u>Download Windows 11 Rapidly: A Step-by-Step Tutorial</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1723808359831-effective-winsxs-directory-management-free-up-disk-space-on-windows-11-in-a-flash/"><u>Effective Winsxs Directory Management: Free Up Disk Space on Windows 11 in a Flash!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/effortless-driver-updates-a-how-to-for-windows-10-and-windows-11/"><u>Effortless Driver Updates: A How-To for Windows 10 and Windows 11</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/enhancing-internet-security-using-tor-on-windows-navigate-privately/"><u>Enhancing Internet Security: Using Tor on Windows Navigate Privately</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/enhancing-your-diablo-4-experience-overcoming-stutter-and-fps-dip-on-windows-gaming-pcs/"><u>Enhancing Your Diablo 4 Experience: Overcoming Stutter and FPS Dip on Windows Gaming PCs</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/error-message-deciphered-correcting-camera-failure-codes-0xa00f4244-on-your-windows-desktop/"><u>Error Message Deciphered: Correcting Camera Failure Codes 0xA00F4244 on Your Window's Desktop</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/essential-tips-for-running-fallout-3-seamlessly-on-windows-10-pcs/"><u>Essential Tips for Running Fallout 3 Seamlessly on Windows 10 PCs</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/fortnite-is-blocked-at-your-school-heres-how-to-unblock-it/"><u>Fortnite Is Blocked at Your School? Here’s How to Unblock It</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/guaranteed-solutions-to-overcome-oculus-software-install-problems-on-your-pc-windows-11-and-10/"><u>Guaranteed Solutions to Overcome Oculus Software Install Problems on Your PC (Windows 11 & 10)</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-boot-into-bios-configuration-in-windows-10windows-7-systems/"><u>How to Boot Into BIOS Configuration in Windows 10/Windows 7 Systems</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-clear-cache-on-windows-10/"><u>How to Clear Cache on Windows 10</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-convert-images-to-gif/"><u>How to Convert Images to GIF</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-detect-and-treat-excessive-temperatures-on-your-motherboards-brain/"><u>How to Detect and Treat Excessive Temperatures on Your Motherboard's Brain</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-easily-rectify-error-code-0x80248007-on-your-windows-11-pc-expert-advice/"><u>How to Easily Rectify Error Code 0X80248007 on Your Windows 11 PC: Expert Advice</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-forget-wireless-network-on-windows-11/"><u>How to Forget Wireless Network on Windows 11</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-screenshot-on-windows-heres-the-quick-way/"><u>How to Screenshot on Windows? Here’s the Quick Way!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-successfully-establish-a-miracast-connection-in-windows-1011-solutions-for-common-problems/"><u>How to Successfully Establish a Miracast Connection in Windows 10/11: Solutions for Common Problems</u></a></li>
<li><a href="https://extra-tips.techidaily.com/in-2024-crafting-audible-magic-cropping-and-edits-in-canva-videos/"><u>In 2024, Crafting Audible Magic  Cropping and Edits in Canva Videos</u></a></li>
<li><a href="https://some-tips.techidaily.com/in-2024-unlock-the-potential-of-audience-feedback-on-youtube/"><u>In 2024, Unlock the Potential of Audience Feedback on YouTube</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/in-laminar-flow-the-velocity-profile-across-a-pipe-section-is-parabolic-with-maximum-velocity-at-the-center/"><u>In Laminar Flow, the Velocity Profile Across a Pipe Section Is Parabolic with Maximum Velocity at the Center.</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-obs-stability-avoid-frame-drops-with-these-techniques/"><u>Mastering OBS Stability - Avoid Frame Drops with These Techniques</u></a></li>
<li><a href="https://fix-guide.techidaily.com/reasons-for-samsung-galaxy-m54-5g-stuck-on-startup-screen-and-ways-to-fix-them-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>Reasons for Samsung Galaxy M54 5G Stuck on Startup Screen and Ways To Fix Them | Dr.fone</u></a></li>
<li><a href="https://hardware-reviews.techidaily.com/rigorous-testing-of-sabrent-rocket-nano-2242-a-1tb-ssd-review-for-m2-needs/"><u>Rigorous Testing of Sabrent Rocket Nano 2242: A 1TB SSD Review for M.2 Needs</u></a></li>
<li><a href="https://fox-info.techidaily.com/swift-signature-bg-cleansing-secrets-revealed/"><u>Swift Signature BG Cleansing Secrets Revealed</u></a></li>
<li><a href="https://win-answers.techidaily.com/top-solutions-for-the-2024-rockstar-games-launcher-malfunction-problems/"><u>Top Solutions for the 2024 Rockstar Games Launcher Malfunction Problems</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1723808124632-troubleshoot-and-fix-how-to-restore-your-logitech-k520-keyboards-functionality-swiftly/"><u>Troubleshoot & Fix: How to Restore Your Logitech K520 Keyboard's Functionality Swiftly!</u></a></li>
<li><a href="https://win-answers.techidaily.com/troubleshooting-guide-getting-dolby-atmos-to-function-properly-on-pcs-with-windows-1110/"><u>Troubleshooting Guide: Getting Dolby Atmos to Function Properly on PCs with Windows 11/10</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/wireless-printing-mastery-setup-and-software-download-guide-for-brother-printers/"><u>Wireless Printing Mastery - Setup & Software Download Guide for Brother Printers</u></a></li>
</ul></div>
