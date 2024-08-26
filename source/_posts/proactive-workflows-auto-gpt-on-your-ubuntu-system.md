---
title: "Proactive Workflows: Auto-GPT on Your Ubuntu System"
date: 2024-08-25T17:37:26.885Z
updated: 2024-08-26T17:37:26.885Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Proactive Workflows: Auto-GPT on Your Ubuntu System"
excerpt: "This Article Describes Proactive Workflows: Auto-GPT on Your Ubuntu System"
thumbnail: https://thmb.techidaily.com/1f277a1e71fd10df1b01699e57758c33c523b120ed3c32dedf0e24f515c80068.png
---

## Proactive Workflows: Auto-GPT on Your Ubuntu System

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

 Once copied, paste the key inside the **.env** file. The env file will store all the API keys that you use with Auto-GPT. If you don't need a backend vector database like Pinecone, your OpenAI API key should be enough to use Auto-GPT.

 To set your API key, open the **.env** file using nano:

`nano .env.template`

 To locate the OpenAI API key variable, hold **CTRL + W**, search for “**OPEN\_API\_KEY=**”, and then hit **Enter**.

![Insert API key](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/paste-api-key.jpg)

 Replace the placeholder with your API key by pressing **Ctrl +V** and hitting **Ctrl + S** to save. You can exit the nano text editor by pressing **Ctrl + X**.

 You must also rename the "**.env.template**" file to only "**.env**". To do so, run:

`sudo mv .env.template .env`

## Step 2: Install Auto-GPT Dependencies on Ubuntu

 Auto-GPT uses a lot of Python libraries. You will need to install all the packages using pip and the **requirements.txt** text file that comes with the AutoGPT source code.

 To install all the Python dependencies, run:

`pip install -r requirements.txt`

![Install Auto-GPT requirements](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/5-install-requirements.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=194977&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.blumentals.net/scrfactory/images/screensaver-software.png" border="0">Screensaver Factory, Create stunning professional screensavers within minutes. Create screensavers for yourself, for marketing or unlimited royalty-free commercial distribution. Make screensavers from images, video and swf flash, add background music and smooth sprite and transition effects. Screensaver Factory is very easy to use, and it enables you to make self-installing screensaver files and CDs for easy setup and distribution. Screensaver Factory is the most advanced software of its kind.</a>
<!-- affiliate ads end -->
 Next, try running Auto-GPT using:

`python3 -m autogpt`

![Successful Auto-GPT installation](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/6-success.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=45152835&QTY=1&AFFILIATE=108875&CART=1"><img src="https://download.terabyteunlimited.com/banners/ad_800x450_d.jpg" border="0"></a>
<!-- affiliate ads end -->
 Congratulations! You have successfully installed and set up Auto-GPT on your Ubuntu machine.

## How to Use Auto-GPT on Ubuntu

 With Auto-GPT installed, you can now make your own AI assistant. There are two modes when it comes to using Auto-GPT. In the default mode, you only need to provide a task. Based on the specified task, Auto-GPT will automatically generate your AI assistant's name, its role, and its goals.

![Auto-GPT auto mode](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/1-auto.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4718730&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/ce9a6fb2becc2d235e62b125e9260102/products/copy_vMixCallScreenshot1-large.jpg" border="0">vMix HD - Software based live production. vMix HD includes everything in vMix Basic HD plus 1000 inputs, Video List, 4 Overlay Channels, and 1 vMix Call 
This bundle includes Studio 200 for vMix from Virtualsetworks, HTTP Matrix 1.0 automation scheduler, and 4 introductory training videos from the Udemy vMix Basic to Amazing course. </a>
<!-- affiliate ads end -->
 In manual mode, Auto-GPT will ask you to specify a name, a goal, and up to five goals you want the AI assistant to follow while doing its task. This mode allows you to be in control of how your AI assistant will function.

 To use manual mode, use the following command:

`--manual`

 In this example, we've named our AI assistant, and given it a role to look for product promos, and a few goals on the quality of the promo.

![Auto-GPT manual mode](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/1-manual.jpg)

<!-- affiliate ads begin -->
<a href="https://store.massmailsoftware.com/order/checkout.php?PRODS=1095219&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/dc87c13749315c7217cdc4ac692e704c/banera_for_partners-20_%281%29.jpg" border="0"></a>
<!-- affiliate ads end -->
 Once the name, goals, and role have been provided, your AI assistant will immediately activate and start looping through its thinking and execution process.

 Throughout the process, you can view your AI assistant's thoughts, reasoning, plan, criticism, and next action. Its next action will only be executed once you've given your approval.

![Input-Commands for Auto-GPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/2-input-y.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4729642&QTY=1&AFFILIATE=108875&CART=1">Advanced Find and Replace for Google Sheets, Lifetime subscription</a>
<!-- affiliate ads end -->
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

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4727541&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/5f4f7141b65a730b4efb0e0d51f63e94/products/copy_copy_forexrobotronbox.gif" border="0">Forex Robotron Gold Package</a>
<!-- affiliate ads end -->
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
<li><a href="https://facebook-video-footage.techidaily.com/new-behind-the-sequence-celebrating-youtubes-top-cosmetics-artists-for-2024/"><u>[New] Behind the Sequence  Celebrating YouTube's Top Cosmetics Artists for 2024</u></a></li>
<li><a href="https://twitter-clips.techidaily.com/new-in-2024-quick-tips-sending-tweets-content-via-whatsapp-app/"><u>[New] In 2024, Quick Tips  Sending Tweets' Content via WhatsApp App</u></a></li>
<li><a href="https://fox-info.techidaily.com/new-pixels-into-panoramas-cutting-edge-edits-for-exceptional-results/"><u>[New] Pixels Into Panoramas  Cutting-Edge Edits for Exceptional Results</u></a></li>
<li><a href="https://facebook-video-files.techidaily.com/updated-2024-approved-enhancing-engagement-on-facebook-a-beginners-roadmap/"><u>[Updated] 2024 Approved  Enhancing Engagement on Facebook  A Beginner’s Roadmap</u></a></li>
<li><a href="https://youtube-sure.techidaily.com/ed-2024-approved-enriching-slides-video-incorporation-from-youtube/"><u>[Updated] 2024 Approved  Enriching Slides  Video Incorporation From YouTube</u></a></li>
<li><a href="https://on-screen-recording.techidaily.com/updated-2024-approved-record-everything-pay-nothing-screen-tools-for-all-users/"><u>[Updated] 2024 Approved  Record Everything, Pay Nothing - Screen Tools for All Users</u></a></li>
<li><a href="https://instagram-clips.techidaily.com/updated-in-2024-mastering-vlog-presentation-converting-h-footage-for-vertical-display/"><u>[Updated] In 2024, Mastering Vlog Presentation  Converting H-Footage for Vertical Display</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-boost-for-hr-routine-challenges/"><u>AI Boost for HR Routine Challenges</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/assessing-the-risk-of-employer-sanctions-for-using-chatgpt-tools/"><u>Assessing the Risk of Employer Sanctions for Using ChatGPT Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/bots-banter-beyond-boundaries-will-it-make-us-merry/"><u>Bot's Banter Beyond Boundaries: Will It Make Us Merry?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/crafting-smart-workflows-with-ai-communication-tools/"><u>Crafting Smart Workflows with AI Communication Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/cybersecurity-exposed-a-call-to-action/"><u>Cybersecurity Exposed: A Call to Action</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/dissecting-machine-might-strong-vs-weak-ai/"><u>Dissecting Machine Might: Strong Vs. Weak AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/explore-the-finest-ai-powered-note-taking-software/"><u>Explore the Finest AI-Powered Note-Taking Software</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/fixing-communication-breakdown-with-chatgpts-plugin-services/"><u>Fixing Communication Breakdown with ChatGPT's Plugin Services</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/from-online-to-offline-installed-llama-2-basics/"><u>From Online to Offline: Installed Llama 2 Basics</u></a></li>
<li><a href="https://unlock-android.techidaily.com/full-guide-to-unlock-your-tecno-by-drfone-android/"><u>Full Guide to Unlock Your Tecno</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/grasping-the-operation-and-mechanism-of-predictive-ai/"><u>Grasping the Operation and Mechanism of Predictive AI</u></a></li>
<li><a href="https://android-location-track.techidaily.com/how-to-check-distance-and-radius-on-google-maps-for-your-nokia-c12-plus-drfone-by-drfone-virtual-android/"><u>How to Check Distance and Radius on Google Maps For your Nokia C12 Plus | Dr.fone</u></a></li>
<li><a href="https://win11.techidaily.com/how-to-rescue-your-windows-mail-app-from-the-clutches-of-0x800713f/"><u>How to Rescue Your Windows Mail App From the Clutches of 0X800713F</u></a></li>
<li><a href="https://remote-screen-capture.techidaily.com/in-2024-digital-diary-the-art-of-screen-recording-on-macbook-air/"><u>In 2024, Digital Diary  The Art of Screen Recording on MacBook Air</u></a></li>
<li><a href="https://fox-direct.techidaily.com/in-2024-how-to-use-zoom-in-gmail-best-ways/"><u>In 2024, How to Use Zoom in Gmail [Best Ways]</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/in-2024-life360-circle-everything-you-need-to-know-on-samsung-galaxy-a25-5g-drfone-by-drfone-virtual-android/"><u>In 2024, Life360 Circle Everything You Need to Know On Samsung Galaxy A25 5G | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/intuitive-bavarder-installation-on-linux-distros/"><u>Intuitive Bavarder Installation on Linux Distros</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/language-architecture-showdown-deciphering-gpt-and-bert-mechanics/"><u>Language Architecture Showdown: Deciphering GPT and BERT Mechanics</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-poetry-through-chatgpt-explorations/"><u>Mastering Poetry Through ChatGPT Explorations</u></a></li>
<li><a href="https://extra-lessons.techidaily.com/mastering-sound-top-10-microphones/"><u>Mastering Sound  Top 10 Microphones</u></a></li>
<li><a href="https://tech-haven.techidaily.com/microsofts-strategic-move-to-acquire-blizzard-and-advances-in-ai-for-artistic-expression-explore-with-us-podcast/"><u>Microsoft's Strategic Move to Acquire Blizzard & Advances in AI for Artistic Expression - Explore with Us [Podcast]</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/plot-and-pixel-combining-chatgpt-with-game-script-development/"><u>Plot and Pixel: Combining ChatGPT with Game Script Development</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/propel-your-mobile-search-the-impactful-usage-of-ai-in-bing-app/"><u>Propel Your Mobile Search: The Impactful Usage of AI in Bing App</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revolutionizing-development-with-ai/"><u>Revolutionizing Development with AI</u></a></li>
<li><a href="https://extra-information.techidaily.com/simplifying-connection-combining-linkedin-profile-with-your-tiktok-bio/"><u>Simplifying Connection  Combining LinkedIn Profile with Your TikTok Bio</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/terminal-talk-command-line-tools-to-engage-chatgpt/"><u>Terminal Talk: Command Line Tools to Engage ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/top-6-ai-enhanced-note-apps-for-optimal-information-capture/"><u>Top 6 AI-Enhanced Note Apps for Optimal Information Capture</u></a></li>
<li><a href="https://howto.techidaily.com/what-to-do-if-your-xiaomi-redmi-note-13-pro-5g-auto-does-not-work-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>What To Do if Your Xiaomi Redmi Note 13 Pro 5G Auto Does Not Work | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/your-path-to-advanced-interactions-with-new-chatgpt-extensions/"><u>Your Path to Advanced Interactions with New ChatGPT Extensions</u></a></li>
</ul></div>
