---
title: "GPT in Terminal: How to Engage via ShellGPT Bash Commands"
date: 2024-12-26T17:42:55.297Z
updated: 2024-12-27T17:02:09.090Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes GPT in Terminal: How to Engage via ShellGPT Bash Commands"
excerpt: "This Article Describes GPT in Terminal: How to Engage via ShellGPT Bash Commands"
thumbnail: https://thmb.techidaily.com/5ef4b9be2cc03e1f5bba8134aa6b00b2355f4bf8946df71748d869f7b05769b2.jpg
---

## GPT in Terminal: How to Engage via ShellGPT Bash Commands

 Artificial intelligence has emerged as a new-age sensation, leaving everything behind in the dust. With new additions daily, there is a lot to look forward to.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 People use this multi-faceted, ubiquitous tool to crack jokes, write codes and even answer the most random questions. It’s easy to use ChatGPT on other OSes, so, as a Linux user, why should you stay behind?

 You too can enjoy ChatGPT’s Linux avatar, ShellGPT. Here's how to install and use the AI tool from your Ubuntu terminal in a few easy steps.

>  Disclaimer: This post includes affiliate links
>
>  If you click on a link and make a purchase, I may receive a commission at no extra cost to you.
>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/Zgwn5kVI5V4?si=1j6j4OuSSndFieXU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## What’s ShellGPT, ChatGPT’s Equivalent Linux Namesake?

 ShellGPT, as it is more commonly known, is ChatGPT’s command-line equivalent, through which users can use and engage with the AI chatbot via their Linux terminal. The chatbot draws power from OpenAI’s Large Language Model, providing intelligent user recommendations.

 Large Language Models (LLMs) are becoming a hot topic of discussion since you can easily [run LLM-enabled chatbots on your Raspberry Pi](https://www.makeuseof.com/raspberry-pi-large-language-model/).

 Sounds intriguing, doesn’t it?

 If you have experience interacting with ChatGPT, you will love this alternate Linux shell version.

 What’s the benefit of installing ShellGPT on your machine? It’s simple; you don’t need to type in unnecessary long commands or head to your browser. Instead, you can perform all possible tasks from the comfort of your Linux terminal.

 Before installing ShellGPT on your Ubuntu machine, here are a few prerequisites to take care of.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/hZsnjxeSh1U?si=hZIfzQPDNX5KtOCg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/wNhKhWc0wLc?si=1XLYV0sXV52Xc0lu" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/6X24fPKs6AE?si=YtQy-8zy7GifgfA7" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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
<iframe width="560" height="315" src="https://www.youtube.com/embed/jjGL9wFdlbo?si=Vb1JgZqRXNc03UGG" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/UcplMvRBulA?si=iBonbwDS1v7RAlHK" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## Using ShellGPT for Generating Code

 You can use your ShellGPT for generating code as well. You can do it by passing the right command with the **sgpt** command:

`sgpt --code "print the Fibonacci series"`

![Ubuntu terminal window with code snippets](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/shellgpt-code-reponse.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/nlwr9LjJ-ng?si=I6UNAtfBkY2FTceu" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://fox-boxes.techidaily.com/new-2024-approved-the-end-of-acid-pro-top-software-alternatives-reviewed/"><u>[New] 2024 Approved The End of ACID Pro Top Software Alternatives Reviewed</u></a></li>
<li><a href="https://facebook-video-recording.techidaily.com/updated-2024-approved-expert-tips-to-enhance-your-live-fb-broadcast-quality-pcmac/"><u>[Updated] 2024 Approved Expert Tips to Enhance Your Live FB Broadcast Quality (PC/Mac)</u></a></li>
<li><a href="https://youtube-zero.techidaily.com/approved-comprehensive-but-concise-guide-to-keyers-techniques/"><u>2024 Approved Comprehensive but Concise Guide to Keyers' Techniques</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-impact-will-gpt-displace-human-roles/"><u>AI Impact: Will GPT Displace Human Roles?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/arena-of-artificial-intelligence-gpt-vs-bing-conversation-masters/"><u>Arena of Artificial Intelligence: GPT Vs. Bing Conversation Masters</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/finding-your-mantra-path-gpts-role-in-meditative-habits/"><u>Finding Your Mantra Path: GPT's Role in Meditative Habits</u></a></li>
<li><a href="https://ai-topics.techidaily.com/hit-the-jackpot-on-pc-gear-get-your-hands-on-alienware-aurora-with-rtx-4080-and-core-i9-save-500-dollars-now/"><u>Hit the Jackpot on PC Gear! Get Your Hands-On Alienware Aurora with RTX 4080 & Core I9, Save 500 Dollars Now</u></a></li>
<li><a href="https://android-unlock.techidaily.com/how-can-we-unlock-our-vivo-v29-phone-screen-by-drfone-android/"><u>How Can We Unlock Our Vivo V29 Phone Screen?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/i-used-chatgpt-to-script-a-podcast-heres-what-happened/"><u>I Used ChatGPT to Script a Podcast: Here's What Happened</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/industry-shift-is-gpt-the-new-workforce-engine/"><u>Industry Shift: Is GPT the New Workforce Engine?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/overriding-character-constraints-in-chatgpt/"><u>Overriding Character Constraints in ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/peeking-into-the-world-of-shap-explainer-by-openai/"><u>Peeking Into the World of SHAP Explainer by OpenAI</u></a></li>
<li><a href="https://fox-glue.techidaily.com/premier-networks-global-gems-with-local-spectacles-2024/"><u>Premier Networks Global Gems with Local Spectacles, 2024</u></a></li>
<li><a href="https://extra-skills.techidaily.com/rhythmic-resonance-select-sites-for-downloading-tones-for-2024/"><u>Rhythmic Resonance Select Sites for Downloading Tones for 2024</u></a></li>
<li><a href="https://discover-amazing.techidaily.com/the-ultimate-guide-transforming-your-audible-aax-downloads-into-crystal-clear-mp3s/"><u>The Ultimate Guide: Transforming Your Audible AAX Downloads Into Crystal Clear MP3s</u></a></li>
<li><a href="https://hardware-tips.techidaily.com/top-ipad-pro-usb-c-hub-unveiled-by-zdnet-a-must-have-accessory-when-you-need-it-most/"><u>Top iPad Pro USB-C Hub Unveiled by ZDNet: A Must-Have Accessory When You Need It Most</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unlocking-ios-15-find-out-eligible-iphone-models-and-begin-your-download-today-zdnet/"><u>Unlocking iOS 15: Find Out Eligible iPhone Models & Begin Your Download Today | ZDNet</u></a></li>
</ul></div>

