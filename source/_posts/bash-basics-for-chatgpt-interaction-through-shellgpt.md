---
title: Bash Basics for ChatGPT Interaction Through ShellGPT
date: 2024-10-10T21:19:54.862Z
updated: 2024-10-14T23:05:48.857Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Bash Basics for ChatGPT Interaction Through ShellGPT
excerpt: This Article Describes Bash Basics for ChatGPT Interaction Through ShellGPT
thumbnail: https://thmb.techidaily.com/dc4a82d976964b1f2e7b859f5b2f6939dbc4ceccf4ea97b9d7a6a6bfaea9749c.jpg
---

## Bash Basics for ChatGPT Interaction Through ShellGPT

 Artificial intelligence has emerged as a new-age sensation, leaving everything behind in the dust. With new additions daily, there is a lot to look forward to.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 People use this multi-faceted, ubiquitous tool to crack jokes, write codes and even answer the most random questions. It’s easy to use ChatGPT on other OSes, so, as a Linux user, why should you stay behind?

 You too can enjoy ChatGPT’s Linux avatar, ShellGPT. Here's how to install and use the AI tool from your Ubuntu terminal in a few easy steps.

>  Disclaimer: This post includes affiliate links
>
>  If you click on a link and make a purchase, I may receive a commission at no extra cost to you.
>

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
<a href="https://aligracehair.sjv.io/c/5597632/1934258/19272" target="_top" id="1934258">
  <img src="//a.impactradius-go.com/display-ad/19272-1934258" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1934258/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

## Step 2: Install and Set Up a Virtual Environment Using Python

 Now that Python and PIP are ready, you can set up Python's virtual environment to make the machine environment conducive for installing and running ShellGPT. Virtual environments are ideal for running isolated programs since they can avoid library conflicts.

 With a virtual environment in tow, you can limit the interactions between your system's and virtual environment's programs while performing different executions in silos.

 Using a virtual environment is an optional step, to avoid any unforeseen mishaps while installing and using Python libraries.

 To create a virtual environment using Python, you need to install the **venv** module:

`sudo apt install python3-venv -y`

![Ubuntu terminal window code snippets](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/install-virtual-environment-module-in-ubuntu.jpg)

<!-- affiliate ads begin -->
<a href="https://imp.i357552.net/c/5597632/977686/11832" target="_top" id="977686">
  <img src="//a.impactradius-go.com/display-ad/11832-977686" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://imp.i357552.net/i/5597632/977686/11832" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://25home.pxf.io/c/5597632/2148644/16836" target="_top" id="2148644">
  <img src="//a.impactradius-go.com/display-ad/16836-2148644" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://25home.pxf.io/i/5597632/2148644/16836" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

## Step 3: Generate an OpenAPI Key

 Since the virtual environment is ready, you must connect the OpenAI services and your Ubuntu machine to run ShellGPT. For this purpose, you must navigate to [OpenAI's website](https://openai.com/) and create an account there.

 If you have an existing account, you can log in with your credentials and navigate to your profile image, located on the top right-hand side of the website.

 Click on **View API Keys**, followed by **Create new secret key**.

![OpenAI website interface showing a drop-down menu](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/view-api-keys-on-openai-website.jpg)

<!-- affiliate ads begin -->
<span id="1982457">
					<video width="576" height="240" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1982457.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/22993-1982457">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1982457.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:360px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fhomestyler.sjv.io%2Fc%2F5597632%2F1982457%2F22993'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1982457/22993" style="position:absolute;visibility:hidden;" border="0" />
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

 Save and exit the editor. Then, use the source command to enable the changes.

`source ./bashrc`

 Finally, verify the API key with the **env** command.

`env`

![List of variables in a linux terminal](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/check-secret-key-in-env-list.jpg)

 Your **OPENAI\_API\_KEY** environment variable should be listed in the output.

<!-- affiliate ads begin -->
<a href="https://ephamedtechinc.pxf.io/c/5597632/2136624/26400" target="_top" id="2136624">
  <img src="//a.impactradius-go.com/display-ad/26400-2136624" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://ephamedtechinc.pxf.io/i/5597632/2136624/26400" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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
<span id="1793213">
					<video width="864" height="1296" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1793213.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/19135-1793213">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1793213.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:540px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Ftinyland.pxf.io%2Fc%2F5597632%2F1793213%2F19135'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1793213/19135" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

## Using ShellGPT for Generating Code

 You can use your ShellGPT for generating code as well. You can do it by passing the right command with the **sgpt** command:

`sgpt --code "print the Fibonacci series"`

![Ubuntu terminal window with code snippets](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/shellgpt-code-reponse.jpg)

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1925570/19272" target="_top" id="1925570">
  <img src="//a.impactradius-go.com/display-ad/19272-1925570" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1925570/19272" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://extra-tips.techidaily.com/new-best-bigger-picture-tvs-ranked-10/"><u>[New] Best Bigger Picture TVs Ranked #10</u></a></li>
<li><a href="https://fox-info.techidaily.com/new-in-2024-unique-outro-music-files-at-your-fingertips-free/"><u>[New] In 2024, Unique Outro Music Files at Your Fingertips - Free</u></a></li>
<li><a href="https://vp-tips.techidaily.com/new-in-2024-zenith-pinnacle-prodigy-review/"><u>[New] In 2024, Zenith Pinnacle Prodigy Review</u></a></li>
<li><a href="https://article-knowledge.techidaily.com/new-master-iphone-podcast-downloads-a-comprehensible-approach-for-2024/"><u>[New] Master iPhone Podcast Downloads A Comprehensible Approach for 2024</u></a></li>
<li><a href="https://screen-activity-recording.techidaily.com/updated-discovering-screenflow-on-macos-an-expert-review/"><u>[Updated] Discovering ScreenFlow on MacOS An Expert Review</u></a></li>
<li><a href="https://desktop-recording.techidaily.com/updated-melodymentor-detailed-sound-review/"><u>[Updated] MelodyMentor Detailed Sound Review</u></a></li>
<li><a href="https://article-files.techidaily.com/comprehensible-guide-to-azure-voice-to-text/"><u>Comprehensible Guide to Azure Voice to Text</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/guide-to-efficiently-deploy-chatgpt-extensions/"><u>Guide to Efficiently Deploy ChatGPT Extensions</u></a></li>
<li><a href="https://article-posts.techidaily.com/in-2024-unlock-creative-potential-with-10-best-backdrop-modification-software/"><u>In 2024, Unlock Creative Potential with 10 Best Backdrop Modification Software</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/introducing-game-changing-ai-to-craftsmanship/"><u>Introducing Game-Changing AI to Craftsmanship</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/steering-clear-of-mistakes-with-ai-generators/"><u>Steering Clear of Mistakes with AI Generators</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-unnoticed-artifacts-by-chatgpt/"><u>The Unnoticed Artifacts by ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/traps-in-tokens-exposing-fake-bingpt-projects/"><u>Traps in Tokens: Exposing Fake BinGPT Projects</u></a></li>
</ul></div>

