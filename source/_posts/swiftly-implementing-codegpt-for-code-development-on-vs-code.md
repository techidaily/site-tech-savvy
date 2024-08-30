---
title: Swiftly Implementing CodeGPT for Code Development on VS Code
date: 2024-08-29T19:49:12.383Z
updated: 2024-08-30T19:49:12.383Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Swiftly Implementing CodeGPT for Code Development on VS Code
excerpt: This Article Describes Swiftly Implementing CodeGPT for Code Development on VS Code
thumbnail: https://thmb.techidaily.com/84772a0e20318a50277b6d80239d31259f3d754cba45388a4148935e78d13735.jpg
---

## Swiftly Implementing CodeGPT for Code Development on VS Code

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
<a href="https://imp.i357552.net/c/5597632/863039/11832" target="_top" id="863039"><img src="//a.impactradius-go.com/display-ad/11832-863039" border="0" alt="" width="300" height="250"/></a>
<!-- affiliate ads end -->
## Refactoring Your Code With CodeGPT

 To refactor your code, select the code that you want to refactor, then right-click on it and select **Refactor CodeGPT**. In the **Refactor CodeGPT** dialog box, enter your prompt describing the refactoring that you want to perform. For example, you could enter "refactor this code to use [a for loop](https://www.makeuseof.com/learn-for-loops-in-python/) instead of [a while loop](https://www.makeuseof.com/learn-while-loop-in-python/)".

 CodeGPT will generate new code that implements the requested refactoring.

<!-- affiliate ads begin -->
<a href="https://aspironcom.sjv.io/c/5597632/1941789/21554" target="_top" id="1941789"><img src="//a.impactradius-go.com/display-ad/21554-1941789" border="0" alt="" width="650" height="800"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1941789/21554" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Explaining Your Code With CodeGPT

 To explain your code, select the code that you want CodeGPT to explain. Then right-click on the highlighted code and select the **Explain CodeGPT** option.

![CodeGPT code explanation on the chat window](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/08/how-to-install-and-use-codegpt-in-vscode-codegpt-explanation.jpg)

<!-- affiliate ads begin -->
<a href="https://engwe.pxf.io/c/5597632/2093504/25579" target="_top" id="2093504"><img src="//a.impactradius-go.com/display-ad/25579-2093504" border="0" alt="" width="1200" height="1200"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2093504/25579" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 CodeGPT will explain what the code does on the chat window.

<!-- affiliate ads begin -->
<a href="https://estore.macxdvd.com/order/checkout.php?PRODS=4526659&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.macxdvd.com/affiliate/new-banner/vcp-500x500.jpg" border="0"></a>
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
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4665597&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.pcclean.io/wp-content/uploads/2018/03/winutilities-box-130521.png" border="0">WinUtilities Pro</a>
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
<li><a href="https://tiktok-videos.techidaily.com/new-in-2024-essential-techniques-5-methods-for-superior-tiktok-captioning/"><u>[New] In 2024, Essential Techniques  5 Methods for Superior TikTok Captioning</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/new-prime-7-fps-titles-you-cant-miss-for-2024/"><u>[New] Prime 7 FPS Titles You Can't Miss for 2024</u></a></li>
<li><a href="https://vimeo-videos.techidaily.com/new-selecting-the-right-video-subscription-plan-at-vimeo/"><u>[New] Selecting the Right Video Subscription Plan at Vimeo</u></a></li>
<li><a href="https://on-screen-recording.techidaily.com/new-ultimate-racing-game-anthology-the-top-five/"><u>[New] Ultimate Racing Game Anthology  The Top Five</u></a></li>
<li><a href="https://vp-tips.techidaily.com/updated-capture-action-the-complete-technique-for-adding-motion-blur-in-photos-for-2024/"><u>[Updated] Capture Action  The Complete Technique for Adding Motion Blur in Photos for 2024</u></a></li>
<li><a href="https://facebook-videos.techidaily.com/updated-maximize-views-sharing-your-twitch-stream-on-fb/"><u>[Updated] Maximize Views  Sharing Your Twitch Stream on FB</u></a></li>
<li><a href="https://fox-cloud.techidaily.com/updated-perfecting-visual-output-incorporating-luts-into-your-ae-projects/"><u>[Updated] Perfecting Visual Output  Incorporating LUTs Into Your AE Projects</u></a></li>
<li><a href="https://fox-cloud.techidaily.com/2024-approved-dynamic-directionality-prime-phone-friendly-tripods/"><u>2024 Approved  Dynamic Directionality  Prime Phone-Friendly Tripods</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/achieve-total-well-being-with-chatgpt-your-guide-to-life-transformation/"><u>Achieve Total Well-Being with ChatGPT: Your Guide to Life Transformation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/battle-royale-ai-titans-clash-chatgpt-vs-google-bard/"><u>Battle Royale: AI Titans Clash - ChatGPT Vs. Google Bard</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chrome-extensions-top-8-with-ai-for-peak-productivity/"><u>Chrome Extensions: Top 8 With AI for Peak Productivity</u></a></li>
<li><a href="https://tiktok-video-recordings.techidaily.com/crafting-your-legacy-the-ultimate-list-of-20-iconic-tiktok-captions/"><u>Crafting Your Legacy  The Ultimate List of 20 Iconic TikTok Captions</u></a></li>
<li><a href="https://win11-tips.techidaily.com/deciphering-your-pcs-intel-processor-gen-through-windows/"><u>Deciphering Your PC's Intel Processor Gen Through Windows</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/delving-into-how-devices-learn-without-cloud-connectivity/"><u>Delving Into How Devices Learn Without Cloud Connectivity</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/diving-into-gpt-enhanced-jobs-money-making-scenarios-explored/"><u>Diving Into GPT-Enhanced Jobs: Money-Making Scenarios Explored</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/embark-on-your-ai-search-adventure-with-bing-sign-up-process/"><u>Embark on Your AI Search Adventure with Bing: Sign Up Process</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/enhancements-arrive-chatgpt-introduces-top-tier-updates/"><u>Enhancements Arrive: ChatGPT Introduces Top-Tier Updates!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/enrich-browser-interactions-the-best-7-ai-chatter-extensions/"><u>Enrich Browser Interactions: The Best 7 AI Chatter Extensions</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ensuring-quality-control-when-integrating-chatgpt-into-your-workflow/"><u>Ensuring Quality Control when Integrating ChatGPT Into Your Workflow</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/evaluating-chatgpts-economic-impact-on-8-business-models/"><u>Evaluating ChatGPT's Economic Impact on 8 Business Models</u></a></li>
<li><a href="https://hardware-tips.techidaily.com/explore-felicia-days-collection-of-downloadable-3d-printer-add-ons-on-thangs-platform/"><u>Explore Felicia Day's Collection of Downloadable 3D Printer Add-Ons on Thangs Platform</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/explore-linguistic-horizons-using-premium-chatgptplus/"><u>Explore Linguistic Horizons Using Premium ChatGPT+</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/fabricate-exclusive-language-models/"><u>Fabricate Exclusive Language Models</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/futurists-unite-global-leaders-on-ai-prospects/"><u>Futurists Unite: Global Leaders on AI Prospects</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/gaming-giants-reimagined-bz-and-ms-merger-sparks-new-wave-in-ai-driven-creativity-and-translation-podcast-exploration/"><u>Gaming Giants Reimagined: BZ & MS Merger Sparks New Wave in AI-Driven Creativity and Translation [Podcast Exploration]</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/governance-and-governors-charting-4-paths-for-ai-tools/"><u>Governance and Governors: Charting 4 Paths for AI Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/hack-turn-dall-e-webp-photos-into-standard-jpegpng/"><u>Hack: Turn DALL-E WebP Photos Into Standard JPEG/PNG</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-automate-your-document-creation-with-chatgpt-in-microsoft-word/"><u>How to Automate Your Document Creation With ChatGPT in Microsoft Word</u></a></li>
<li><a href="https://facebook.techidaily.com/how-to-leverage-symbolic-meanings-in-social-media-conversations/"><u>How to Leverage Symbolic Meanings in Social Media Conversations</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/immediate-assistance-at-fingertips-bing-ai-on-the-go-with-android-keyboards/"><u>Immediate Assistance at Fingertips: Bing AI on the Go with Android Keyboards</u></a></li>
<li><a href="https://review-topics.techidaily.com/in-2024-complete-tutorial-to-use-gps-joystick-to-fake-gps-location-on-apple-iphone-12-drfone-by-drfone-virtual-ios/"><u>In 2024, Complete Tutorial to Use GPS Joystick to Fake GPS Location On Apple iPhone 12 | Dr.fone</u></a></li>
<li><a href="https://android-transfer.techidaily.com/in-2024-how-to-migrate-android-data-from-honor-100-to-new-android-phone-drfone-by-drfone-transfer-from-android-transfer-from-android/"><u>In 2024, How to Migrate Android Data From Honor 100 to New Android Phone? | Dr.fone</u></a></li>
<li><a href="https://bypass-frp.techidaily.com/in-2024-is-gsm-flasher-adb-legit-full-review-to-bypass-your-nubia-red-magic-8s-proplus-phone-frp-lock-by-drfone-android/"><u>In 2024, Is GSM Flasher ADB Legit? Full Review To Bypass Your Nubia Red Magic 8S Pro+ Phone FRP Lock</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/inside-look-best-practices-for-using-gpt-3-openai-style/"><u>Inside Look: Best Practices for Using GPT-3, OpenAI Style</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/language-giants-face-off-chatgpt-and-googles-bard-duel/"><u>Language Giants Face Off: ChatGPT & Google's Bard Duel</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/leveraging-chatgpt-via-siri-on-ios-devices/"><u>Leveraging ChatGPT via Siri on iOS Devices</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-the-enrollment-process-for-chatgpt-updates/"><u>Mastering the Enrollment Process for ChatGPT Updates</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/method-to-resolve-plugin-service-link-failures-in-chatgpt/"><u>Method to Resolve Plugin-Service Link Failures in ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/optimizing-your-wellbeing-top-9-chatgpt-uses/"><u>Optimizing Your Wellbeing: Top 9 ChatGPT Uses</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/pioneering-llm-tech-revolutionizing-natural-language-understanding/"><u>Pioneering LLM Tech: Revolutionizing Natural Language Understanding</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/seamless-content-generation-using-hixgpt-4/"><u>Seamless Content Generation Using HIX/GPT-4</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/snap-vs-gpt-choosing-your-social-tech-ally/"><u>Snap vs GPT: Choosing Your Social Tech Ally</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/speak-to-chatgpt-your-personal-ai/"><u>Speak to ChatGPT – Your Personal AI</u></a></li>
<li><a href="https://driver-download.techidaily.com/step-by-step-guide-installing-your-nexiq-usb-connection-driver-today/"><u>Step-by-Step Guide: Installing Your Nexiq USB Connection Driver Today</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/tackling-chatgpts-character-restrictions/"><u>Tackling ChatGPT's Character Restrictions</u></a></li>
<li><a href="https://tech-hub.techidaily.com/the-new-frontier-are-ai-systems-ready-for-a-change/"><u>The New Frontier: Are AI Systems Ready for a Change?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-world-embraces-gpt-4-understanding-the-impact/"><u>The World Embraces GPT-4: Understanding the Impact</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/turbo-power-unleashed-optimal-free-copilot-usage/"><u>Turbo Power Unleashed: Optimal Free Copilot Usage</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unfolding-gpt-4-integration-in-these-7-modern-tools/"><u>Unfolding GPT-4 Integration in These 7 Modern Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unpacking-googles-artificial-intelligence-gemini-project/"><u>Unpacking Google's Artificial Intelligence Gemini Project</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unravel-the-mysteries-of-artificial-intelligence-learn-to-use-free-dall-e-3-on-bing-by-microsoft/"><u>Unravel the Mysteries of Artificial Intelligence: Learn to Use Free DALL-E 3 on Bing by Microsoft</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unraveling-the-workings-of-gpt-4-in-these-7/"><u>Unraveling The Workings of GPT-4 in These 7</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-the-best-in-4k-technology-in-depth-review-of-sealoc-coastal-silver-55-screen-ideal-for-outdoor-viewing-pleasures/"><u>Unveiling the Best in 4K Technology: In-Depth Review of Sealoc Coastal Silver 55 Screen - Ideal for Outdoor Viewing Pleasures</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/why-authenticity-over-automation-textual-ai-pitfalls/"><u>Why Authenticity Over Automation: Textual AI Pitfalls</u></a></li>
</ul></div>
