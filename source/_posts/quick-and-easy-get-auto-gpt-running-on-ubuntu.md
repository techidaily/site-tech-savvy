---
title: "Quick & Easy: Get Auto-GPT Running on Ubuntu"
date: 2024-08-25T17:32:32.981Z
updated: 2024-08-26T17:32:32.981Z
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
<a href="https://natural-cycles.sjv.io/c/5597632/2072200/17885" target="_top" id="2072200"><img src="//a.impactradius-go.com/display-ad/17885-2072200" border="0" alt="" width="728" height="90"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2072200/17885" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 Next, try running Auto-GPT using:

`python3 -m autogpt`

![Successful Auto-GPT installation](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/6-success.jpg)

 Congratulations! You have successfully installed and set up Auto-GPT on your Ubuntu machine.

## How to Use Auto-GPT on Ubuntu

 With Auto-GPT installed, you can now make your own AI assistant. There are two modes when it comes to using Auto-GPT. In the default mode, you only need to provide a task. Based on the specified task, Auto-GPT will automatically generate your AI assistant's name, its role, and its goals.

![Auto-GPT auto mode](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/1-auto.jpg)

<!-- affiliate ads begin -->
<a href="https://estore.winxdvd.com/order/checkout.php?PRODS=4081991&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.winxdvd.com/affiliate/new-banner/wt-500x500.jpg" border="0"></a>
<!-- affiliate ads end -->
 In manual mode, Auto-GPT will ask you to specify a name, a goal, and up to five goals you want the AI assistant to follow while doing its task. This mode allows you to be in control of how your AI assistant will function.

 To use manual mode, use the following command:

`--manual`

 In this example, we've named our AI assistant, and given it a role to look for product promos, and a few goals on the quality of the promo.

![Auto-GPT manual mode](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/1-manual.jpg)

<!-- affiliate ads begin -->
<a href="https://purchase.swifdoo.com/order/checkout.php?PRODS=38709260&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/8b932759a5a04ddb34bf79e3f9072e4b/products/Product%20box%20white-1024x1024.png" border="0">SwifDoo PDF Perpetual (2-PC)  Free upgrade. No monthly fees ever. </a>
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

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4709458&QTY=1&AFFILIATE=108875&CART=1"><img src="https://3d-kstudio.com/wp-content/uploads/2014/02/Project-Manager-3D-Models-4-800x800.jpg" border="0">Project Manager - Asset Browser for 3Ds Max</a>
<!-- affiliate ads end -->
 Success! Our AI assistant gave us a list of active promo codes for the mouse we were looking for.

<!-- affiliate ads begin -->
<a href="https://order.glarysoft.com/order/checkout.php?PRODS=4535075&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/6734fa703f6633ab896eecbdfad8953a/products/GU-500_672.png" border="0">Glary Utilities PRO -  Premium all-in-one utility to clean, speed up, maintain and protect your PC</a>
<!-- affiliate ads end -->
## Limitations of Auto-GPT

 Although Auto-GPT gave us some pretty promising results, it still isn't as powerful or useful as it was initially hyped to be. During our testing, any slightly complex task often resulted in the AI assistant looping through the same pattern of thoughts and actions, which eventually failed.

 A big part of this problem was the AI’s inability to handle website ads, cookies, log-in pages, and pop-ups. It was likely caused by the fact that Auto-GPT is still in its early development phase.

 So for now, you should only use Auto-GPT as a way to play and experiment with AI assistants.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4537547&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/4b0a0290ad7df100b77e86839989a75e/products/vcfpro.png" border="0">Video Converter Factory Pro</a>
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
<li><a href="https://vp-tips.techidaily.com/new-2024-approved-advanced-3d-text-techniques-in-ai/"><u>[New] 2024 Approved  Advanced 3D Text Techniques in AI</u></a></li>
<li><a href="https://snapchat-videos.techidaily.com/new-2024-approved-smooth-operations-direct-backup-of-camera-roll-images-to-social-media-apps/"><u>[New] 2024 Approved  Smooth Operations  Direct Backup of Camera Roll Images to Social Media Apps</u></a></li>
<li><a href="https://facebook-clips.techidaily.com/updated-2024-approved-achieve-synchronicity-with-your-browser-and-fbs-autoplay-feature/"><u>[Updated] 2024 Approved  Achieve Synchronicity with Your Browser and FB's Autoplay Feature</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/updated-2024-approved-free-best-10-video-editing-apps-to-edit-and-make-instagram-reels/"><u>[Updated] 2024 Approved  FREE Best 10 Video Editing Apps to Edit and Make Instagram Reels</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-optimization-for-streamlined-hr-tasks/"><u>AI Optimization for Streamlined HR Tasks</u></a></li>
<li><a href="https://meme-emoji.techidaily.com/best-10-emoji-makers-to-create-your-own-emojispconlineandroidiphone-for-2024/"><u>Best 10 Emoji Makers to Create Your Own EmojisPC/Online/Android/iPhone for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-and-the-evolution-of-romantic-encounters/"><u>ChatGPT and the Evolution of Romantic Encounters</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-makeover-building-with-your-own-insights/"><u>ChatGPT Makeover: Building with Your Own Insights</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-transforms-officedoc-space-for-optimal-performance/"><u>ChatGPT Transforms OfficeDoc Space for Optimal Performance</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-the-key-to-seamless-workflow-management/"><u>ChatGPT: The Key to Seamless Workflow Management</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpts-culinary-classroom-for-healthy-eating/"><u>ChatGPT's Culinary Classroom for Healthy Eating</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/concealing-your-digital-chatter-with-gpt/"><u>Concealing Your Digital Chatter with GPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/conversational-cinema-choices-mastering-chatgpts-skills/"><u>Conversational Cinema Choices: Mastering ChatGPT's Skills</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/conversing-cars-into-customization-masterpieces-via-chatgpt/"><u>Conversing Cars Into Customization Masterpieces via ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/cyber-threats-on-rise-hackers-pursuit-of-ai-conversations/"><u>Cyber Threats on Rise: Hackers' Pursuit of AI Conversations</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/demystifying-the-ban-gptbots-role-in-ai-driven-creativity/"><u>Demystifying the Ban: GPTBot’s Role in AI-Driven Creativity</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/examining-the-cybersecurity-of-chatbot-technology/"><u>Examining the Cybersecurity of Chatbot Technology</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/explore-chatgpts-best-for-document-insights/"><u>Explore ChatGPT's Best for Document Insights</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/explore-uncharted-gpt-territories-5-features-to-enhance-dialogue/"><u>Explore Uncharted GPT Territories: 5 Features to Enhance Dialogue</u></a></li>
<li><a href="https://extra-resources.techidaily.com/exquisite-photographic-saga-assembler/"><u>Exquisite Photographic Saga Assembler</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/false-chatgpt-addon-subverts-facebook-logons/"><u>False ChatGPT Addon: Subverts Facebook Logons</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/from-dataset-to-dialogue-building-a-unique-bot/"><u>From Dataset to Dialogue: Building a Unique Bot</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/from-ideas-to-reality-chatgpts-role-in-sound-synthesis/"><u>From Ideas to Reality: ChatGPT's Role in Sound Synthesis</u></a></li>
<li><a href="https://remote-screen-capture.techidaily.com/in-2024-efficient-whiteboard-use-in-webinars-apple-android-and-pc-solutions-explored/"><u>In 2024, Efficient Whiteboard Use in Webinars  Apple, Android & PC Solutions Explored</u></a></li>
<li><a href="https://ai-video-translation.techidaily.com/in-2024-how-to-convert-video-voice-to-text-online-for-free/"><u>In 2024, How To Convert Video Voice to Text Online for Free?</u></a></li>
<li><a href="https://apple-account.techidaily.com/in-2024-how-to-delete-icloud-account-from-iphone-7-plus-without-password-by-drfone-ios/"><u>In 2024, How to Delete iCloud Account From iPhone 7 Plus without Password?</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/in-2024-how-to-screen-mirroring-motorola-razr-40-ultra-to-pc-drfone-by-drfone-android/"><u>In 2024, How to Screen Mirroring Motorola Razr 40 Ultra to PC? | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/innovating-audio-artistry-using-chatgpt-in-digital-production/"><u>Innovating Audio Artistry: Using ChatGPT in Digital Production</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/innovative-poetry-writing-via-ai-the-chatgpt-approach/"><u>Innovative Poetry Writing via AI: The ChatGPT Approach</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/innovative-solutions-at-your-fingertips-androidiphones-best-ai-apps/"><u>Innovative Solutions at Your Fingertips: Android/iPhone's Best AI Apps</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/is-openai-outmaneuvered-by-gpt/"><u>Is OpenAI Outmaneuvered by GPT?</u></a></li>
<li><a href="https://extra-approaches.techidaily.com/live-action-top-9-gaming-portals-for-2024/"><u>Live Action  Top 9 Gaming Portals for 2024</u></a></li>
<li><a href="https://tech-hub.techidaily.com/new-era-microsofts-ai-on-bing-search/"><u>New Era: Microsoft's AI on Bing Search</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/optimizing-data-management-with-gpt-in-google-docs/"><u>Optimizing Data Management with GPT in Google Docs</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/should-you-trust-ai-like-chatgpt-and-bard-for-financial-advice/"><u>Should You Trust AI Like ChatGPT and Bard for Financial Advice?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/synergy-of-gpt-and-cryptocurrency-discussions/"><u>Synergy of GPT and Cryptocurrency Discussions</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/takeoff-triumphs-comparing-copilots-foundations/"><u>Takeoff Triumphs: Comparing CoPilot's Foundations</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-developers-path-to-dynamic-web-with-gpt/"><u>The Developer's Path to Dynamic Web with GPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-smart-analysts-guide-to-ai-driven-insights/"><u>The Smart Analyst’s Guide to AI-Driven Insights</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/third-party-chatgpt-tools-safe-or-riskier/"><u>Third-Party ChatGPT Tools: Safe or Riskier?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/triple-pathways-to-augmenting-chatgpt-with-wolframalpha/"><u>Triple Pathways to Augmenting ChatGPT with WolframAlpha</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ubuntu-bash-scripts-to-converse-with-chatgpt/"><u>Ubuntu Bash Scripts to Converse with ChatGPT</u></a></li>
<li><a href="https://fox-friendly.techidaily.com/vive-headset-revolutionizes-virtual-reality-playtime-for-2024/"><u>Vive Headset Revolutionizes Virtual Reality Playtime for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/who-will-triumph-googles-bard-vs-microsofts-bing-chat/"><u>Who Will Triumph? Google's Bard Vs. Microsoft's Bing Chat</u></a></li>
</ul></div>
