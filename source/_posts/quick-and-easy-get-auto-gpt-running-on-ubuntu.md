---
title: "Quick & Easy: Get Auto-GPT Running on Ubuntu"
date: 2025-01-29T22:33:49.112Z
updated: 2025-02-02T20:39:37.901Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Quick & Easy: Get Auto-GPT Running on Ubuntu"
excerpt: "This Article Describes Quick & Easy: Get Auto-GPT Running on Ubuntu"
thumbnail: https://thmb.techidaily.com/a9c4773f553465442855522d53311e6c839ae2e2683158738f923e4b38285f41.jpg
---

## Quick & Easy: Get Auto-GPT Running on Ubuntu

 Auto-GPT is an open-source project that allows people to create AI assistants that cater to their needs. These AI assistants are capable of thought and self-criticism and can generate their own prompts to reach a particular set of goals and accomplish their role. It uses the same GPT language model used in the already popular ChatGPT.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 If you would like to harness the power of GPT in the form of an AI assistant, it might interest you to try out Auto-GPT. Here's how you can install and set up Auto-GPT on Ubuntu.

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

## Step 1: Configure Auto-GPT on Ubuntu

 Now that you've correctly set up the environment for Auto-GPT, you need to configure your OpenAI API key as an environment variable.

 To get an OpenAI API key, sign up for an account by heading over to [platform.openai.com](https://platform.openai.com/signup). Ensure you set up your payment method to use OpenAI's GPT product.

 After logging into your account, click on the profile image on the top right and select **View API Keys**.

 To generate an API key, click on the **Create new secret key** button, add any name, and copy the API key by pressing **Ctrl + C** or clicking the copy icon. You'll use this key as credentials for your AI assistant to use OpenAI's GPT technology.

![Creating OpenAI API key](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/3-get-api-key.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/K7fATC_lI7o?si=UFotPJqflDRZr-mv" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Once copied, paste the key inside the **.env** file. The env file will store all the API keys that you use with Auto-GPT. If you don't need a backend vector database like Pinecone, your OpenAI API key should be enough to use Auto-GPT.

 To set your API key, open the **.env** file using nano:

`nano .env.template`

 To locate the OpenAI API key variable, hold **CTRL + W**, search for “**OPEN\_API\_KEY=**”, and then hit **Enter**.

![Insert API key](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/paste-api-key.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/1KKovVi9epE?si=EF7KA7b4KsEpWA-M" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Replace the placeholder with your API key by pressing **Ctrl +V** and hitting **Ctrl + S** to save. You can exit the nano text editor by pressing **Ctrl + X**.

 You must also rename the "**.env.template**" file to only "**.env**". To do so, run:

`sudo mv .env.template .env`

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/0dOfcihxjiw?si=_fkp1S1Uw0N1dp6b" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## Step 2: Install Auto-GPT Dependencies on Ubuntu

 Auto-GPT uses a lot of Python libraries. You will need to install all the packages using pip and the **requirements.txt** text file that comes with the AutoGPT source code.

 To install all the Python dependencies, run:

`pip install -r requirements.txt`

![Install Auto-GPT requirements](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/5-install-requirements.jpg)

 Next, try running Auto-GPT using:

`python3 -m autogpt`

![Successful Auto-GPT installation](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/6-success.jpg)

 Congratulations! You have successfully installed and set up Auto-GPT on your Ubuntu machine.

## How to Use Auto-GPT on Ubuntu

 With Auto-GPT installed, you can now make your own AI assistant. There are two modes when it comes to using Auto-GPT. In the default mode, you only need to provide a task. Based on the specified task, Auto-GPT will automatically generate your AI assistant's name, its role, and its goals.

![Auto-GPT auto mode](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/1-auto.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/4DJKH1uY7P0?si=tCG66XVlbwSKoATj" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 In manual mode, Auto-GPT will ask you to specify a name, a goal, and up to five goals you want the AI assistant to follow while doing its task. This mode allows you to be in control of how your AI assistant will function.

 To use manual mode, use the following command:

`--manual`

 In this example, we've named our AI assistant, and given it a role to look for product promos, and a few goals on the quality of the promo.

![Auto-GPT manual mode](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/1-manual.jpg)

 Once the name, goals, and role have been provided, your AI assistant will immediately activate and start looping through its thinking and execution process.

 Throughout the process, you can view your AI assistant's thoughts, reasoning, plan, criticism, and next action. Its next action will only be executed once you've given your approval.

![Input-Commands for Auto-GPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/2-input-y.jpg)

 You can approve the AI's next action by typing "**y**" for yes. If you don't want the AI to continue with its plans, you can type "**n**" for no and exit.

 If you trust your AI assistant and don't want to continue monitoring all of its thoughts and actions, you can type "**y -(number)**". For example, if you want Auto-GPT to execute its next five actions, you can type "**y -5**". Furthermore, if you want to provide feedback to your AI assistant, you can also type your prompt as input.

 In this example, our assistant has been looping around the same thoughts, plans, and executions three times now. So we decided to give it feedback to stop as its initial efforts were already enough.

![Providing human feedback to Auto-GPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/3-human-feedback.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/MTb4xHzeQEk?si=9Sqq-gFWnHc8x3_P" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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
<li><a href="https://fox-http.techidaily.com/updated-infinite-professional-slideshow-resource-for-businesses/"><u>[Updated] Infinite Professional Slideshow Resource for Businesses</u></a></li>
<li><a href="https://fox-access.techidaily.com/updated-masterful-zoom-techniques-simple-iphone-solutions-for-2024/"><u>[Updated] Masterful Zoom Techniques Simple iPhone Solutions for 2024</u></a></li>
<li><a href="https://win-news.techidaily.com/adjust-audio-levels-using-control-panel-a-step-by-step-guide-from-yl-software-solutions/"><u>Adjust Audio Levels Using Control Panel: A Step-by-Step Guide From YL Software Solutions</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/are-apples-airpods-pro-released-still-worth-your-investment-a-comprehensive-analysis/"><u>Are Apple's AirPods Pro, Released , Still Worth Your Investment? A Comprehensive Analysis</u></a></li>
<li><a href="https://extra-hints.techidaily.com/bridging-gaps-preventing-video-holds-in-photoshoots/"><u>Bridging Gaps Preventing Video Holds in Photoshoots</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-strategies-for-streamlined-3d-printing-processes/"><u>ChatGPT Strategies for Streamlined 3D Printing Processes</u></a></li>
<li><a href="https://fox-web3.techidaily.com/free-bootstrap-ui-toolkit-by-creative-tim-essential-tools-for-efficient-development/"><u>Free Bootstrap UI Toolkit by Creative Tim: Essential Tools for Efficient Development</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-ensure-the-integrity-of-ios-ai-apps/"><u>How to Ensure the Integrity of iOS AI Apps</u></a></li>
<li><a href="https://location-social.techidaily.com/in-2024-set-your-preferred-job-location-on-linkedin-app-of-your-apple-iphone-6s-plus-drfone-by-drfone-virtual-ios/"><u>In 2024, Set Your Preferred Job Location on LinkedIn App of your Apple iPhone 6s Plus | Dr.fone</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/in-2024-top-10-meizu-android-sim-unlock-apk-by-drfone-android/"><u>In 2024, Top 10 Meizu Android SIM Unlock APK</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/intuitive-talking-to-ai-try-this-chrome-tool/"><u>Intuitive Talking to AI? Try This Chrome Tool</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/iphone-showdown-unveiling-differences-between-iphone-16-pro-and-14-pro-worth-your-upgrade/"><u>IPhone Showdown : Unveiling Differences Between iPhone 16 Pro and 14 Pro - Worth Your Upgrade?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/limited-offer-on-presidents-day-save-big-and-score-200-off-the-latest-macbook-pro-with-apple-silicon-m3-pro-chip-exclusive-at-zdnet-shop/"><u>Limited Offer on Presidents' Day: Save Big & Score $200 Off the Latest MacBook Pro with Apple Silicon - M3 Pro Chip Exclusive at ZDNet Shop</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-chatgpt-cultivating-daily-mindfulness-practice/"><u>Mastering ChatGPT: Cultivating Daily Mindfulness Practice</u></a></li>
<li><a href="https://fox-zaraz.techidaily.com/mastering-folder-synchronization-step-by-step-tips-for-a-harmonized-digital-experience/"><u>Mastering Folder Synchronization: Step-by-Step Tips for a Harmonized Digital Experience</u></a></li>
<li><a href="https://mondly-stories.techidaily.com/mondly-and-apple-lead-charge-in-education-tech-with-10-ranking/"><u>Mondly and Apple Lead Charge in Education Tech with #10 Ranking</u></a></li>
<li><a href="https://media-tips.techidaily.com/multiple-techniques-to-transfer-mts-files-onto-your-ipad/"><u>Multiple Techniques to Transfer MTS Files Onto Your iPad</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unlocking-the-solution-overcome-the-risky-battery-flaw-in-your-airtags-and-compatible-gadgets-expert-tips/"><u>Unlocking the Solution: Overcome the Risky Battery Flaw in Your AirTags and Compatible Gadgets - Expert Tips</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/voice-enabled-chatgpt-for-your-android-device/"><u>Voice-Enabled ChatGPT for Your Android Device</u></a></li>
</ul></div>

