---
title: Navigating the Installation of CodeGPT Into VS Code
date: 2024-08-15T02:34:57.754Z
updated: 2024-08-16T02:34:57.754Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Navigating the Installation of CodeGPT Into VS Code
excerpt: This Article Describes Navigating the Installation of CodeGPT Into VS Code
thumbnail: https://thmb.techidaily.com/77e082dee0c1d3d5334c873749cdc85b7f4282a5c68bf8d7b3fdd304d8146b2a.jpg
---

## Navigating the Installation of CodeGPT Into VS Code

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
<!-- affiliate ads begin -->
<a href="https://united.elfm.net/c/5597632/517826/4704" target="_top" id="517826"><img src="//a.impactradius-go.com/display-ad/4704-517826" border="0" alt="" width="728" height="90"/></a><img height="0" width="0" src="https://united.elfm.net/i/5597632/517826/4704" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 You can then copy and paste the code into your script. This method is not tidy as the response has text on it.

 To generate code by chatting with CodeGPT, click on the CodeGPT chat icon on the left sidebar. This will open a chat window.

![CodeGPT chat window](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/08/how-to-install-and-use-codegpt-in-vscode-chat.jpg)
<!-- affiliate ads begin -->
<a href="https://shop.systoolsgroup.com/affiliate.php?ACCOUNT=SYSTOOBY&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.systoolsgroup.com%3FAFFILIATE%3D108875%26RESOURCE%3DSysTools%2BSQL%2BRecovery"><img src="https://www.systoolsgroup.com/box/sql-recovery.png" border="0"></a>
<!-- affiliate ads end -->

 Then input your request and click **Send**. In this case, the request is for a simple calculator. CodeGPT will process your request and generate your code in the chat window.

![CodeGPT code generation in the chat window](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/08/how-to-install-and-use-codegpt-in-vscode-code-generation-1.jpg)
<!-- affiliate ads begin -->
<a href="https://store.massmailsoftware.com/order/checkout.php?PRODS=1095219&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/dc87c13749315c7217cdc4ac692e704c/banera_for_partners-20_%281%29.jpg" border="0"></a>
<!-- affiliate ads end -->

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
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4615471&QTY=1&AFFILIATE=108875&CART=1"><img src="https://images.wondershare.com/affiliate-image/affiliate_banners_en/max_782x90.png" border="0"></a>
<!-- affiliate ads end -->
## Refactoring Your Code With CodeGPT

 To refactor your code, select the code that you want to refactor, then right-click on it and select **Refactor CodeGPT**. In the **Refactor CodeGPT** dialog box, enter your prompt describing the refactoring that you want to perform. For example, you could enter "refactor this code to use [a for loop](https://www.makeuseof.com/learn-for-loops-in-python/) instead of [a while loop](https://www.makeuseof.com/learn-while-loop-in-python/)".

 CodeGPT will generate new code that implements the requested refactoring.

## Explaining Your Code With CodeGPT

 To explain your code, select the code that you want CodeGPT to explain. Then right-click on the highlighted code and select the **Explain CodeGPT** option.

![CodeGPT code explanation on the chat window](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/08/how-to-install-and-use-codegpt-in-vscode-codegpt-explanation.jpg)
<!-- affiliate ads begin -->
<a href="https://ukaidot.sjv.io/c/5597632/1793233/19578" target="_top" id="1793233"><img src="//a.impactradius-go.com/display-ad/19578-1793233" border="0" alt="" width="1200" height="1200"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1793233/19578" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 CodeGPT will explain what the code does on the chat window.

<!-- affiliate ads begin -->
<a href="https://checkout.mirillis.com/order/checkout.php?PRODS=4704640&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/547a5a56d43f6d40f9a6a2f76501d013/products/1_mirillis_action_boxshot_store_1x.jpg" border="0">
	Home Use license is dedicated for personal, non-commercial use only. 
	If Action! is used for commercial gain or to further any commercial purpose, 
	a Commercial Use license is required. Multi-license (volume discount) is intended for single 
 
	company, user or members of the same household. Action! - screen and game recorder</a>
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
<li><a href="https://extra-hints.techidaily.com/2024-approved-core-principles-in-internet-story-development/"><u>2024 Approved  Core Principles in Internet Story Development</u></a></li>
<li><a href="https://android-frp.techidaily.com/5-quick-methods-to-bypass-oppo-k11-5g-frp-by-drfone-android/"><u>5 Quick Methods to Bypass Oppo K11 5G FRP</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/authenticity-at-risk-recognizing-ai-influence-on-writing/"><u>Authenticity at Risk: Recognizing AI Influence on Writing</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chagpt-unveiled-android-and-ios-application/"><u>ChaGPT Unveiled: Android & iOS Application</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/charting-ethical-ai-journeys-the-role-of-governance-opensai-suggests/"><u>Charting Ethical AI Journeys: The Role of Governance, OpensAI Suggests</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/charting-the-course-of-ais-emotional-comprehension/"><u>Charting the Course of AI's Emotional Comprehension</u></a></li>
<li><a href="https://techno-recovery.techidaily.com/comprehensive-analysis-of-western-digitals-data-lifeguard-a-diagnostic-software-evaluation/"><u>Comprehensive Analysis of Western Digital's Data Lifeguard: A Diagnostic Software Evaluation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/demystifying-predictive-ais-workings-in-simple-terms/"><u>Demystifying Predictive AI's Workings in Simple Terms</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/elevate-your-resume-game-with-ai-innovation/"><u>Elevate Your Resume Game with AI Innovation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/enterprise-advancement-through-expanded-api-scope-gpt-whisper/"><u>Enterprise Advancement Through Expanded API Scope: GPT, Whisper</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/evaluating-ais-craft-in-cocktail-creation/"><u>Evaluating AI's Craft in Cocktail Creation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/explore-seamless-integrations-your-gateway-to-chatgpt-via-chrome/"><u>Explore Seamless Integrations: Your Gateway to ChatGPT via Chrome</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/from-concept-to-execution-python-for-gpt-3/"><u>From Concept to Execution: Python for GPT-3</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/from-gpt-1-to-gpt-4-an-in-depth-analysis/"><u>From GPT-1 To GPT-4: An In-Depth Analysis</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/from-script-to-scenario-chatgpts-six-steps-to-perfecting-roleplay/"><u>From Script to Scenario: ChatGPT's Six Steps to Perfecting Roleplay</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/gpt-3-unveils-game-changing-upgrades-key-highlights/"><u>GPT-3 Unveils Game-Changing Upgrades: Key Highlights</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/how-can-i-catch-the-regional-pokemon-without-traveling-on-xiaomi-redmi-note-13-proplus-5g-drfone-by-drfone-virtual-android/"><u>How Can I Catch the Regional Pokémon without Traveling On Xiaomi Redmi Note 13 Pro+ 5G | Dr.fone</u></a></li>
<li><a href="https://blog-min.techidaily.com/how-to-restore-wiped-videos-on-find-x6-by-fonelab-android-recover-video/"><u>How to restore wiped videos on Find X6</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-use-chatgpt-as-your-personal-assistant-for-work/"><u>How to Use ChatGPT as Your Personal Assistant for Work</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-use-chatgpt-to-write-a-poetry-book/"><u>How to Use ChatGPT to Write a Poetry Book</u></a></li>
<li><a href="https://android-transfer.techidaily.com/in-2024-2-ways-to-transfer-text-messages-from-vivo-y100t-to-iphone-1514131211x8-drfone-by-drfone-transfer-from-android-transfer-from-android/"><u>In 2024, 2 Ways to Transfer Text Messages from Vivo Y100t to iPhone 15/14/13/12/11/X/8/ | Dr.fone</u></a></li>
<li><a href="https://review-topics.techidaily.com/in-2024-does-airplane-mode-turn-off-gps-location-on-apple-iphone-se-2020-drfone-by-drfone-virtual-ios/"><u>In 2024, Does Airplane Mode Turn off GPS Location On Apple iPhone SE (2020)? | Dr.fone</u></a></li>
<li><a href="https://review-topics.techidaily.com/in-2024-how-to-change-google-play-location-on-xiaomi-redmi-note-12-pro-4g-drfone-by-drfone-virtual-android/"><u>In 2024, How to Change Google Play Location On Xiaomi Redmi Note 12 Pro 4G | Dr.fone</u></a></li>
<li><a href="https://android-location-track.techidaily.com/in-2024-how-to-check-distance-and-radius-on-google-maps-for-your-vivo-y100-5g-drfone-by-drfone-virtual-android/"><u>In 2024, How to Check Distance and Radius on Google Maps For your Vivo Y100 5G | Dr.fone</u></a></li>
<li><a href="https://apple-account.techidaily.com/in-2024-how-to-fix-when-apple-account-locked-on-apple-iphone-se-2022-by-drfone-ios/"><u>In 2024, How to Fix when Apple Account Locked On Apple iPhone SE (2022)?</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/in-2024-how-to-screen-mirror-on-apple-iphone-12-mini-drfone-by-drfone-ios/"><u>In 2024, How to Screen Mirror on Apple iPhone 12 mini? | Dr.fone</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/in-2024-overview-of-the-best-samsung-galaxy-f15-5g-screen-mirroring-app-drfone-by-drfone-android/"><u>In 2024, Overview of the Best Samsung Galaxy F15 5G Screen Mirroring App | Dr.fone</u></a></li>
<li><a href="https://extra-skills.techidaily.com/in-2024-script-zip-up-creating-srt-from-video-archives-fastly/"><u>In 2024, Script Zip-Up  Creating SRT From Video Archives Fastly</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/insightful-interaction-how-chatgpt-revolutionizes-data-analysis/"><u>Insightful Interaction: How ChatGPT Revolutionizes Data Analysis</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/journey-blueprint-top-picks-of-seven-ai-apps-for-free-travel-planning/"><u>Journey Blueprint: Top Picks of Seven AI Apps for FREE Travel Planning</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/leveraging-ai-for-better-health-with-chatgpt-techniques/"><u>Leveraging AI for Better Health with ChatGPT Techniques</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/overcoming-service-errors-between-chatgpt-and-plugins/"><u>Overcoming Service Errors Between ChatGPT and Plugins</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/peak-tools-enhancing-gpt-and-vs-code-collaboration/"><u>Peak Tools: Enhancing GPT & VS Code Collaboration</u></a></li>
<li><a href="https://extra-support.techidaily.com/pro-tips-navigating-without-watching-edgenuity-content-for-2024/"><u>Pro Tips  Navigating Without Watching Edgenuity Content for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/real-world-ai-mastery-top-7-strategies-revealed/"><u>Real-World AI Mastery: Top 7 Strategies Revealed</u></a></li>
<li><a href="https://win-solutions.techidaily.com/resolving-stutter-and-crashes-in-no-rest-for-the-wicked-a-comprehensive-troubleshooting-guide/"><u>Resolving Stutter & Crashes in 'No Rest for the Wicked': A Comprehensive Troubleshooting Guide</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revealing-the-hidden-powers-of-your-conversational-ai/"><u>Revealing the Hidden Powers of Your Conversational AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revolutionizing-learning-why-embrace-not-resist-ai-in-schools/"><u>Revolutionizing Learning: Why Embrace, Not Resist, AI in Schools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/sustainable-value-can-auto-gpt-work-alone/"><u>Sustainable Value: Can Auto-GPT Work Alone?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-art-of-intrigue-9-techniques-chatgpt-uses-in-fiction/"><u>The Art of Intrigue: 9 Techniques ChatGPT Uses in Fiction</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-rationale-behind-the-rhythm-chatgpt-4-and-its-slower-beat/"><u>The Rationale Behind the Rhythm: ChatGPT-4 & Its Slower Beat</u></a></li>
<li><a href="https://screen-recording.techidaily.com/top-screen-recording-tools-face-off-summary/"><u>Top Screen Recording Tools Face-Off Summary</u></a></li>
<li><a href="https://win-blog.techidaily.com/troubleshooting-tips-resolving-nvidia-control-panel-malfunctions/"><u>Troubleshooting Tips: Resolving NVIDIA Control Panel Malfunctions</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-the-top-9-powerful-chatgpt-tools/"><u>Unveiling the Top 9 Powerful ChatGPT Tools</u></a></li>
<li><a href="https://extra-information.techidaily.com/whats-new-in-big-sur-necessary-specs-and-features/"><u>What's New in Big Sur  Necessary Specs and Features</u></a></li>
</ul></div>
