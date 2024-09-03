---
title: "From Source to System: Your Auto-GPT Walkthrough"
date: 2024-09-02T20:38:17.793Z
updated: 2024-09-03T20:38:17.793Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes From Source to System: Your Auto-GPT Walkthrough"
excerpt: "This Article Describes From Source to System: Your Auto-GPT Walkthrough"
thumbnail: https://thmb.techidaily.com/c6867ae9c4f4e3df3c9379b15f4163ebd35319a50b7aab7a2fe4029be64b0298.jpg
---

## From Source to System: Your Auto-GPT Walkthrough

 With the explosion of ChatGPT, many people were impressed by the power and utility of OpenAI's GPT technology. This sparked the idea of making an automatic ChatGPT that answers and generates its prompts to achieve a specific goal, an idea that evolved into Auto-GPT.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 Since Auto-GPT is still under development, you'll only be able to access Auto-GPT just how a developer would—which may require a bit of technical know-how.

 To make things easier for you, here is a step-by-step guide on how to download and install Auto-GPT.

## Step 1: Download Python and AutoGPT

 Despite what you may have read elsewhere, installing Auto-GPT is pretty straightforward.

 Let's begin by manually downloading the latest version of Python 3 and the Auto-GPT executable from GitHub. You'll first want to download and install Python 3 since your PC will need it to read and execute files within Auto-GPT.

**Download:** [Python 3](https://www.python.org/downloads/) (Free)

 Once downloaded, double-click on the file to install Python. Make sure to tick the box for **Add python.exe to PATH**. This will enable your PC to use Python anywhere in your PC. After that, go ahead and click **Install Now**.

![A tab showing a tab to install Python](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/2-install-python.jpg)

 After Installing Python, you can download Auto-GPT from GitHub.

**Download**: [Auto-GPT](https://github.com/Significant-Gravitas/Auto-GPT/releases/tag/v0.4.7) (Free)

**Source code.zip** is for Windows, while **Source code.tar.gz** is for Linux and MacOS. First, download the file for your operating system, then copy the folder and paste it into your desired location.

## Step 2: Configure Auto-GPT

 Since AutoGPT uses OpenAI's GPT model, you must generate an API key from OpenAI to act as your credential to use their product.

 Keep in mind that your account on ChatGPT is different from an OpenAI account. You must [register for an OpenAI account](https://openai.com/blog/openai-api) to access an OpenAI API. Now:

1. After registration and login, click on **Personal** in the top right corner of the website and select **View API keys**. This will send you to the [OpenAI API keys management](https://platform.openai.com/account/api-keys), where you can manage your API keys.
2. To create a key, click **Create new secret key**, input a name, then click **Create secret key**. You can then copy the API key by using **CTRL + C** or clicking the copy icon on the right.  
![Create API key](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/7-create-test-key.jpg)
3. Now you have your API key, go to your Auto-GPT folder and open the **.env** file using Notepad.  
![Open env with Notepad](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/6-open-env.jpg)
4. Once opened, scroll down to the **LLM PROVIDER** section. There you will see OPENAI\_API\_KEY. Replace the placeholder with the API key you've just copied, then save the file.  
![Set API as environment variable](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/08/wrwe.jpg)

 This file is where all your service credentials are placed, so if you want to use a [backend vector database to boost AI](https://www.makeuseof.com/what-is-a-vector-database/), you can set your product API keys here. But if you only want to use AutoGPT, the OpenAI API key should be enough.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4620780&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/07dd4d5a72f5740ef0f035f201951476/728__90banner.jpg" border="0"></a>
<!-- affiliate ads end -->
## Step 3: Install Auto-GPT Dependencies

 Now that you have configured Auto-GPT, it's time to install its dependencies through a terminal.

1. To open a terminal in the Auto-GPT environment, right-click on the Auto-GPT folder, then select **Open in Terminal**.
2. To install all the requirements needed for Auto-GPT to work, use the command:  
pip install -r requirements.txt
3. Once you press enter, your terminal will download and install all the required dependencies.  
![Pip install requirements](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/08/3-4.jpg)
4. After installation, try opening Auto-GPT using:  
<!-- affiliate ads begin -->
<a href="https://laganoo.pxf.io/c/5597632/1657397/16446" target="_top" id="1657397"><img src="//a.impactradius-go.com/display-ad/16446-1657397" border="0" alt="" width="336" height="280"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1657397/16446" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
python -m autogpt  
![AutoGPT installation success](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/08/4-4.jpg)

 Congratulations! You have successfully Installed Auto-GPT.

<!-- affiliate ads begin -->
<a href="https://store.nero.com/order/checkout.php?PRODS=42296740&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.nero.com/nero-com-wAssets/img/banners/2023/biu/Nero_BackItUp_Screen_2.webp" border="0"></a>
<!-- affiliate ads end -->
## How to Use Auto-GPT

 Now that you have successfully installed Auto-GPT on your computer let's discuss how to use Auto-GPT.

 When you first open Auto-GPT, you'll be given two options: Manual or Automatic mode. Automatic mode is the default mode where you'll only need to input what you want to be achieved. In this mode, AutoGPT will automatically assign the name of your AI assistant, its role, and its goals. Use this mode if you're not particularly knowledgeable about the process of achieving your goal.

 But if you are knowledgeable, we suggest you use the Manual mode. This ensures that your goals are properly detailed, which makes the output more likely to mirror your expectations. To activate this mode, use the command:

--manual

 After setting AutoGPT on Manual mode, it will ask you to name your AI assistant, then assign its role and five goals the AI should follow.

 You can input any name you want. It doesn't affect Auto-GPT performance (as far as we know). After giving a name, try providing a clear and concise role, as this will set the AI's role.

 Although you don't need to fill all five goals, it is still recommended that you do, as this will likely affect the efficiency of your AI.

![Creating Recipe-Generator](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/recipe-generator.jpg)

 In this example, we have named our AI assistant "Recipe-Generator." Its role is to make a recipe based on the top five ingredients readily available in the US. We've set the first three goals as parameters on what we expect the recipe will be and set the last two to tell Auto-GPT to save the file as TXT, then shutdown.

![Running Recipe-Generator](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/2-recipe-generator-thinking.jpg)

<!-- affiliate ads begin -->
<a href="https://newchic.sjv.io/c/5597632/1659704/14420" target="_top" id="1659704"><img src="//a.impactradius-go.com/display-ad/14420-1659704" border="0" alt="" width="728" height="90"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1659704/14420" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 Once you give your last goal, you can hit enter for Auto-GPT to run.

 While running, you can see the AI's thoughts, reasoning, plan, and criticism. For every action of the AI assistant, you will be asked to authorize its plan to execute. You can do so by typing "y" as yes.

 If you want the AI to continue a number of times without asking you for authorization, you can type "y -(number actions authorized)." For example, if you want your AI assistant to continue executing the following five steps, you can type "y -5" and hit enter.

 One advantage of Auto-GPT over ChatGPT is that it is free to probe through the internet. As you can see here, our Recipe-Generator assistant downloads a file.

![AutoGPT downloading file](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/3-recipe-generator.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=38729081&QTY=1&AFFILIATE=108875&CART=1"><img src="https://website-prod.cache.wpscdn.com/img/wps-spreadsheet-free-excel-editor-online-offline-1x.93e269d.png" border="0">
WPS Office Premium ( File Recovery, Photo Scanning, Convert PDF)--Yearly</a>
<!-- affiliate ads end -->
 This makes this [AI potentially dangerous](https://www.makeuseof.com/what-is-ai-what-dangers-does-artificial-intelligence-pose/); that's why Auto-GPT always asks you for authorization before executing plans. Always read and understand your AI assistant's thoughts, reasoning, and plan before authorizing its actions.

 After every action of the AI, you can also provide your feedback to help the AI with its task.

![Providing human input](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/4-recipe-generator-human-interaction.jpg)

 In this screenshot, our AI assistant has looped through the same step three times. So, we tell the AI to skip browsing for recipes and start creating the output.

 After making the recipe, our AI has now completed its task.

![Shutting down Auto-GPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/08/6-1.jpg)

 To view the output, go to your Auto-GPT folder and **open auto-gpt-workspace**.

![Viewing-AutoGPT-Output](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/08/7-1.jpg)

 Success! Our AI assistant has given us a recipe for a chicken pot pie casserole.

## Auto-GPT Limitations

 Although Auto-GPT's automation works, it's still quite limited. Through a series of testing, we discovered that Auto-GPT couldn't handle anything complex. Most of the time, it continued looping around the same thought and reasoning. Although you can keep providing helpful prompts, it feels more like ChatGPT stuck in a loop instead of the autonomous assistant it is meant to be.

 Many of these loopings are caused by an endless cycle of generating prompts for a problem, querying the internet about the problem, identifying what is true from false, then trying to solve the problem with the information gathered.

 The problem with Generative Pre-trained Models is that they are expected to hallucinate occasionally ([AI hallucination refers to an AI tool outputting false information](https://www.makeuseof.com/what-is-ai-hallucination-and-how-do-you-spot-it/) but presenting it as fact). If the GPT model hallucinates, Auto-GPT will likely continue looping as it looks to solve problems generated from false info. The more complex the problem is, the more likely that Auto-GPT and similar programs will get stuck in this loop.

 Other problems that contribute to Auto-GPT getting stuck are the model struggling to handle or navigate website advertising and cookies, login pages, and all kinds of pop-ups (the stuff humans hate, too!).

 Using GPT-4 will noticeably reduce hallucinations and improve overall performance. However, its context size is still limited to 8,000 tokens. After reaching the 8k-token mark, GPT-4 will start losing context starting from the beginning of the task, affecting results. Furthermore, using GPT-4 is several times pricier than GPT-3.5 ([each GPT token has a cost](https://www.makeuseof.com/what-is-chatgpt-token-limit-can-you-exceed-it/)). You'll want to set limits through your API account.

<!-- affiliate ads begin -->
<a href="https://versadesk.pxf.io/c/5597632/1892108/21290" target="_top" id="1892108"><img src="//a.impactradius-go.com/display-ad/21290-1892108" border="0" alt="" width="1080" height="1080"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1892108/21290" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## The Future of Auto-GPT

 Ever since the start of August 2023, the Auto-GPT GitHub project has continuously gained support gaining over 140,000 GitHub Starts. Developments and updates don't seem to be slowing down. Future developments are expected to provide more functionalities, bug fixes, and improved stability in conjunction with the release of GPT-4 and its 32K model.

 With that said, Auto-GPT is still in its early development stage, and GPT-4 is still on its 8k model. As for now, Auto-GPT should not be used as a tool for any professional or business applications. Anyone using it should only be for the purpose of learning and experimentation.

**SCROLL TO CONTINUE WITH CONTENT**

 Since Auto-GPT is still under development, you'll only be able to access Auto-GPT just how a developer would—which may require a bit of technical know-how.

 To make things easier for you, here is a step-by-step guide on how to download and install Auto-GPT.

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
<li><a href="https://tiktok-videos.techidaily.com/new-2024-approved-master-the-art-of-rapid-tiktok-videos/"><u>[New] 2024 Approved  Master the Art of Rapid TikTok Videos</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/new-excellent-20-anime-opening-anthems/"><u>[New] Excellent 20 Anime Opening Anthems</u></a></li>
<li><a href="https://on-screen-recording.techidaily.com/new-in-2024-premier-6-modern-architecture-in-mc-world/"><u>[New] In 2024, Premier 6 Modern Architecture in MC World</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/updated-2024-approved-alternative-cinema-highlights-audiences/"><u>[Updated] 2024 Approved  Alternative Cinema Highlights Audiences</u></a></li>
<li><a href="https://youtube-lab.techidaily.com/ed-affordable-acoustic-amps-and-mics-for-video-voyagers/"><u>[Updated] Affordable Acoustic Amps and Mics for Video Voyagers</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/updated-balance-aesthetics-and-functionality-on-instagram/"><u>[Updated] Balance Aesthetics and Functionality on Instagram</u></a></li>
<li><a href="https://facebook-video-footage.techidaily.com/updated-youtube-snippet-income-breakdown-whats-your-profit-share/"><u>[Updated] YouTube Snippet Income Breakdown  What's Your Profit Share?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1-essential-lessons-from-my-journey-top-8-technological-blunders-for-newbies-and-their-solutions/"><u>1. Essential Lessons From My Journey: Top 8 Technological Blunders for Newbies & Their Solutions</u></a></li>
<li><a href="https://apple-account.techidaily.com/3-ways-of-how-to-get-someones-apple-id-off-apple-iphone-13-pro-max-without-password-by-drfone-ios/"><u>3 Ways of How to Get Someones Apple ID Off Apple iPhone 13 Pro Max without Password</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/affordable-boost-mobile-5g-plans-now-available/"><u>Affordable Boost Mobile 5G Plans Now Available</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/battle-of-the-titans-google-pixel-8-versus-samsung-galaxy-s24-a-new-era-for-miniature-flagships/"><u>Battle of the Titans: Google Pixel 8 Versus Samsung Galaxy S24 – A New Era for Miniature Flagships</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/boost-your-digital-safety-asap-with-these-9-speedy-cybersecurity-tips/"><u>Boost Your Digital Safety ASAP with These 9 Speedy Cybersecurity Tips!</u></a></li>
<li><a href="https://win-blog.techidaily.com/check-the-box-with-ease-microsoft-excels-latest-update-introduces-checkbox-functionality/"><u>Check the Box with Ease: Microsoft Excel's Latest Update Introduces Checkbox Functionality</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/discover-the-joy-of-melodic-brain-teasers-a-fresh-take-on-daily-song-quizzes/"><u>Discover the Joy of Melodic Brain Teasers - A Fresh Take on Daily Song Quizzes!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/discover-ways-to-determine-if-workplace-surveillance-is-tracking-your-digital-footprint/"><u>Discover Ways To Determine If Workplace Surveillance Is Tracking Your Digital Footprint!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/easily-create-individual-browser-windows-instead-of-tabs-on-your-androids-chrome-app/"><u>Easily Create Individual Browser Windows Instead of Tabs on Your Android's Chrome App</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/easy-ways-to-send-documents-through-fax-on-your-smartphone/"><u>Easy Ways to Send Documents Through Fax on Your Smartphone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/effective-techniques-for-managing-and-maximizing-remaining-space-on-your-iphone/"><u>Effective Techniques for Managing and Maximizing Remaining Space on Your iPhone</u></a></li>
<li><a href="https://extra-resources.techidaily.com/elevating-podcast-reputation-logo-design-principles/"><u>Elevating Podcast Reputation  Logo Design Principles</u></a></li>
<li><a href="https://buynow-tips.techidaily.com/ensuring-quality-streams-finding-the-best-spot-for-your-ps4-camera/"><u>Ensuring Quality Streams: Finding the Best Spot for Your PS4 Camera</u></a></li>
<li><a href="https://article-helps.techidaily.com/exploring-microsofts-hololens-a-hologram-horizon-for-2024/"><u>Exploring Microsoft's HoloLens  A Hologram Horizon for 2024</u></a></li>
<li><a href="https://screen-video-capture.techidaily.com/gamings-finest-bike-battles-compiled/"><u>Gaming's Finest Bike Battles Compiled</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-i-mastered-the-vintage-method-for-seamless-file-transfers-at-53-years-old/"><u>How I Mastered the Vintage Method for Seamless File Transfers at 53 Years Old</u></a></li>
<li><a href="https://android-location-track.techidaily.com/in-2024-9-best-phone-monitoring-apps-for-oneplus-nord-3-5g-drfone-by-drfone-virtual-android/"><u>In 2024, 9 Best Phone Monitoring Apps for OnePlus Nord 3 5G | Dr.fone</u></a></li>
<li><a href="https://activate-lock.techidaily.com/in-2024-top-7-icloud-activation-bypass-tools-for-your-apple-iphone-8-plus-by-drfone-ios/"><u>In 2024, Top 7 iCloud Activation Bypass Tools For your Apple iPhone 8 Plus</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/is-the-galaxy-s24-ultra-maintaining-its-throne-as-the-top-android-device-after-half-a-year/"><u>Is the Galaxy S24 Ultra Maintaining Its Throne as the Top Android Device After Half a Year?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/maximizing-efficiency-with-mobile-tech-discover-8-essential-lessons-from-turning-your-phone-into-a-laptop-alternative/"><u>Maximizing Efficiency with Mobile Tech: Discover 8 Essential Lessons From Turning Your Phone Into a Laptop Alternative</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/quickly-categorize-your-memories-with-google-photos-collections-feature/"><u>Quickly Categorize Your Memories with Google Photos Collections Feature</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/reassessing-googles-strategy-the-importance-of-concentration-over-the-expansion-of-ai-initiatives/"><u>Reassessing Google's Strategy: The Importance of Concentration over the Expansion of AI Initiatives</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revive-your-sonos-speakers-a-guide-on-fixing-common-problems-with-an-outdated-third-party-application/"><u>Revive Your Sonos Speakers: A Guide on Fixing Common Problems with an Outdated Third-Party Application</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/riding-the-wave-of-progress-the-ongoing-expansion-of-t-mobiles-high-speed-internet-network/"><u>Riding the Wave of Progress: The Ongoing Expansion of T-Mobile's High-Speed Internet Network</u></a></li>
<li><a href="https://printer-issues.techidaily.com/sleeper-mode-dilemma-usb-printers-not-awakening-in-w7/"><u>Sleeper Mode Dilemma: USB Printers Not Awakening in W7</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/step-by-step-guide-verifying-java-installation-in-windows-11/"><u>Step-by-Step Guide: Verifying Java Installation in Windows 11</u></a></li>
<li><a href="https://hardware-updates.techidaily.com/the-ultimate-source-for-cutting-edge-pc-components-at-toms-site/"><u>The Ultimate Source for Cutting-Edge PC Components at Tom's Site</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/troubleshoot-and-solve-your-windows-security-connection-problems-tips-for-restoring-internet-access/"><u>Troubleshoot & Solve Your Windows Security Connection Problems – Tips for Restoring Internet Access</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ultimate-guide-to-utilizing-pushd-and-popd-in-your-linux-terminal/"><u>Ultimate Guide to Utilizing Pushd and Popd in Your Linux Terminal</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/understanding-and-activating-smart-app-control-in-windows-11-an-essential-tutorial/"><u>Understanding & Activating Smart App Control in Windows 11 - An Essential Tutorial</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/understanding-the-impact-how-does-ios-18-revolutionize-your-mobile-experience/"><u>Understanding the Impact: How Does iOS 18 Revolutionize Your Mobile Experience?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unleash-new-features-introducing-powertoys-v079s-customizable-keyboard-shortcuts-for-enhanced-windows-control/"><u>Unleash New Features: Introducing PowerToys V0.79's Customizable Keyboard Shortcuts for Enhanced Windows Control</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unlock-the-full-potential-the-best-10-uses-of-your-google-tv/"><u>Unlock the Full Potential: The Best 10 Uses of Your Google TV</u></a></li>
<li><a href="https://instagram-clips.techidaily.com/unlocking-igtvs-potential-secrets-to-attract-more-subscribers/"><u>Unlocking IGTV's Potential  Secrets to Attract More Subscribers</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-the-mystery-behind-googles-covert-project-the-emergence-of-fuchsia-os/"><u>Unveiling the Mystery Behind Google's Covert Project - The Emergence of Fuchsia OS</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/vintage-cellphones-the-perfect-kid-friendly-devices-for-listening-to-tunes-and-educational-talks/"><u>Vintage Cellphones: The Perfect Kid-Friendly Devices for Listening to Tunes & Educational Talks</u></a></li>
</ul></div>
