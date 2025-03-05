---
title: Step-by-Step Guide to CodeGPT in VS Code
date: 2025-02-25T20:07:38.235Z
updated: 2025-03-05T02:08:35.106Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Step-by-Step Guide to CodeGPT in VS Code
excerpt: This Article Describes Step-by-Step Guide to CodeGPT in VS Code
thumbnail: https://thmb.techidaily.com/7dc1f793da1f2b9c448c995323e3532e944d0308246b622538179ed42958d614.jpg
---

## Step-by-Step Guide to CodeGPT in VS Code

 VS Code has several useful extensions that enhance its functionality and provide features for development workflows. One of these extensions is CodeGPT, which brings the power of generative artificial intelligence to VS Code.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 CodeGPT allows you to manipulate your code effortlessly. You can use it to generate code from comments, refactor it, debug it, document it, or even explain what a certain block of code does.

>  Disclaimer: This post includes affiliate links
>
>  If you click on a link and make a purchase, I may receive a commission at no extra cost to you.
>

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

## Refactoring Your Code With CodeGPT

 To refactor your code, select the code that you want to refactor, then right-click on it and select **Refactor CodeGPT**. In the **Refactor CodeGPT** dialog box, enter your prompt describing the refactoring that you want to perform. For example, you could enter "refactor this code to use [a for loop](https://www.makeuseof.com/learn-for-loops-in-python/) instead of [a while loop](https://www.makeuseof.com/learn-while-loop-in-python/)".

 CodeGPT will generate new code that implements the requested refactoring.

## Explaining Your Code With CodeGPT

 To explain your code, select the code that you want CodeGPT to explain. Then right-click on the highlighted code and select the **Explain CodeGPT** option.

![CodeGPT code explanation on the chat window](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/08/how-to-install-and-use-codegpt-in-vscode-codegpt-explanation.jpg)

 CodeGPT will explain what the code does on the chat window.

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
<li><a href="https://youtube-video-recordings.techidaily.com/new-a-compre-written-in-sounds-youtube-playlists-decoded/"><u>[New] A Compre Written in Sounds YouTube Playlists Decoded</u></a></li>
<li><a href="https://instagram-video-files.techidaily.com/updated-discover-the-perfect-moment-timing-your-insta-posts/"><u>[Updated] Discover the Perfect Moment Timing Your Insta Posts</u></a></li>
<li><a href="https://fox-friendly.techidaily.com/updated-elevating-package-revelation-innovative-ways-for-first-encounters-for-2024/"><u>[Updated] Elevating Package Revelation Innovative Ways for First Encounters for 2024</u></a></li>
<li><a href="https://android-location.techidaily.com/9-best-free-android-monitoring-apps-to-monitor-phone-remotely-for-your-google-pixel-fold-drfone-by-drfone-virtual/"><u>9 Best Free Android Monitoring Apps to Monitor Phone Remotely For your Google Pixel Fold | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/black-friday-shockwave-how-virtual-reality-headsets-beat-apples-airpods-in-sales/"><u>Black Friday Shockwave: How Virtual Reality Headsets Beat Apple's AirPods in Sales!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/evolving-tech-the-enhanced-more-affordable-ar-laptop-without-a-display-latest-updates-from-zdnet/"><u>Evolving Tech: The Enhanced, More Affordable AR Laptop Without a Display - Latest Updates From ZDNet</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/experience-top-xbox-games-on-meta-quest-platform-without-needing-a-console-microsoft-enables-ported-classics/"><u>Experience Top Xbox Games on Meta Quest Platform without Needing a Console, Microsoft Enables Ported Classics</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-apple-pixar-and-nvidias-unprecedented-partnership-will-transform-3d-video-creation-into-a-monumental-venture-zdnet-insights/"><u>How Apple, Pixar, and Nvidia's Unprecedented Partnership Will Transform 3D Video Creation Into a Monumental Venture | ZDNet Insights</u></a></li>
<li><a href="https://extra-skills.techidaily.com/in-2024-speed-up-sound-on-smartphones-with-these/"><u>In 2024, Speed Up Sound on Smartphones with These</u></a></li>
<li><a href="https://fox-sys.techidaily.com/in-depth-analysis-unveiling-the-strengths-and-weaknesses-of-screencast-crafting-tool/"><u>In-Depth Analysis: Unveiling the Strengths & Weaknesses of Screencast-Crafting Tool</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/maximize-your-apple-vision-pro-experience-with-these-must-have-add-ons-recommended-by-zdnet/"><u>Maximize Your Apple Vision Pro Experience with These Must-Have Add-Ons Recommended by ZDNet</u></a></li>
<li><a href="https://windows11.techidaily.com/polishing-old-videos-windows-madvr-techniques-unveiled/"><u>Polishing Old Videos: Windows MadVR Techniques Unveiled</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/sunday-success-unlocked-chick-fil-as-innovative-strategy-revealed/"><u>Sunday Success Unlocked: Chick-Fil-A's Innovative Strategy Revealed</u></a></li>
<li><a href="https://fox-hovers.techidaily.com/the-essentials-of-hosting-a-zoom-event-via-android-for-2024/"><u>The Essentials of Hosting a Zoom Event via Android for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unitys-beta-launch-opens-doors-for-apple-vision-pro-start-creating-augmented-reality-and-virtual-reality-gaming-experiences-now/"><u>Unity's Beta Launch Opens Doors for Apple Vision Pro - Start Creating Augmented Reality & Virtual Reality Gaming Experiences Now</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/upcoming-apple-virtual-realityaugmented-reality-glasses-the-latest-insights-and-details-unveiled/"><u>Upcoming Apple Virtual Reality/Augmented Reality Glasses: The Latest Insights and Details Unveiled</u></a></li>
<li><a href="https://location-social.techidaily.com/why-your-whatsapp-live-location-is-not-updating-and-how-to-fix-on-your-samsung-galaxy-f54-5g-drfone-by-drfone-virtual-android/"><u>Why Your WhatsApp Live Location is Not Updating and How to Fix on your Samsung Galaxy F54 5G | Dr.fone</u></a></li>
</ul></div>

