---
title: CodeGPT Setup Tutorial for VS Code Users
date: 2024-08-21T15:36:41.260Z
updated: 2024-08-22T15:36:41.260Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes CodeGPT Setup Tutorial for VS Code Users
excerpt: This Article Describes CodeGPT Setup Tutorial for VS Code Users
thumbnail: https://thmb.techidaily.com/4ba28a3dd24936be14c010b9b472cc28e6164f2ddc628c9763c3b8ea3ee12f42.png
---

## CodeGPT Setup Tutorial for VS Code Users

 VS Code has several useful extensions that enhance its functionality and provide features for development workflows. One of these extensions is CodeGPT, which brings the power of generative artificial intelligence to VS Code.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 CodeGPT allows you to manipulate your code effortlessly. You can use it to generate code from comments, refactor it, debug it, document it, or even explain what a certain block of code does.

## Installing and Configuring CodeGPT

 To install [CodeGPT](https://marketplace.visualstudio.com/items?itemName=DanielSanMedium.dscodegpt), launch VS Code. Then click on the extensions icon on the left sidebar of your window. Then search for **Code GPT**​​​​​​. It should be the first in the search results. Make sure it has a blue verification badge.

![CodeGPT extension in VSCode EXTENSIONS: MARKETPLACE](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/08/how-to-install-and-use-codegpt-in-vscode.jpg)

 Click on the **Install** button to add it to VS Code. Having installed CodeGPT, you now need to connect it to a large language model. This model is what gives it its generative capabilities.

 To establish the connection between CodeGPT and the large language model, you need an API Key. In this guide, you'll be [using the OpenAI API](https://www.makeuseof.com/openai-api-guide-what-can-you-do/). To get one proceed to the [OpenAI API](https://platform.openai.com/) platform and log in. If you do not have an account, sign up for one. After logging in, select the **API** option on the page that appears.

![OpenAI API service selection page](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/08/how-to-install-and-use-codegpt-in-vscode-api-homepage.jpg)

 This will take you to the API homepage. In the top right corner, click on your profile and select the **View API keys** option.

![OpenAI API homepage](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/08/how-to-install-and-use-codegpt-in-vscode-api-key-view.jpg)

 Now, you will be directed to the **API keys** page. Click on the **Create new secret key** option. Then, name and generate your secret key.

![OpenAI API key naming](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/08/how-to-install-and-use-codegpt-in-vscode-api-generation.jpg)

 This is the API key that you will use to connect the OpenAI [large language model](https://www.makeuseof.com/what-are-large-langauge-models-how-do-they-work/) to CodeGPT. Copy it to your clipboard.

 Proceed to VS Code and navigate to **Settings > Extensions > CodeGPT**​​​​​​.

![CodeGPT configuration page in VSCode](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/08/how-to-install-and-use-codegpt-in-vscode-codegpt-configuration.jpg)

 From this page, you can configure how CodeGPT interacts with the large language model. You can choose your **AI Provider**, **Max Tokens** for each request, and the **Model** to use. Also, when you scroll further down you can also set the **Temperature** value.

**Max Tokens** help you control the length of the generated text. The **Temperature** value which is between 0 and 1 helps you control the randomness of the text in the model's output. You are not limited to OpenAI LLM. You can use any of the language models in the **AI Provider** option, provided you have their API Key.

 To enter your API Key, press **Cmd + Shift + P** on Mac or **Ctrl + Shift + P** on Windows to open the command palette. Then search for CodeGPT and select **CodeGPT: Set API KEY**.

![CodeGPT API command on VSCode command palette](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/08/how-to-install-and-use-codegpt-in-vscode-command-pallete.jpg)

 Click on it and paste your API key on the prompt that appears. Save it by pressing **Enter**. Finally, reload VS Code to start using CodeGPT.

## Generating Code With CodeGPT

 To demonstrate the CodeGPT code generation feature, you will create a calculator app using Python.

 You can generate code with CodeGPT by the use of comments or using the chat CodeGPT chat window. To generate code from comments write a comment about what you would like CodeGPT to do in your script. Then with the cursor at the end of the comment, press **Ctrl + Shift + I**. CodeGPT will process the request and open a new window with the results.

![CodeGPT generating code from a comment](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/08/how-to-install-and-use-codegpt-in-vscode-comment-code-generation.jpg)

 You can then copy and paste the code into your script. This method is not tidy as the response has text on it.

 To generate code by chatting with CodeGPT, click on the CodeGPT chat icon on the left sidebar. This will open a chat window.

![CodeGPT chat window](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/08/how-to-install-and-use-codegpt-in-vscode-chat.jpg)

 Then input your request and click **Send**. In this case, the request is for a simple calculator. CodeGPT will process your request and generate your code in the chat window.

![CodeGPT code generation in the chat window](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/08/how-to-install-and-use-codegpt-in-vscode-code-generation-1.jpg)

 Click on the "insert code" arrow to automatically paste the code into your script. As you can see, this method is more tidy. The generated code is as shown below:

`def add(x, y):  
   return x + y  
def subtract(x, y):  
   return x - y  
def multiply(x, y):  
   return x * y  
def divide(x, y):  
   if y != 0:  
       return x / y  
   else:  
       return "Error: cannot divide by zero"  
print("Select operation:")  
print("1. Addition")  
print("2. Subtraction")  
print("3. Multiplication")  
print("4. Division")  
choice = input("Enter your choice (1-4): ")  
num1 = float(input("Enter the first number: "))  
num2 = float(input("Enter the second number: "))  
if choice == '1':  
   print(num1, "+", num2, "=", add(num1, num2))  
elif choice == '2':  
   print(num1, "-", num2, "=", subtract(num1, num2))  
elif choice == '3':  
   print(num1, "*", num2, "=", multiply(num1, num2))  
elif choice == '4':  
   print(num1, "/", num2, "=", divide(num1, num2))  
else:  
   print("Invalid input. Please try again.")  
`

 When you run the code it works correctly. With just a single prompt, you were able to create a simple calculator.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4576829&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/9e740b84bb48a64dde25061566299467/products/copy_1_jp_box_big.png" border="0">Jet Profiler for MySQL, Enterprise Version： Jet Profiler for MySQL is real-time query performance and diagnostics tool for the MySQL database server. Its detailed query information, graphical interface and ease of use makes this a great tool for finding performance bottlenecks in your MySQL databases. </a>
<!-- affiliate ads end -->
## Refactoring Your Code With CodeGPT

 To refactor your code, select the code that you want to refactor, then right-click on it and select **Refactor CodeGPT**. In the **Refactor CodeGPT** dialog box, enter your prompt describing the refactoring that you want to perform. For example, you could enter "refactor this code to use [a for loop](https://www.makeuseof.com/learn-for-loops-in-python/) instead of [a while loop](https://www.makeuseof.com/learn-while-loop-in-python/)".

 CodeGPT will generate new code that implements the requested refactoring.

<!-- affiliate ads begin -->
<a href="https://estore.macxdvd.com/order/checkout.php?PRODS=4526659&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.macxdvd.com/affiliate/new-banner/vcp-500x500.jpg" border="0"></a>
<!-- affiliate ads end -->
## Explaining Your Code With CodeGPT

 To explain your code, select the code that you want CodeGPT to explain. Then right-click on the highlighted code and select the **Explain CodeGPT** option.

![CodeGPT code explanation on the chat window](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/08/how-to-install-and-use-codegpt-in-vscode-codegpt-explanation.jpg)

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2068416/7443" target="_top" id="2068416"><img src="//a.impactradius-go.com/display-ad/7443-2068416" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2068416/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 CodeGPT will explain what the code does on the chat window.

<!-- affiliate ads begin -->
<a href="https://shop.systoolsgroup.com/affiliate.php?ACCOUNT=SYSTOOBY&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.systoolsgroup.com%3FAFFILIATE%3D108875%26RESOURCE%3DSysTools%2BSQL%2BRecovery"><img src="https://www.systoolsgroup.com/box/sql-recovery.png" border="0"></a>
<!-- affiliate ads end -->
## Documenting Your Code Using CodeGPT

[Documenting your code](https://www.makeuseof.com/python-code-document-using-docstrings/) helps other developers read and understand your code. It can also help you understand your code in the future.

 To document your code, select the code you want to document, then right-click on it and select the **Document CodeGPT** option. CodeGPT will generate documentation of the code in the chat window. You can then copy and paste the explanation into your documentation.

 For inline comments, use the chat window to instruct CodeGPT to insert the necessary inline comments into your code. Instructing CodeGPT to insert inline comments to the functions in the calculator app produces the following results:

`def add(x, y):  
   return x + y # returns the sum of x and y  
  
def subtract(x, y):  
   return x - y # returns the difference between x and y  
  
def multiply(x, y):  
   return x * y # returns the product of x and y  
  
def divide(x, y):  
   if y != 0:  
       return x / y # returns the division result of x and y  
   else:  
       # returns an error message if y is zero (dividing by zero is not allowed)  
       return "Error: cannot divide by zero" `

 These are clear and correct inline comments.

<!-- affiliate ads begin -->
<a href="https://shop.mondly.com/affiliate.php?ACCOUNT=ATISTUDI&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.mondly.com%3FAFFILIATE%3D108875%26RESOURCE%3D%2BEducational%2B300x600%2B"><img src="https://secure.avangate.com/images/merchant/69c418c33ec2e1a4267fa9bb77fa1428/educational-300x600.gif" border="0"></a>
<!-- affiliate ads end -->
## Understanding How Generative AI Works

 CodeGPT utilizes the power of generative AI for all its features. It may not always provide the correct information. Hence, you need to counter-check whether its results are correct. Understanding how generative AI works will help you become familiar with its strengths and weaknesses.

**SCROLL TO CONTINUE WITH CONTENT**

 CodeGPT allows you to manipulate your code effortlessly. You can use it to generate code from comments, refactor it, debug it, document it, or even explain what a certain block of code does.

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
<li><a href="https://youtube-data.techidaily.com/024-approved-ultimate-guide-selecting-8-exquisite-weddings-vids/"><u>[New] 2024 Approved  Ultimate Guide  Selecting 8 Exquisite Weddings - Vids</u></a></li>
<li><a href="https://article-helps.techidaily.com/new-stock-photos-without-watermarks-a-guide-for-2024/"><u>[New] Stock Photos Without Watermarks – A Guide for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/solved-google-chrome-has-stopped-working/"><u>[Solved] Google Chrome Has Stopped Working</u></a></li>
<li><a href="https://vimeo-videos.techidaily.com/2024-approved-avoiding-the-ignored-making-your-video-a-staff-pick-on-vimeo/"><u>2024 Approved  Avoiding the Ignored  Making Your Video a Staff Pick on Vimeo</u></a></li>
<li><a href="https://some-guidance.techidaily.com/2024-approved-unlock-your-devices-sound-identity-with-a-customized-whatsapp-ringtone/"><u>2024 Approved  Unlock Your Device's Sound Identity with a Customized WhatsApp Ringtone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/accelerate-your-computer-speeding-up-windows-11-vs-windows-turbocharging-techniques/"><u>Accelerate Your Computer: Speeding Up Windows 11 Vs. Windows Turbocharging Techniques</u></a></li>
<li><a href="https://instagram-video-files.techidaily.com/be-inspired-today-the-essentials-of-stunning-photos-on-ig/"><u>Be Inspired Today! The Essentials of Stunning Photos on IG</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/beginner-friendly-steps-setting-up-a-vpn-connection-on-your-apple-tv/"><u>Beginner-Friendly Steps: Setting up a VPN Connection on Your Apple TV</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/complete-overview-screenflow-v4-for-macos/"><u>Complete Overview  ScreenFlow v4 for macOS</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/connecting-your-xbox-one-gamepad-to-windows-pc-a-step-by-step-tutorial/"><u>Connecting Your Xbox One Gamepad to Windows PC: A Step-by-Step Tutorial</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/directx-download-for-windows-11-and-10-quickly-and-easily/"><u>DirectX Download for Windows 11 & 10. Quickly & Easily!</u></a></li>
<li><a href="https://hardware-tips.techidaily.com/dive-into-hardware-evaluations-with-toms-technological-perspectives/"><u>Dive Into Hardware Evaluations with Tom's Technological Perspectives</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1723807936957-do-you-need-a-vpn-yes-you-do-heres-why/"><u>Do You Need a VPN? Yes, You Do. Here's Why.</u></a></li>
<li><a href="https://hardware-updates.techidaily.com/download-and-activate-the-newest-thunderbolt-drivers-for-windows-computers/"><u>Download and Activate the Newest Thunderbolt Drivers for Windows Computers</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/easy-to-stream-from-ps4-without-delay/"><u>Easy to Stream From PS4 [Without Delay]</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/expert-solutions-for-when-your-logitech-wireless-mouse-stops-responding/"><u>Expert Solutions for When Your Logitech Wireless Mouse Stops Responding</u></a></li>
<li><a href="https://article-tips.techidaily.com/exploring-dji-phantom-3s-advanced-aerial-capabilities/"><u>Exploring DJI Phantom 3’S Advanced Aerial Capabilities</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/external-hard-drive-not-showing-up-in-windows-10-solved/"><u>External Hard Drive Not Showing Up in Windows 10 [Solved]</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/fixing-windows-11-installation-failed-issues-with-ease/"><u>Fixing 'Windows 11 Installation Failed' Issues with Ease</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/fresh-start-for-your-computer-doing-a-hard-reset-of-windows-7-without-any-physical-media/"><u>Fresh Start for Your Computer: Doing a Hard Reset of Windows 7 without Any Physical Media</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/from-novice-to-pro-how-to-proficiently-record-videos-with-your-computer/"><u>From Novice to Pro: How To Proficiently Record Videos with Your Computer</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/getting-past-a-glitch-ultimate-guide-for-thawing-out-stuck-windows-updates/"><u>Getting Past a Glitch: Ultimate Guide for Thawing Out Stuck Windows Updates</u></a></li>
<li><a href="https://android-unlock.techidaily.com/how-can-we-unlock-our-lava-agni-2-5g-phone-screen-by-drfone-android/"><u>How Can We Unlock Our Lava Agni 2 5G Phone Screen?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-deactivate-windows-security-feature-on-windows-10-using-three-different-methods/"><u>How to Deactivate Windows Security Feature on Windows 10 Using Three Different Methods</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-delete-a-virus-on-windows-10-4-methods/"><u>How to Delete a Virus on Windows 10 – 4 Methods</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-download-fortnite-on-pc-solved/"><u>How to Download Fortnite on PC [SOLVED]</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-enable-offline-mode-in-steam-and-keep-gaming/"><u>How to Enable Offline Mode in Steam and Keep Gaming</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-fix-exodus-for-your-kodi-device-following-the-latest-july-2020-patch/"><u>How to Fix Exodus for Your Kodi Device Following the Latest July 2020 Patch</u></a></li>
<li><a href="https://techidaily.com/how-to-reset-itel-a70-without-the-home-button-drfone-by-drfone-reset-android-reset-android/"><u>How to Reset Itel A70 Without the Home Button | Dr.fone</u></a></li>
<li><a href="https://video-capture.techidaily.com/in-2024-essential-mac-tech-tips-5-snapshot-strategies/"><u>In 2024, Essential Mac Tech Tips  5 Snapshot Strategies</u></a></li>
<li><a href="https://android-location-track.techidaily.com/in-2024-how-do-i-stop-someone-from-tracking-my-oppo-find-n3-flip-drfone-by-drfone-virtual-android/"><u>In 2024, How Do I Stop Someone From Tracking My Oppo Find N3 Flip? | Dr.fone</u></a></li>
<li><a href="https://android-unlock.techidaily.com/in-2024-how-to-reset-a-vivo-y78plus-phone-that-is-locked-by-drfone-android/"><u>In 2024, How to Reset a Vivo Y78+ Phone that is Locked?</u></a></li>
<li><a href="https://facebook-video-recording.techidaily.com/learn-the-procedure-for-automatic-video-broadcasting-on-facebook-for-2024/"><u>Learn the Procedure for Automatic Video Broadcasting on Facebook for 2024</u></a></li>
<li><a href="https://extra-support.techidaily.com/playful-media-extractor-evaluation-for-2024/"><u>Playful Media Extractor Evaluation for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/quick-guide-accessing-advanced-startup-settings-on-windows-11/"><u>Quick Guide: Accessing Advanced Startup Settings on Windows 11</u></a></li>
<li><a href="https://techidaily.com/repair-office-2003-files-word-excel-and-powerpointon-windows-by-stellar-guide/"><u>Repair Office 2003 Files (Word, Excel and PowerPoint)on Windows</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/seamless-torrent-acquisition-a-step-by-step-walkthrough-for-first-timers/"><u>Seamless Torrent Acquisition: A Step-by-Step Walkthrough for First-Timers</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/step-by-step-guide-turning-on-and-off-automatic-launch-programs-on-windows-abinary-operating-system/"><u>Step-by-Step Guide: Turning On and Off Automatic Launch Programs on Windows Abinary Operating System</u></a></li>
<li><a href="https://vp-tips.techidaily.com/the-best-apps-for-keeping-your-linkedin-vids-safe-and-sound-for-2024/"><u>The Best Apps for Keeping Your LinkedIn Vids Safe & Sound for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/top-techniques-for-high-quality-screen-recording-and-audio-capture-on-windows-systems/"><u>Top Techniques for High-Quality Screen Recording and Audio Capture on Windows Systems</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/top-two-techniques-for-simple-audio-extraction-from-youtube-videos/"><u>Top Two Techniques for Simple Audio Extraction From YouTube Videos</u></a></li>
<li><a href="https://win-blog.techidaily.com/troubleshoot-and-improve-performance-combat-csgos-stuttering-snags/"><u>Troubleshoot and Improve Performance: Combat CS:GO's Stuttering Snags</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/troubleshooting-tips-for-connecting-a-logitech-keyboard-in-windows-11-systems-that-wont-recognize-it/"><u>Troubleshooting Tips for Connecting a Logitech Keyboard in Windows 11 Systems That Won't Recognize It</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/troubleshooting-windows-10-how-to-fix-disabled-synchronization-features/"><u>Troubleshooting Windows 10: How to Fix Disabled Synchronization Features</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unleash-maximum-frame-rates-on-ps5xbox-series-x-with-the-new-skyrim-se-speed-upgrade-2024/"><u>Unleash Maximum Frame Rates on PS5/Xbox Series X with the New Skyrim SE Speed Upgrade, 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1723808235815-whats-new-in-windows-10-creators-update-insider-preview-build-1503/"><u>What's New in Windows 10 Creators Update: Insider Preview Build 1503</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/why-wont-my-oculus-controller-respond-tips-for-immediate-solutions/"><u>Why Won't My Oculus Controller Respond? Tips for Immediate Solutions</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/zoom-troubles-overcome-screen-sharing-problems-with-these-latest-fixes/"><u>Zoom Troubles? Overcome Screen Sharing Problems with These Latest Fixes</u></a></li>
</ul></div>
