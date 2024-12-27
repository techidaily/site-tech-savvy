---
title: Harness the Power of AI in Ubuntu with Auto-GPT
date: 2024-12-23T18:08:59.750Z
updated: 2024-12-27T19:03:21.619Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Harness the Power of AI in Ubuntu with Auto-GPT
excerpt: This Article Describes Harness the Power of AI in Ubuntu with Auto-GPT
thumbnail: https://thmb.techidaily.com/0de78e74e4231d077c0bbd1093422fc13ce8314c6f52350885d9fed67ecbab12.jpg
---

## Harness the Power of AI in Ubuntu with Auto-GPT

 Auto-GPT is an open-source project that allows people to create AI assistants that cater to their needs. These AI assistants are capable of thought and self-criticism and can generate their own prompts to reach a particular set of goals and accomplish their role. It uses the same GPT language model used in the already popular ChatGPT.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 If you would like to harness the power of GPT in the form of an AI assistant, it might interest you to try out Auto-GPT. Here's how you can install and set up Auto-GPT on Ubuntu.

>  Disclaimer: This post includes affiliate links
>
>  If you click on a link and make a purchase, I may receive a commission at no extra cost to you.
>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/DxUX4R6Cf7c?si=prHevNQJivSkIfUt" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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
<iframe width="560" height="315" src="https://www.youtube.com/embed/15TKQ-BOENI?si=Ri4B2AuxAdi0Bglz" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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

## Step 2: Install Auto-GPT Dependencies on Ubuntu

 Auto-GPT uses a lot of Python libraries. You will need to install all the packages using pip and the **requirements.txt** text file that comes with the AutoGPT source code.

 To install all the Python dependencies, run:

`pip install -r requirements.txt`

![Install Auto-GPT requirements](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/5-install-requirements.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/XA_wP7rS9ww?si=LarMG3sEHAhSoL6q" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Next, try running Auto-GPT using:

`python3 -m autogpt`

![Successful Auto-GPT installation](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/6-success.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/7JBG_O3Vnh4?si=lUO0fta6YPJ50qjg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Congratulations! You have successfully installed and set up Auto-GPT on your Ubuntu machine.

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

 You can approve the AI's next action by typing "**y**" for yes. If you don't want the AI to continue with its plans, you can type "**n**" for no and exit.

 If you trust your AI assistant and don't want to continue monitoring all of its thoughts and actions, you can type "**y -(number)**". For example, if you want Auto-GPT to execute its next five actions, you can type "**y -5**". Furthermore, if you want to provide feedback to your AI assistant, you can also type your prompt as input.

 In this example, our assistant has been looping around the same thoughts, plans, and executions three times now. So we decided to give it feedback to stop as its initial efforts were already enough.

![Providing human feedback to Auto-GPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/3-human-feedback.jpg)

 Once your AI assistant finishes its task, you can view its final output by opening the **/Auto-GPT-x.x.x/autogpt/auto\_gpt\_workspace** directory.

![Successful Auto-GPT session](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/success-1.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/3C51hzX46eY?si=o5qiDSkT7mXUGm3F" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://tech-recovery.techidaily.com/1722873499752-current-month-find-your-dream-apple-watch-at-unbelievable-discounts/"><u>[Current Month]: Find Your Dream Apple Watch at Unbelievable Discounts!</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/new-ideal-hosts-maximizing-youtube-video-exposure/"><u>[New] Ideal Hosts Maximizing YouTube Video Exposure</u></a></li>
<li><a href="https://digital-screen-recording.techidaily.com/new-in-2024-simultaneous-video-documentation/"><u>[New] In 2024, Simultaneous Video Documentation</u></a></li>
<li><a href="https://facebook-video-share.techidaily.com/new-learn-how-to-build-youtube-backlinks-for-your-channel/"><u>[New] Learn How to Build YouTube Backlinks for Your Channel</u></a></li>
<li><a href="https://fox-links.techidaily.com/new-m1-masterpiece-flawless-video-edits-just-a-click-away-for-2024/"><u>[New] M1 Masterpiece Flawless Video Edits, Just a Click Away for 2024</u></a></li>
<li><a href="https://some-approaches.techidaily.com/new-transform-your-podcast-with-these-google-upload-insights/"><u>[New] Transform Your Podcast with These Google Upload Insights</u></a></li>
<li><a href="https://youtube-tips.techidaily.com/ed-redefining-digital-space-alternative-video-hosting-sites-for-2024/"><u>[Updated] Redefining Digital Space Alternative Video Hosting Sites for 2024</u></a></li>
<li><a href="https://youtube-stream.techidaily.com/2024-approved-unlocking-trending-potential-in-your-videos/"><u>2024 Approved Unlocking Trending Potential in Your Videos</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ace-the-competition-mastering-secrets-of-getting-hired-as-a-remote-full-stack-developer-insights-from-zdnet/"><u>Ace the Competition: Mastering Secrets of Getting Hired as a Remote Full-Stack Developer - Insights From ZDNet</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/achieve-peak-productivity-by-adopting-programming-principles-in-daily-workflows-insights-from-zdnet/"><u>Achieve Peak Productivity by Adopting Programming Principles in Daily Workflows | Insights From ZDNet</u></a></li>
<li><a href="https://easy-unlock-android.techidaily.com/how-to-remove-forgotten-pin-of-your-oneplus-ace-2-by-drfone-android/"><u>How to Remove Forgotten PIN Of Your OnePlus Ace 2</u></a></li>
<li><a href="https://instagram-clips.techidaily.com/in-2024-expert-tips-for-efficient-instagram-to-mp4-transformation/"><u>In 2024, Expert Tips for Efficient Instagram to MP4 Transformation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/master-the-application-process-expert-tips-for-getting-hired-by-leading-tech-giants-based-on-zdnets-ultimate-guide/"><u>Master the Application Process: Expert Tips for Getting Hired by Leading Tech Giants, Based on ZDNet's Ultimate Guide</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/shifting-paths-essential-strategies-for-moving-from-hospitality-to-technology-careers-with-expert-insights/"><u>Shifting Paths: Essential Strategies for Moving From Hospitality to Technology Careers with Expert Insights</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/streamline-your-admin-duties-with-windows-powershell-for-just-16-discover-the-secrets-at-zdnet/"><u>Streamline Your Admin Duties with Windows PowerShell for Just $16 | Discover the Secrets at ZDNet</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/tech-innovation-craze-mainstream-companies-still-hunting-for-expertise/"><u>Tech Innovation Craze: Mainstream Companies Still Hunting for Expertise</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-unexpected-driving-forces-causing-most-employees-to-quit-what-experts-at-zdnet-discovered/"><u>The Unexpected Driving Forces Causing Most Employees to Quit: What Experts at ZDNet Discovered</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/thousands-tap-into-apples-latest-initiative-free-ai-education-for-students-and-graduates-discover-more-on-zdnet/"><u>Thousands Tap Into Apple's Latest Initiative: Free AI Education for Students & Graduates - Discover More on ZDNet</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/understanding-staffing-shifts-in-major-tech-companies-beyond-layoff-headlines/"><u>Understanding Staffing Shifts in Major Tech Companies: Beyond Layoff Headlines</u></a></li>
</ul></div>

