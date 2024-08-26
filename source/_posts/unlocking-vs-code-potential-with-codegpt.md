---
title: Unlocking VS Code Potential with CodeGPT
date: 2024-08-25T17:31:36.822Z
updated: 2024-08-26T17:31:36.822Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Unlocking VS Code Potential with CodeGPT
excerpt: This Article Describes Unlocking VS Code Potential with CodeGPT
thumbnail: https://thmb.techidaily.com/df49fa8741560cd4a2c304321a86cf5312094c2923c9c82c5634adc9a69e6807.jpg
---

## Unlocking VS Code Potential with CodeGPT

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
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=2337838&QTY=1&AFFILIATE=108875&CART=1"><iframe width="640" height="390" src="https://www.youtube.com/embed/rzZwphIv4RM" title="APFill - Ink and Toner Coverage Calculator" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe></a>
<!-- affiliate ads end -->
## Refactoring Your Code With CodeGPT

 To refactor your code, select the code that you want to refactor, then right-click on it and select **Refactor CodeGPT**. In the **Refactor CodeGPT** dialog box, enter your prompt describing the refactoring that you want to perform. For example, you could enter "refactor this code to use [a for loop](https://www.makeuseof.com/learn-for-loops-in-python/) instead of [a while loop](https://www.makeuseof.com/learn-while-loop-in-python/)".

 CodeGPT will generate new code that implements the requested refactoring.

<!-- affiliate ads begin -->
<a href="https://propmoneyinc.pxf.io/c/5597632/1803115/14559" target="_top" id="1803115"><img src="//a.impactradius-go.com/display-ad/14559-1803115" border="0" alt="" width="859" height="859"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1803115/14559" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Explaining Your Code With CodeGPT

 To explain your code, select the code that you want CodeGPT to explain. Then right-click on the highlighted code and select the **Explain CodeGPT** option.

![CodeGPT code explanation on the chat window](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/08/how-to-install-and-use-codegpt-in-vscode-codegpt-explanation.jpg)

<!-- affiliate ads begin -->
<a href="https://shop.manycam.com/order/checkout.php?PRODS=17728032&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/8230bea7d54bcdf99cdfe85cb07313d5/mcaffbanner920x120.png" border="0"></a>
<!-- affiliate ads end -->
 CodeGPT will explain what the code does on the chat window.

<!-- affiliate ads begin -->
<a href="https://estore.winxdvd.com/order/checkout.php?PRODS=1412049&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.winxdvd.com/affiliate/new-banner/pt-200x200.jpg" border="0"></a>
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
<a href="https://otszone.ots7.com/order/checkout.php?PRODS=4713322&QTY=1&AFFILIATE=108875&CART=1"><img src="https://green.ots7.com/screenshots/OtsAV/OtsAVRadio1.90-300x188.jpg" border="0">OtsAV Radio Webcaster</a>
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
<li><a href="https://youtube-web.techidaily.com/024-approved-whats-youtube-creative-commons-and-how-to-use-it-to-make-video/"><u>[New] 2024 Approved  What's YouTube Creative Commons and How to Use It to Make Video</u></a></li>
<li><a href="https://article-knowledge.techidaily.com/new-critical-choice-10-apps-to-stream-your-favorite-rugby-matches/"><u>[New] Critical Choice 10 Apps to Stream Your Favorite Rugby Matches</u></a></li>
<li><a href="https://some-tips.techidaily.com/new-unleashing-creativity-harnessing-the-full-potential-of-movie-maker-windows-8/"><u>[New] Unleashing Creativity  Harnessing the Full Potential of Movie Maker (Windows 8)</u></a></li>
<li><a href="https://fox-friendly.techidaily.com/updated-decrypting-covertly-hid-viewers-responses-in-videos/"><u>[Updated] Decrypting Covertly-Hid Viewers' Responses in Videos</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/updated-illuminating-the-art-of-iphone-long-exposure/"><u>[Updated] Illuminating the Art of iPhone Long Exposure</u></a></li>
<li><a href="https://remote-screen-capture.techidaily.com/updated-in-2024-webcam-wizardry-crafting-ultimate-gamer-footage/"><u>[Updated] In 2024, WebCam Wizardry  Crafting Ultimate Gamer Footage</u></a></li>
<li><a href="https://video-capture.techidaily.com/updated-top-cycling-sims-worth-your-time/"><u>[Updated] Top Cycling Sims Worth Your Time</u></a></li>
<li><a href="https://hardware-reviews.techidaily.com/advanced-gadget-reviews-unveiling-insights-from-toms-hardware/"><u>Advanced Gadget Reviews: Unveiling Insights From Tom's Hardware</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-mastery-unmatched-online-course-selection/"><u>AI Mastery: Unmatched Online Course Selection</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-driven-paperclip-maximization-exploring-new-possibilities/"><u>AI-Driven Paperclip Maximization: Exploring New Possibilities</u></a></li>
<li><a href="https://extra-hints.techidaily.com/best-entry-level-camera-reviews-2024-for-beginners/"><u>Best Entry-Level Camera Reviews 2024 | for Beginners</u></a></li>
<li><a href="https://extra-resources.techidaily.com/best-rated-android-soundbanks-for-2024/"><u>Best-Rated Android Soundbanks for 2024</u></a></li>
<li><a href="https://howto.techidaily.com/bricked-your-vivo-y27-4g-heres-a-full-solution-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>Bricked Your Vivo Y27 4G? Heres A Full Solution | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/bridging-gaps-the-future-of-design-via-chatgpt-persona-creation/"><u>Bridging Gaps: The Future of Design via ChatGPT Persona Creation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/bringing-advanced-search-to-your-fingers-bings-ai-for-smartphones/"><u>Bringing Advanced Search to Your Fingers: Bing’s AI for Smartphones.</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-enhanced-excel-streamlining-complex-tasks-and-processes/"><u>ChatGPT-Enhanced Excel: Streamlining Complex Tasks and Processes</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/comparing-scales-public-vs-private-ai-systems/"><u>Comparing Scales: Public Vs. Private AI Systems</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/crafting-concepts-three-bots-on-a-creative-frontier/"><u>Crafting Concepts: Three Bots on a Creative Frontier</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/decoding-ai-interpretability-openais-shap-e/"><u>Decoding AI Interpretability: OpenAI's SHAP E</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/dialogue-dissection-gpt-vs-bingbots-10-key-dichotomies/"><u>Dialogue Dissection: GPT Vs. BingBot's 10 Key Dichotomies</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/discover-endless-possibilities-with-chatgpts-my-bot-capabilities/"><u>Discover Endless Possibilities With ChatGPT's My Bot Capabilities</u></a></li>
<li><a href="https://win-solutions.techidaily.com/effective-solutions-to-prevent-crackdown-3-from-crashing-on-your-desktop-computer/"><u>Effective Solutions to Prevent 'Crackdown 3' From Crashing on Your Desktop Computer</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/efficiency-in-academia-the-chatgpt-technique/"><u>Efficiency in Academia: The ChatGPT Technique</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/elite-ai-tools-empowering-digital-research-endeavors/"><u>Elite AI Tools Empowering Digital Research Endeavors</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/evaluating-artificial-intelligence-for-personal-finance-decisions/"><u>Evaluating Artificial Intelligence for Personal Finance Decisions</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/excels-advanced-operational-skills-eclipsing-chatgpts-potential/"><u>Excel's Advanced Operational Skills Eclipsing ChatGPT's Potential</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/exploring-the-nuances-of-using-gptzero-for-detecting-ai-content/"><u>Exploring the Nuances of Using GPTZero for Detecting AI Content</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/freelance-breakthroughs-unleash-potential-using-chatgpts-top-6-strategies/"><u>Freelance Breakthroughs: Unleash Potential Using ChatGPT's Top 6 Strategies</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/future-frontiers-the-new-era-of-chatbots-and-ai/"><u>Future Frontiers: The New Era of Chatbots & AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/futuristic-commute-mercedes-benz-melds-chatgpt-and-voice-control/"><u>Futuristic Commute: Mercedes-Benz Melds ChatGPT & Voice Control</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/get-to-know-gptzero-the-definitive-guide-for-distinguishing-ai-creations/"><u>Get to Know GPTZero: The Definitive Guide for Distinguishing AI Creations</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/gpt-and-student-essays-are-they-competing-titles-now/"><u>GPT and Student Essays: Are They Competing Titles Now?</u></a></li>
<li><a href="https://techidaily.com/how-to-easily-hard-reset-my-honor-x8b-drfone-by-drfone-reset-android-reset-android/"><u>How to Easily Hard reset my Honor X8b | Dr.fone</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/how-to-optimize-your-viewing-a-guide-to-high-definition-cricket-live-streaming-for-2024/"><u>How to Optimize Your Viewing  A Guide to High-Definition Cricket Live Streaming for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/idea-fountainheads-blending-mindmaps-with-ai/"><u>Idea Fountainheads: Blending Mindmaps with AI</u></a></li>
<li><a href="https://youtube-video-recordings.techidaily.com/in-2024-crafting-video-magic-with-imovie-directed-to-youtube/"><u>In 2024, Crafting Video Magic with iMovie, Directed to YouTube</u></a></li>
<li><a href="https://ios-unlock.techidaily.com/in-2024-how-to-change-your-apple-id-password-on-your-iphone-8-plus-by-drfone-ios/"><u>In 2024, How To Change Your Apple ID Password On your iPhone 8 Plus</u></a></li>
<li><a href="https://review-topics.techidaily.com/in-2024-how-to-simulate-gps-movement-in-ar-games-on-nokia-c12-pro-drfone-by-drfone-virtual-android/"><u>In 2024, How to Simulate GPS Movement in AR games On Nokia C12 Pro? | Dr.fone</u></a></li>
<li><a href="https://bypass-frp.techidaily.com/in-2024-the-complete-guide-to-vivo-x-flip-frp-bypass-everything-you-need-to-know-by-drfone-android/"><u>In 2024, The Complete Guide to Vivo X Flip FRP Bypass Everything You Need to Know</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-text-generation-your-openai-toolkit/"><u>Mastering Text Generation: Your OpenAI Toolkit</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/maximizing-productivity-top-10-ways-to-utilize-chatgpt-in-vs-code/"><u>Maximizing Productivity: Top 10 Ways to Utilize ChatGPT in VS Code</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/new-era-dawn-deciphering-twitters-metasig-phenomenon/"><u>New Era Dawn! Deciphering Twitter's Metasig Phenomenon</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/speeding-up-the-talk-comparing-chatgpt-4-and-35-speed/"><u>Speeding Up the Talk: Comparing ChatGPT-4 and 3.5 Speed</u></a></li>
<li><a href="https://facebook.techidaily.com/the-hidden-risks-in-accepting-everyones-friendship-overtures/"><u>The Hidden Risks in Accepting Everyone's Friendship Overtures</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-intersection-of-gaming-and-machine-learning-magic/"><u>The Intersection of Gaming and Machine Learning Magic</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-ultimate-guide-to-mastering-bings-ai-features-on-android/"><u>The Ultimate Guide to Mastering Bing's AI Features on Android</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/understanding-turings-challenge-is-it-unbeatable/"><u>Understanding Turing's Challenge: Is It Unbeatable?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-chatgpt-enterprise-potential/"><u>Unveiling ChatGPT Enterprise Potential</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-openais-tool-for-transparent-ai-insight/"><u>Unveiling OpenAI's Tool for Transparent AI Insight</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-the-best-of-ai-file-analysis-via-gpt/"><u>Unveiling the Best of AI: File Analysis via GPT</u></a></li>
<li><a href="https://win-solutions.techidaily.com/valorant-pc-troubles-heres-how-you-can-prevent-the-game-from-keeping-crashes/"><u>Valorant PC Troubles? Here's How You Can Prevent the Game From Keeping Crashes</u></a></li>
</ul></div>
