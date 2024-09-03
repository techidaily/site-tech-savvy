---
title: Seamless Use of CodeGPT Within VS Code
date: 2024-09-02T20:36:54.201Z
updated: 2024-09-03T20:36:54.201Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Seamless Use of CodeGPT Within VS Code
excerpt: This Article Describes Seamless Use of CodeGPT Within VS Code
thumbnail: https://thmb.techidaily.com/e55121a8e00138bfd889740b0f7a193e7e03922e85acffafd82353c8a22765d2.jpg
---

## Seamless Use of CodeGPT Within VS Code

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
<a href="https://appsumo.8odi.net/c/5597632/2075475/7443" target="_top" id="2075475"><img src="//a.impactradius-go.com/display-ad/7443-2075475" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2075475/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Refactoring Your Code With CodeGPT

 To refactor your code, select the code that you want to refactor, then right-click on it and select **Refactor CodeGPT**. In the **Refactor CodeGPT** dialog box, enter your prompt describing the refactoring that you want to perform. For example, you could enter "refactor this code to use [a for loop](https://www.makeuseof.com/learn-for-loops-in-python/) instead of [a while loop](https://www.makeuseof.com/learn-while-loop-in-python/)".

 CodeGPT will generate new code that implements the requested refactoring.

<!-- affiliate ads begin -->
<a href="https://store.movavi.com/affiliate.php?ACCOUNT=MOVAVI&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.movavi.com%3FAFFILIATE%3D108875%26RESOURCE%3DMovavi%2BVideo%2BConverter%2BBox"><img src="https://mcusercontent.com/0885a03ded3d480dca9287f12/images/8020c1dc-518e-3bdf-6e7b-e6d1bdf1597b.jpg" border="0"></a>
<!-- affiliate ads end -->
## Explaining Your Code With CodeGPT

 To explain your code, select the code that you want CodeGPT to explain. Then right-click on the highlighted code and select the **Explain CodeGPT** option.

![CodeGPT code explanation on the chat window](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/08/how-to-install-and-use-codegpt-in-vscode-codegpt-explanation.jpg)

<!-- affiliate ads begin -->
<a href="https://imp.i357552.net/c/5597632/863039/11832" target="_top" id="863039"><img src="//a.impactradius-go.com/display-ad/11832-863039" border="0" alt="" width="300" height="250"/></a>
<!-- affiliate ads end -->
 CodeGPT will explain what the code does on the chat window.

<!-- affiliate ads begin -->
<a href="https://coinrule.sjv.io/c/5597632/1958374/18409" target="_top" id="1958374"><img src="//a.impactradius-go.com/display-ad/18409-1958374" border="0" alt="" width="300" height="300"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1958374/18409" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://aspironcom.sjv.io/c/5597632/1941789/21554" target="_top" id="1941789"><img src="//a.impactradius-go.com/display-ad/21554-1941789" border="0" alt="" width="650" height="800"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1941789/21554" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://extra-hints.techidaily.com/new-10-finest-fee-free-lut-options-reviewed-and-accessible-here/"><u>[New] 10 Finest, Fee-Free LUT Options Reviewed & Accessible Here</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/new-budget-friendly-video-grabber-selections-for-2024/"><u>[New] Budget-Friendly Video Grabber Selections for 2024</u></a></li>
<li><a href="https://on-screen-recording.techidaily.com/new-expert-techniques-for-high-quality-android-recordings/"><u>[New] Expert Techniques for High-Quality Android Recordings</u></a></li>
<li><a href="https://screen-capture.techidaily.com/new-in-2024-advanced-procedures-for-livestreaming-sporting-spectacles/"><u>[New] In 2024, Advanced Procedures for Livestreaming Sporting Spectacles</u></a></li>
<li><a href="https://article-knowledge.techidaily.com/new-techniques-for-fabulous-photo-collage-artistry/"><u>[New] Techniques for Fabulous Photo Collage Artistry</u></a></li>
<li><a href="https://fox-glue.techidaily.com/updated-capturing-heights-a-deep-dive-into-gopro-karma/"><u>[Updated] Capturing Heights  A Deep Dive Into GoPro Karma</u></a></li>
<li><a href="https://instagram-clips.techidaily.com/updated-masterclass-in-design-upgrading-igtv-backgrounds/"><u>[Updated] Masterclass in Design  Upgrading IGTV Backgrounds</u></a></li>
<li><a href="https://fox-glue.techidaily.com/updated-perfect-your-movie-watching-with-added-captions-on-windows-media-player-for-2024/"><u>[Updated] Perfect Your Movie Watching with Added Captions on Windows Media Player for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-command-connoisseurs-best-courses-unveiled/"><u>AI Command Connoisseurs: Best Courses Unveiled</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-enhanced-solutions-for-hr-efficiency/"><u>AI Enhanced Solutions for HR Efficiency</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/altering-email-on-protonbrowser-a-comprehensive-guide/"><u>Altering Email on ProtonBrowser - A Comprehensive Guide</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/artistic-integrity-vs-tech-might-the-sarah-silverman-suit/"><u>Artistic Integrity Vs. Tech Might: The Sarah Silverman Suit</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/bypassing-the-500-word-cap-with-chatgpt/"><u>Bypassing the 500-Word Cap with ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/crafting-epic-scenarios-with-ai-assistance/"><u>Crafting Epic Scenarios with AI Assistance</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/deciphering-chatgpt-control-pros-and-cons/"><u>Deciphering ChatGPT Control: Pros & Cons</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/decoding-six-common-car-ai-configurations-fails/"><u>Decoding Six Common Car AI Configurations Fails</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/digital-storytelling-engaging-text-based-rpg-with-chatgpt/"><u>Digital Storytelling: Engaging Text-Based RPG with ChatGPT</u></a></li>
<li><a href="https://screen-activity-recording.techidaily.com/discovering-the-capabilities-of-bandicams-screen-capture-feature/"><u>Discovering the Capabilities of Bandicam's Screen Capture Feature</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/essential-techniques-for-using-gpt-3-openai-edition/"><u>Essential Techniques for Using GPT-3, OpenAI Edition</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/evaluating-artificial-companions-in-psychological-care/"><u>Evaluating Artificial Companions in Psychological Care</u></a></li>
<li><a href="https://win-forum.techidaily.com/1722915229386-exploring-major-networks-connect-with-facebook-twitter-instagram-and-youtube/"><u>Exploring Major Networks: Connect with Facebook, Twitter, Instagram and Youtube!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/github-copilot-vs-chatgpt-which-is-better-for-programming/"><u>GitHub Copilot Vs. ChatGPT: Which Is Better for Programming?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/gpts-potential-in-revolutionizing-medical-services/"><u>GPT's Potential in Revolutionizing Medical Services</u></a></li>
<li><a href="https://blog-min.techidaily.com/how-to-identify-malfunctioning-hardware-drivers-with-windows-device-manager-in-windows-11107-by-drivereasy-guide/"><u>How to identify malfunctioning hardware drivers with Windows Device Manager in Windows 11/10/7</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/how-to-record-vimeo-in-2024/"><u>How to Record Vimeo, In 2024</u></a></li>
<li><a href="https://win-blog.techidaily.com/how-to-repair-palworld-session-search-glitches-quickly/"><u>How to Repair Palworld Session Search Glitches Quickly</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ideal-enhancements-boosting-chatgpt-and-vs-code-synergy/"><u>Ideal Enhancements: Boosting ChatGPT & VS Code Synergy</u></a></li>
<li><a href="https://screen-sharing-recording.techidaily.com/in-2024-hp-laptop-tutorial-easy-webcam-video-recording-steps/"><u>In 2024, HP Laptop Tutorial  Easy Webcam Video Recording Steps</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/inside-ais-frailty-decoding-how-prompt-injection-threat-operates/"><u>Inside AI's Frailty: Decoding How Prompt Injection Threat Operates</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/laughter-algorithm-computing-milestones-and-privacy-in-the-cloud/"><u>Laughter Algorithm: Computing Milestones & Privacy in the Cloud</u></a></li>
<li><a href="https://extra-skills.techidaily.com/launch-free-portable-dvd-software-today-for-2024/"><u>Launch Free, Portable DVD Software Today for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/launching-microsoft-copilot-on-a-mac-with-flair/"><u>Launching Microsoft Copilot on a Mac with Flair</u></a></li>
<li><a href="https://youtube-video-recordings.techidaily.com/live-stream-success-obs-steps-to-shine-on-youtube/"><u>Live Stream Success  OBS Steps to Shine on Youtube</u></a></li>
<li><a href="https://techtrends.techidaily.com/messaging-insights-techniques-to-tell-when-your-sms-is-actually-viewed/"><u>Messaging Insights: Techniques to Tell When Your SMS Is Actually Viewed</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/overcoming-the-top-4-barriers-in-your-gpt-account/"><u>Overcoming the Top 4 Barriers in Your GPT Account</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/quick-recognition-of-sham-chatgpt-sites/"><u>Quick Recognition of Sham ChatGPT Sites</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/shielding-sensitive-information-from-customized-ai/"><u>Shielding Sensitive Information From Customized AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/stealthy-gpt-conversation-archiving-strategies/"><u>Stealthy GPT Conversation Archiving Strategies</u></a></li>
<li><a href="https://facebook-video-content.techidaily.com/step-by-step-guide-to-creating-fb-slideshows/"><u>Step-by-Step Guide to Creating FB Slideshows</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/streamlining-persona-building-in-chatgpt-driven-design/"><u>Streamlining Persona Building in ChatGPT-Driven Design</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/subscriptionshutdowns-seeking-new-access-era/"><u>SubscriptionShutdowns: Seeking New Access Era</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/surprising-fact-start-a-dialogue-with-chatgpt/"><u>Surprising Fact: Start a Dialogue with ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-9-most-overlooked-dangers-when-using-ai-for-mental-support/"><u>The 9 Most Overlooked Dangers When Using AI for Mental Support</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-journey-from-concept-to-collection-via-chatgpt/"><u>The Journey From Concept to Collection via ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-power-of-conversational-ai-for-workflow-optimization/"><u>The Power of Conversational AI for Workflow Optimization</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-synergy-of-technology-and-spirituality-with-chatgpt/"><u>The Synergy of Technology and Spirituality with ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/three-paths-to-harnessing-gpt-4-for-free/"><u>Three Paths to Harnessing GPT-4 for Free</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ubuntu-bash-integrating-shellgpt-with-openais-chatgpt/"><u>Ubuntu Bash: Integrating ShellGPT with OpenAI's ChatGPT</u></a></li>
<li><a href="https://instagram-clips.techidaily.com/unlock-potential-innovating-with-effective-instagram-video-loops/"><u>Unlock Potential  Innovating with Effective Instagram Video Loops</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-7-issues-with-generative-ai-for-chats/"><u>Unveiling 7 Issues with Generative AI for Chats</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-auto-gpt-download-and-installation/"><u>Unveiling Auto-GPT: Download & Installation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/voice-activated-strategies-for-directing-ai-5-gpt-techniques/"><u>Voice-Activated Strategies for Directing AI: 5 GPT Techniques</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/who-wins-in-ai-battle-the-gpt-showdown-with-bing-and-bard/"><u>Who Wins in AI Battle? The GPT Showdown with Bing and Bard</u></a></li>
</ul></div>
