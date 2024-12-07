---
title: "Setting Up Smart Tech: Auto-GPT Installation Guide"
date: 2024-12-02T22:05:05.836Z
updated: 2024-12-06T22:29:08.627Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Setting Up Smart Tech: Auto-GPT Installation Guide"
excerpt: "This Article Describes Setting Up Smart Tech: Auto-GPT Installation Guide"
thumbnail: https://thmb.techidaily.com/a8a502e12209ca4cf0a910d9af6975208a0b7497dd6ac900e046b6637a6b7e0e.jpg
---

## Setting Up Smart Tech: Auto-GPT Installation Guide

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

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/kZVDkvMZvP4?si=xAugrCf-Ud6EMMpm" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Replace the placeholder with your API key by pressing **Ctrl +V** and hitting **Ctrl + S** to save. You can exit the nano text editor by pressing **Ctrl + X**.

 You must also rename the "**.env.template**" file to only "**.env**". To do so, run:

`sudo mv .env.template .env`

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/xtylXDY9YfA?si=VonzSiDFGCpJm2uC" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/_dOmuXhsV6Y?si=aT6vgPbDx4ajjvdr" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## How to Use Auto-GPT on Ubuntu

 With Auto-GPT installed, you can now make your own AI assistant. There are two modes when it comes to using Auto-GPT. In the default mode, you only need to provide a task. Based on the specified task, Auto-GPT will automatically generate your AI assistant's name, its role, and its goals.

![Auto-GPT auto mode](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/1-auto.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/JNxZ4Z6BVCg?si=522oz1OPSQDhNYWT" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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

 Once your AI assistant finishes its task, you can view its final output by opening the **/Auto-GPT-x.x.x/autogpt/auto\_gpt\_workspace** directory.

![Successful Auto-GPT session](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/success-1.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/5OmJZ4Z8jgk?si=YIoEaPI8geoiFSYE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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
<li><a href="https://fox-helps.techidaily.com/new-viral-visionaries-top-ten-meme-templates-exposed/"><u>[New] Viral Visionaries Top Ten Meme Templates Exposed</u></a></li>
<li><a href="https://article-knowledge.techidaily.com/2024-approved-avoiding-grainy-zoom-videos-techniques-included/"><u>2024 Approved Avoiding Grainy Zoom Videos – Techniques Included</u></a></li>
<li><a href="https://screen-capture.techidaily.com/2024-approved-crop-companion-chronicles-best-agricultural-titles-with-pals/"><u>2024 Approved Crop Companion Chronicles Best Agricultural Titles with Pals</u></a></li>
<li><a href="https://discover-brilliant.techidaily.com/buy-your-winx-ipad-converter-bundle-at-a-discounted-price-shop-now/"><u>Buy Your WinX iPad Converter Bundle at a Discounted Price - Shop Now!</u></a></li>
<li><a href="https://win-blog.techidaily.com/easy-steps-to-make-excel-open-predefined-workbooks-upon-initialization/"><u>Easy Steps to Make Excel Open Predefined Workbooks Upon Initialization</u></a></li>
<li><a href="https://games-able.techidaily.com/embracing-the-future-of-healthcare-how-digitally-first-strategies-are-transforming-hospitals-into-smart-patient-centered-facilities/"><u>Embracing the Future of Healthcare: How Digitally-First Strategies Are Transforming Hospitals Into Smart, Patient-Centered Facilities</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ensuring-artificial-agents-align-with-human-ethos/"><u>Ensuring Artificial Agents Align with Human Ethos</u></a></li>
<li><a href="https://instagram-clips.techidaily.com/in-2024-be-the-life-of-the-party-uploading-and-sharing-gifs-on-instagram-instant-guide/"><u>In 2024, Be the Life of the Party Uploading & Sharing GIFs on Instagram [Instant Guide]</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ingenious-chatbot-creation-guided-by-gpt-principles/"><u>Ingenious Chatbot Creation: Guided by GPT Principles</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/navigate-the-world-of-apples-spatial-videos-in-virtual-reality-with-a-meta-quest-device-guidance/"><u>Navigate the World of Apple's Spatial Videos in Virtual Reality with a Meta Quest Device | Guidance</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/precision-modification-chatgpts-role-in-custom-cars/"><u>Precision Modification: ChatGPT's Role in Custom Cars</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revolutionizing-mobile-photography-how-iphone-16s-new-visual-intelligence-feature-mirrors-google-lens-capabilities-zdnet-explained/"><u>Revolutionizing Mobile Photography: How iPhone 16'S New Visual Intelligence Feature Mirrors Google Lens Capabilities - ZDNET Explained</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/step-by-step-to-integrating-chatgpt-widget/"><u>Step-by-Step to Integrating ChatGPT Widget</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/understanding-and-remedying-four-account-blocks/"><u>Understanding and Remedying Four Account Blocks</u></a></li>
<li><a href="https://ai-video-apps.techidaily.com/updated-2024-approved-how-to-reduce-the-size-of-video-file-online-in-this-article-well-share-top-10-free-online-video-compressors-that-you-can-use-anywhere-/"><u>Updated 2024 Approved How to Reduce the Size of Video File Online? In This Article, Well Share Top 10 Free Online Video Compressors that You Can Use Anywhere at Any Time and on Any Device</u></a></li>
<li><a href="https://smart-video-creator.techidaily.com/updated-transform-your-videos-easy-editing-with-microsoft-video-editor-on-windows/"><u>Updated Transform Your Videos Easy Editing with Microsoft Video Editor on Windows</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/whats-new-in-carplay-explore-the-exciting-upgrades-from-apples-wwdc-2024-keynote-gizmodo/"><u>What's New in CarPlay - Explore the Exciting Upgrades From Apple's WWDC 2024 Keynote | Gizmodo</u></a></li>
</ul></div>

