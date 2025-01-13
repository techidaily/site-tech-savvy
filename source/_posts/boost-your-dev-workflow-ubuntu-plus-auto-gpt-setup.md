---
title: "Boost Your Dev Workflow: Ubuntu + Auto-GPT Setup"
date: 2025-01-11T21:36:10.390Z
updated: 2025-01-12T18:24:09.916Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Boost Your Dev Workflow: Ubuntu + Auto-GPT Setup"
excerpt: "This Article Describes Boost Your Dev Workflow: Ubuntu + Auto-GPT Setup"
thumbnail: https://thmb.techidaily.com/24d9ad97cc4d2914a6f62f8ac9d6325300e284842ea91d53be138fc17a246961.jpg
---

## Boost Your Dev Workflow: Ubuntu + Auto-GPT Setup

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
<iframe width="560" height="315" src="https://www.youtube.com/embed/58KlTPHv8dU?si=7ICagyNgrao7OkVO" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Once copied, paste the key inside the **.env** file. The env file will store all the API keys that you use with Auto-GPT. If you don't need a backend vector database like Pinecone, your OpenAI API key should be enough to use Auto-GPT.

 To set your API key, open the **.env** file using nano:

`nano .env.template`

 To locate the OpenAI API key variable, hold **CTRL + W**, search for “**OPEN\_API\_KEY=**”, and then hit **Enter**.

![Insert API key](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/paste-api-key.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/KKFdFHaVIJg?si=x2vLw7ty3FtHX-9T" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Replace the placeholder with your API key by pressing **Ctrl +V** and hitting **Ctrl + S** to save. You can exit the nano text editor by pressing **Ctrl + X**.

 You must also rename the "**.env.template**" file to only "**.env**". To do so, run:

`sudo mv .env.template .env`

## Step 2: Install Auto-GPT Dependencies on Ubuntu

 Auto-GPT uses a lot of Python libraries. You will need to install all the packages using pip and the **requirements.txt** text file that comes with the AutoGPT source code.

 To install all the Python dependencies, run:

`pip install -r requirements.txt`

![Install Auto-GPT requirements](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/5-install-requirements.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/3C51hzX46eY?si=o5qiDSkT7mXUGm3F" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Next, try running Auto-GPT using:

`python3 -m autogpt`

![Successful Auto-GPT installation](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/6-success.jpg)

 Congratulations! You have successfully installed and set up Auto-GPT on your Ubuntu machine.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/Xa2_mFu-obA?si=_xDGF1pv-dnuaDOr" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## How to Use Auto-GPT on Ubuntu

 With Auto-GPT installed, you can now make your own AI assistant. There are two modes when it comes to using Auto-GPT. In the default mode, you only need to provide a task. Based on the specified task, Auto-GPT will automatically generate your AI assistant's name, its role, and its goals.

![Auto-GPT auto mode](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/1-auto.jpg)

 In manual mode, Auto-GPT will ask you to specify a name, a goal, and up to five goals you want the AI assistant to follow while doing its task. This mode allows you to be in control of how your AI assistant will function.

 To use manual mode, use the following command:

`--manual`

 In this example, we've named our AI assistant, and given it a role to look for product promos, and a few goals on the quality of the promo.

![Auto-GPT manual mode](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/1-manual.jpg)

 Once the name, goals, and role have been provided, your AI assistant will immediately activate and start looping through its thinking and execution process.

 Throughout the process, you can view your AI assistant's thoughts, reasoning, plan, criticism, and next action. Its next action will only be executed once you've given your approval.

![Input-Commands for Auto-GPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/2-input-y.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/pGHmqD53gc8?si=ymgHIB6Aa7_MoUUf" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://facebook-record-videos.techidaily.com/new-2024-approved-crafting-universal-streams-for-youtube-and-beyond-networks/"><u>[New] 2024 Approved Crafting Universal Streams for YouTube & Beyond Networks</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/updated-innovative-vertical-video-editing-for-instagrams-igtv-for-2024/"><u>[Updated] Innovative Vertical Video Editing for Instagram's IGTV for 2024</u></a></li>
<li><a href="https://some-approaches.techidaily.com/updated-unraveling-lightrooms-potential-on-android-devices/"><u>[Updated] Unraveling Lightroom's Potential on Android Devices</u></a></li>
<li><a href="https://games-able.techidaily.com/4-reasons-why-you-shouldnt-buy-a-ps5/"><u>4 Reasons Why You Shouldn't Buy a PS5</u></a></li>
<li><a href="https://fox-that.techidaily.com/adjust-inaccurate-person-tags-in-your-apple-photos-with-these-simple-tips/"><u>Adjust Inaccurate Person Tags in Your Apple Photos with These Simple Tips</u></a></li>
<li><a href="https://unlock-android.techidaily.com/can-i-bypass-a-forgotten-phone-password-of-tecno-pova-5-by-drfone-android/"><u>Can I Bypass a Forgotten Phone Password Of Tecno Pova 5?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatbot-conversation-replication-techniques/"><u>Chatbot Conversation Replication Techniques</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/easing-the-capacity-load-of-wins-chatgpt/"><u>Easing the Capacity Load of Win's ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/exploring-ai-conversations-bots-that-captivate-users/"><u>Exploring AI Conversations: Bots that Captivate Users</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/exploring-the-differences-auto-gpt-versus-chatgpt/"><u>Exploring the Differences: Auto-GPT Versus ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-apples-ios-175-brought-back-lost-memories-understanding-the-technology-behind-recovered-images-and-next-steps-for-users/"><u>How Apple's iOS 17.5 Brought Back Lost Memories: Understanding the Technology Behind Recovered Images & Next Steps for Users</u></a></li>
<li><a href="https://fox-http.techidaily.com/in-2024-leading-online-tools-select-your-new-photo-background/"><u>In 2024, Leading Online Tools Select Your New Photo Background</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/in-2024-wondering-the-best-alternative-to-hola-on-lava-blaze-pro-5g-here-is-the-answer-drfone-by-drfone-virtual-android/"><u>In 2024, Wondering the Best Alternative to Hola On Lava Blaze Pro 5G? Here Is the Answer | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mitigating-data-disappearance-in-ai-talks/"><u>Mitigating Data Disappearance in AI Talks</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/slow-and-steady-why-does-chatgpt-4-pace-slower/"><u>Slow and Steady: Why Does ChatGPT-4 Pace Slower?</u></a></li>
<li><a href="https://tech-revival.techidaily.com/unleashing-creativity-in-gaming-6-methods-for-using-chatgpt-as-your-co-writer/"><u>Unleashing Creativity in Gaming: 6 Methods for Using ChatGPT as Your Co-Writer</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/upgrade-to-the-new-era-comparing-features-between-iphone-16-and-15-is-it-time-gadgetguru/"><u>Upgrade to the New Era: Comparing Features Between iPhone 16 and 15 - Is It Time? | GadgetGuru</u></a></li>
</ul></div>

