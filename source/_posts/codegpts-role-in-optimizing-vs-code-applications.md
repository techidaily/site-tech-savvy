---
title: CodeGPT's Role in Optimizing VS Code Applications
date: 2024-08-21T15:36:32.843Z
updated: 2024-08-22T15:36:32.843Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes CodeGPT's Role in Optimizing VS Code Applications
excerpt: This Article Describes CodeGPT's Role in Optimizing VS Code Applications
thumbnail: https://thmb.techidaily.com/ef372663750da3323ed4b8491ee9b4b175fd85bfcc73dd50c99f11aa454f80c7.jpg
---

## CodeGPT's Role in Optimizing VS Code Applications

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
<a href="https://aofit.pxf.io/c/5597632/1399701/16396" target="_top" id="1399701"><img src="//a.impactradius-go.com/display-ad/16396-1399701" border="0" alt="" width="960" height="300"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1399701/16396" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Refactoring Your Code With CodeGPT

 To refactor your code, select the code that you want to refactor, then right-click on it and select **Refactor CodeGPT**. In the **Refactor CodeGPT** dialog box, enter your prompt describing the refactoring that you want to perform. For example, you could enter "refactor this code to use [a for loop](https://www.makeuseof.com/learn-for-loops-in-python/) instead of [a while loop](https://www.makeuseof.com/learn-while-loop-in-python/)".

 CodeGPT will generate new code that implements the requested refactoring.

<!-- affiliate ads begin -->
<h3 id="200610"><a href="https://sentrypc.7eer.net/c/5597632/200610/3022">Parental Control Software</a></h3>
<span class="text-ad-content">
	#1 Rated Parental Control Software.<br/>
	Monitor & Control all PC Activity!<br/>
		<cite style="color:green">sentrypc.com/parental-controls/</cite>
	</span><img height="0" width="0" src="https://sentrypc.7eer.net/i/5597632/200610/3022" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Explaining Your Code With CodeGPT

 To explain your code, select the code that you want CodeGPT to explain. Then right-click on the highlighted code and select the **Explain CodeGPT** option.

![CodeGPT code explanation on the chat window](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/08/how-to-install-and-use-codegpt-in-vscode-codegpt-explanation.jpg)

<!-- affiliate ads begin -->
<a href="https://shop.pcdj.com/order/checkout.php?PRODS=4698998&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/47f4b6321e9fd8e8f7326a6adc1a7c1e/products/MacBook_Pro_lyrx-withsinger-tv.png" border="0">LYRX is an easy-to-use karaoke software with the professional features karaoke hosts need to perform with precision. LYRX is karaoke show hosting software that supports all standard karaoke file types as well as HD video formats, and it’s truly fun to use. 
LYRX Karaoke Software MAC/WINDOWS (Includes Activation For 3 Machines)</a>
<!-- affiliate ads end -->
 CodeGPT will explain what the code does on the chat window.

<!-- affiliate ads begin -->
<a href="https://checkout.abbyy.com/order/checkout.php?PRODS=39254549&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/0e5fb5c76fca16adbee503c9aff393cd/products/8_FR-Badges-NEW-FR-Standard-16-WIN-200.png" border="0"> PDF application, powered by AI-based OCR, for unified workflows with both digital and scanned documents. </a>
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
<a href="https://aligracehair.sjv.io/c/5597632/2087267/19272" target="_top" id="2087267"><img src="//a.impactradius-go.com/display-ad/19272-2087267" border="0" alt="" width="728" height="90"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2087267/19272" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://facebook-video-share.techidaily.com/new-in-2024-avoiding-common-pitfalls-in-youtube-sponsorships-according-to-famebit/"><u>[New] In 2024, Avoiding Common Pitfalls in YouTube Sponsorships, According to FameBit</u></a></li>
<li><a href="https://remote-screen-capture.techidaily.com/new-top-10-gratuitous-video-chats-with-desktop-viewing/"><u>[New] Top 10 Gratuitous Video Chats with Desktop Viewing</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/solved-obs-dropping-frames-2024-tips/"><u>[Solved] OBS Dropping Frames - 2024 Tips</u></a></li>
<li><a href="https://youtube-blog.techidaily.com/ed-2024-approved-youtubes-creative-playground-explained-with-ease/"><u>[Updated] 2024 Approved  YouTube's Creative Playground Explained with Ease</u></a></li>
<li><a href="https://snapchat-videos.techidaily.com/updated-in-2024-perfect-your-snapchat-boomerangs-quickly/"><u>[Updated] In 2024, Perfect Your Snapchat Boomerangs Quickly</u></a></li>
<li><a href="https://screen-recording.techidaily.com/2024-approved-stream-to-record-essential-know-how-for-tv-capture/"><u>2024 Approved  Stream to Record  Essential Know-How for TV Capture</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/best-android-data-recovery-retrieve-lost-contacts-from-zte-blade-a73-5g-by-fonelab-android-recover-contacts/"><u>Best Android Data Recovery - Retrieve Lost Contacts from ZTE Blade A73 5G.</u></a></li>
<li><a href="https://some-techniques.techidaily.com/expert-tips-zooming-in-on-videoleap-videos-for-2024/"><u>Expert Tips  Zooming In on Videoleap Videos for 2024</u></a></li>
<li><a href="https://techtrends.techidaily.com/going-wire-free-innovative-ways-to-gain-online-access-without-cables/"><u>Going Wire-Free: Innovative Ways to Gain Online Access Without Cables</u></a></li>
<li><a href="https://fix-guide.techidaily.com/how-to-fix-part-of-the-touch-screen-not-working-on-tecno-pova-5-pro-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>How To Fix Part of the Touch Screen Not Working on Tecno Pova 5 Pro | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-overcome-the-problem-when-itunes-cannot-communicate-with-your-iphone/"><u>How to Overcome the Problem When iTunes Cannot Communicate with Your iPhone</u></a></li>
<li><a href="https://blog-min.techidaily.com/how-to-recover-deleted-photos-from-android-gallery-after-format-on-motorola-moto-g-stylus-5g-2023-by-stellar-photo-recovery-android-mobile-photo-recover/"><u>How to recover deleted photos from Android Gallery after format on Motorola Moto G Stylus 5G (2023)</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-uninstall-windows-10-and-downgrade-to-windows-7-or-windows-81-quickly-and-easily/"><u>How to Uninstall Windows 10 and Downgrade to Windows 7 or Windows 8.1, Quickly and Easily!</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/how-to-unlock-sim-card-on-iphone-13-mini-online-without-jailbreak-by-drfone-ios/"><u>How to Unlock SIM Card on iPhone 13 mini online without jailbreak</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-update-windows-11-drivers-if-you-cant-find-them-on-manufacturers-website/"><u>How to Update Windows 11 Drivers if You Can't Find Them on Manufacturer's Website</u></a></li>
<li><a href="https://unlock-android.techidaily.com/in-2024-best-ways-on-how-to-unlockbypassswiperemove-honor-x9a-fingerprint-lock-by-drfone-android/"><u>In 2024, Best Ways on How to Unlock/Bypass/Swipe/Remove Honor X9a Fingerprint Lock</u></a></li>
<li><a href="https://extra-hints.techidaily.com/in-2024-choreographing-compelling-screen-trailers/"><u>In 2024, Choreographing Compelling Screen Trailers</u></a></li>
<li><a href="https://easy-unlock-android.techidaily.com/in-2024-downloading-samfw-frp-tool-30-for-nokia-c02-by-drfone-android/"><u>In 2024, Downloading SamFw FRP Tool 3.0 for Nokia C02</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/maximizing-video-quality-mastering-insta-to-mp4-conversion/"><u>Maximizing Video Quality  Mastering Insta-to-MP4 Conversion</u></a></li>
<li><a href="https://hardware-updates.techidaily.com/onboard-hazard-laptop-fire-forces-immediate-disembarkation-of-american-airlines-passenger-plane/"><u>Onboard Hazard: Laptop Fire Forces Immediate Disembarkation of American Airlines Passenger Plane</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/optimize-your-gaming-experience-tips-for-increasing-frames-per-second-fps-in-rust/"><u>Optimize Your Gaming Experience: Tips for Increasing Frames Per Second (FPS) in Rust</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/overwatch-reduce-buffering-what-does-it-do/"><u>Overwatch Reduce Buffering: What Does It Do?</u></a></li>
<li><a href="https://howto.techidaily.com/play-store-not-working-on-huawei-nova-y91-8-solutions-inside-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>Play Store Not Working On Huawei Nova Y91? 8 Solutions Inside | Dr.fone</u></a></li>
<li><a href="https://extra-resources.techidaily.com/prime-mobileweb-invest-in-no-cost-imagery-upgrade/"><u>Prime Mobile/Web  Invest in No-Cost Imagery Upgrade</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/quick-guide-disabling-automatic-windows-updates-on-windows-10/"><u>Quick Guide: Disabling Automatic Windows Updates on Windows 10</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1723808175815-remove-a-virus-from-android-cell-phone-without-factory-reset/"><u>Remove a Virus From Android Cell Phone – Without Factory Reset</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/reset-this-pc-windows-10-when-and-how-to-use-it/"><u>Reset This PC Windows 10 – When & How to Use It</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/resolving-itunes-error-invalid-device-responses-preventing-iphone-connections/"><u>Resolving iTunes Error: Invalid Device Responses Preventing iPhone Connections</u></a></li>
<li><a href="https://hardware-tips.techidaily.com/rising-dram-market-demands-lead-sk-hynix-towards-expanded-production/"><u>Rising DRAM Market Demands Lead SK Hynix Towards Expanded Production</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/seamlessly-connect-your-ps4-controller-step-by-step-tutorial/"><u>Seamlessly Connect Your PS4 Controller: Step-by-Step Tutorial</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/simple-solution-correcting-realtek-hd-sound-card-driver-malfunction/"><u>Simple Solution: Correcting Realtek HD Sound Card Driver Malfunction</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/simple-steps-to-disable-windows-11-updates-a-beginners-guide/"><u>Simple Steps to Disable Windows 11 Updates: A Beginner's Guide</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/simple-techniques-for-taking-easy-screenshots-on-pcs-and-laptops/"><u>Simple Techniques for Taking Easy Screenshots on PCs and Laptops</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/step-by-step-guide-securing-your-online-privacy-with-a-vpn-on-the-opera-browser/"><u>Step-by-Step Guide: Securing Your Online Privacy with a VPN on the Opera Browser</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/step-by-step-guide-switching-your-laptop-display-orientation/"><u>Step-by-Step Guide: Switching Your Laptop Display Orientation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/step-by-step-tutorial-thawing-out-a-locked-windows-10-system/"><u>Step-by-Step Tutorial: Thawing Out A Locked Windows 10 System</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-essentials-of-vpns-why-they-matter-and-their-functioning-explained/"><u>The Essentials of VPNs: Why They Matter and Their Functioning Explained</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/troubleshooting-and-resolving-issues-with-your-lagging-and-stuttering-computer-system/"><u>Troubleshooting and Resolving Issues with Your Lagging and Stuttering Computer System</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/troubleshooting-steps-when-oculus-quest-2-wont-pair-with-pc/"><u>Troubleshooting Steps When Oculus Quest 2 Won't Pair with PC</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ultimate-guide-stopping-auto-updates-of-drivers-in-windows-11/"><u>Ultimate Guide: Stopping Auto-Updates of Drivers in Windows 11</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ultimate-visual-guide-for-setting-up-bluetooth-audio-on-playstation-4/"><u>Ultimate Visual Guide for Setting Up Bluetooth Audio on PlayStation 4</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/windows-explorer-has-stopped-working-in-windows-7-solved/"><u>Windows Explorer Has Stopped Working in Windows 7 [Solved]</u></a></li>
</ul></div>
