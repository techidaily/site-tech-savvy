---
title: "AI for Everyone: Automating with Auto-GPT on Ubuntu"
date: 2024-12-04T23:30:47.946Z
updated: 2024-12-06T23:17:13.619Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes AI for Everyone: Automating with Auto-GPT on Ubuntu"
excerpt: "This Article Describes AI for Everyone: Automating with Auto-GPT on Ubuntu"
thumbnail: https://thmb.techidaily.com/51c8c0f8bc5e38b3222968b9d07888b2af3d71ae1414dd0e4e4eff08dd69bb83.jpg
---

## AI for Everyone: Automating with Auto-GPT on Ubuntu

 Auto-GPT is an open-source project that allows people to create AI assistants that cater to their needs. These AI assistants are capable of thought and self-criticism and can generate their own prompts to reach a particular set of goals and accomplish their role. It uses the same GPT language model used in the already popular ChatGPT.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 If you would like to harness the power of GPT in the form of an AI assistant, it might interest you to try out Auto-GPT. Here's how you can install and set up Auto-GPT on Ubuntu.

>  Disclaimer: This post includes affiliate links
>
>  If you click on a link and make a purchase, I may receive a commission at no extra cost to you.
>

## Prerequisites to Install Auto-GPT

 To install Auto-GPT, you first need to install the latest Python3 and Git packages on your computer.

 Python is extensively used in Auto-GPT. To [install the latest version of Python on Ubuntu](https://www.makeuseof.com/install-python-ubuntu/), open up a terminal and upgrade and update the packages using:

`sudo apt update && sudo apt upgrade`

 Now, add the deadsnakes PPA with the following command:

`sudo add-apt-repository ppa:deadsnakes/ppa`

 Install the latest version of Python with:

`sudo apt install python3.11`

 Replace "python3.11" in the above command with the latest Python version at the time.

 After installation, check if pip is already installed on your machine:

`pip --version`

 If you're using Python 3.4 or above, pip should already be installed. But in case it's missing, install pip with:

`sudo apt install python3-pip`

 Now that you've installed the latest Python version and pip on Ubuntu, install Git and clone the Auto-GPT repository using **git clone**:

`sudo apt install git  
sudo git clone https://github.com/Significant-Gravitas/Auto-GPT.git`

 Change the directory to the newly created Auto-GPT code folder using [the cd command](https://www.makeuseof.com/cd-command-in-linux/):

`cd Auto-GPT`

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/0OxkndZbIA4?si=TWJlkTbYKsVag8-q" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## Step 1: Configure Auto-GPT on Ubuntu

 Now that you've correctly set up the environment for Auto-GPT, you need to configure your OpenAI API key as an environment variable.

 To get an OpenAI API key, sign up for an account by heading over to [platform.openai.com](https://platform.openai.com/signup). Ensure you set up your payment method to use OpenAI's GPT product.

 After logging into your account, click on the profile image on the top right and select **View API Keys**.

 To generate an API key, click on the **Create new secret key** button, add any name, and copy the API key by pressing **Ctrl + C** or clicking the copy icon. You'll use this key as credentials for your AI assistant to use OpenAI's GPT technology.

![Creating OpenAI API key](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/3-get-api-key.jpg)

 Once copied, paste the key inside the **.env** file. The env file will store all the API keys that you use with Auto-GPT. If you don't need a backend vector database like Pinecone, your OpenAI API key should be enough to use Auto-GPT.

 To set your API key, open the **.env** file using nano:

`nano .env.template`

 To locate the OpenAI API key variable, hold **CTRL + W**, search for “**OPEN\_API\_KEY=**”, and then hit **Enter**.

![Insert API key](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/paste-api-key.jpg)

 Replace the placeholder with your API key by pressing **Ctrl +V** and hitting **Ctrl + S** to save. You can exit the nano text editor by pressing **Ctrl + X**.

 You must also rename the "**.env.template**" file to only "**.env**". To do so, run:

`sudo mv .env.template .env`

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/xIP8ktrmOdg?si=zRnjbGzM6PDx2jCq" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## Step 2: Install Auto-GPT Dependencies on Ubuntu

 Auto-GPT uses a lot of Python libraries. You will need to install all the packages using pip and the **requirements.txt** text file that comes with the AutoGPT source code.

 To install all the Python dependencies, run:

`pip install -r requirements.txt`

![Install Auto-GPT requirements](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/5-install-requirements.jpg)

 Next, try running Auto-GPT using:

`python3 -m autogpt`

![Successful Auto-GPT installation](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/6-success.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/pRR3Oq03EuE?si=ZTy8-WH0AesA9zRh" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Congratulations! You have successfully installed and set up Auto-GPT on your Ubuntu machine.

## How to Use Auto-GPT on Ubuntu

 With Auto-GPT installed, you can now make your own AI assistant. There are two modes when it comes to using Auto-GPT. In the default mode, you only need to provide a task. Based on the specified task, Auto-GPT will automatically generate your AI assistant's name, its role, and its goals.

![Auto-GPT auto mode](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/1-auto.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/wVVp-GggK3U?si=RJb1ClNQV7GjTu_3" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 In manual mode, Auto-GPT will ask you to specify a name, a goal, and up to five goals you want the AI assistant to follow while doing its task. This mode allows you to be in control of how your AI assistant will function.

 To use manual mode, use the following command:

`--manual`

 In this example, we've named our AI assistant, and given it a role to look for product promos, and a few goals on the quality of the promo.

![Auto-GPT manual mode](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/1-manual.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/DEqoiNArwjQ?si=oaL_lgnI-RxY5Qy_" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Once the name, goals, and role have been provided, your AI assistant will immediately activate and start looping through its thinking and execution process.

 Throughout the process, you can view your AI assistant's thoughts, reasoning, plan, criticism, and next action. Its next action will only be executed once you've given your approval.

![Input-Commands for Auto-GPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/2-input-y.jpg)

 You can approve the AI's next action by typing "**y**" for yes. If you don't want the AI to continue with its plans, you can type "**n**" for no and exit.

 If you trust your AI assistant and don't want to continue monitoring all of its thoughts and actions, you can type "**y -(number)**". For example, if you want Auto-GPT to execute its next five actions, you can type "**y -5**". Furthermore, if you want to provide feedback to your AI assistant, you can also type your prompt as input.

 In this example, our assistant has been looping around the same thoughts, plans, and executions three times now. So we decided to give it feedback to stop as its initial efforts were already enough.

![Providing human feedback to Auto-GPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/3-human-feedback.jpg)

 Once your AI assistant finishes its task, you can view its final output by opening the **/Auto-GPT-x.x.x/autogpt/auto\_gpt\_workspace** directory.

![Successful Auto-GPT session](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/success-1.jpg)

 Success! Our AI assistant gave us a list of active promo codes for the mouse we were looking for.

## Limitations of Auto-GPT

 Although Auto-GPT gave us some pretty promising results, it still isn't as powerful or useful as it was initially hyped to be. During our testing, any slightly complex task often resulted in the AI assistant looping through the same pattern of thoughts and actions, which eventually failed.

 A big part of this problem was the AI’s inability to handle website ads, cookies, log-in pages, and pop-ups. It was likely caused by the fact that Auto-GPT is still in its early development phase.

 So for now, you should only use Auto-GPT as a way to play and experiment with AI assistants.

## Auto-GPT Will Keep Getting Better and Better

 Auto-GPT is not as powerful as it should be due to its current development stage and the limited access to GPT-4\. However, these wouldn't last long as Auto-GPT is gaining lots of traction and support from people worldwide.

 The development of Auto-GPT will likely continue until it gets to a mature and stable state where many useful features get implemented. It is only a matter of time before Auto-GPT becomes a practical tool for our personal, professional, and business applications.

**SCROLL TO CONTINUE WITH CONTENT**

 If you would like to harness the power of GPT in the form of an AI assistant, it might interest you to try out Auto-GPT. Here's how you can install and set up Auto-GPT on Ubuntu.

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
<li><a href="https://youtube-help.techidaily.com/new-methodology-to-purging-your-youtube-watch-later-playlist/"><u>[New] Methodology to Purging Your YouTube Watch Later Playlist</u></a></li>
<li><a href="https://extra-skills.techidaily.com/updated-mastering-the-art-of-softening-dynamics-in-fl-studio-soundscape/"><u>[Updated] Mastering the Art of Softening Dynamics in FL Studio Soundscape</u></a></li>
<li><a href="https://screen-sharing-recording.techidaily.com/updated-ultimate-racing-game-compilation-for-2024/"><u>[Updated] Ultimate Racing Game Compilation for 2024</u></a></li>
<li><a href="https://eaxpv-info.techidaily.com/accelerating-performance-microsoft-edges-speed-enhancements/"><u>Accelerating Performance: Microsoft Edge's Speed Enhancements</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/agentgpt-deployment-made-a-breeze-for-browser-users/"><u>AgentGPT Deployment Made a Breeze for Browser Users</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/auto-gpt-explained-a-comparative-study-with-chatgpt/"><u>Auto-GPT Explained – A Comparative Study with ChatGPT</u></a></li>
<li><a href="https://android-location-track.techidaily.com/best-anti-tracker-software-for-vivo-y27-4g-drfone-by-drfone-virtual-android/"><u>Best Anti Tracker Software For Vivo Y27 4G | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/boost-your-instruction-crafting-skills-using-these-innovative-aids/"><u>Boost Your Instruction Crafting Skills Using These Innovative Aids</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/finewoven-discontinued-by-apple-in-favor-of-new-partnership-with-beats-for-case-production-zdnet/"><u>FineWoven Discontinued by Apple in Favor of New Partnership with Beats for Case Production - ZDNet</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/how-do-i-sign-a-wpd-file-electronically-by-ldigisigner-sign-a-word-sign-a-word/"><u>How do i sign a .wpd file electronically</u></a></li>
<li><a href="https://blog-min.techidaily.com/how-to-honor-x7b-get-deleted-phone-number-back-with-ease-and-safety-by-fonelab-android-recover-contacts/"><u>How to Honor X7b Get Deleted Phone Number Back with Ease and Safety</u></a></li>
<li><a href="https://vp-tips.techidaily.com/in-2024-ultimate-guide-to-affordable-vector-art-websites/"><u>In 2024, Ultimate Guide to Affordable Vector Art Websites</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/insights-into-the-unique-benefits-of-business-focused-gpt/"><u>Insights Into the Unique Benefits of Business-Focused GPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/tech-value-showdown-get-iphone-ipad-apple-watch-airpods-and-mac-cheaper-than-vision-pro/"><u>Tech Value Showdown: Get iPhone, iPad, Apple Watch, AirPods, and Mac Cheaper than Vision Pro</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/top-apple-watch-offers-in-july-2024-find-the-best-savings-on-latest-models-tech-news-today/"><u>Top Apple Watch Offers in July 2024: Find the Best Savings on Latest Models | Tech News Today</u></a></li>
</ul></div>

