---
title: "Unleashing Code Power: 10 Ways to Merge ChatGPT and VS Code"
date: 2024-10-16T17:31:45.034Z
updated: 2024-10-20T18:10:09.373Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Unleashing Code Power: 10 Ways to Merge ChatGPT and VS Code"
excerpt: "This Article Describes Unleashing Code Power: 10 Ways to Merge ChatGPT and VS Code"
thumbnail: https://thmb.techidaily.com/f7564240f8faa92ac0e388d789a175a79bd1b95533429025b3702f8272211ea0.jpg
---

## Unleashing Code Power: 10 Ways to Merge ChatGPT and VS Code

 You can be the boss of your tasks and boost your productivity when you learn to leverage the AI tools trooping out of research labs daily. VS Code features the ChatGPT extension to bring you an OpenAI-enabled coding environment.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 You can leverage ChatGPT's vast coding model to complete your projects more efficiently and quicker—right inside the IDE. Here are handy ways you can use ChatGPT with VS Code.

>  Disclaimer: This post includes affiliate links
>
>  If you click on a link and make a purchase, I may receive a commission at no extra cost to you.
>

## How to Install and Use the ChatGPT Extension in VS Code

 When you search for "ChatGPT" or "Code GPT" in VS Code extension marketplace, many related extensions come up. Unlike GitHub Copilot, these are not officially directly from OpenAI.

 Most VS Code ChatGPT extensions sampled work the same way, though. But we'll stick to [EasyCode's ChatGPT extension](https://marketplace.visualstudio.com/items?itemName=EasyCodeAI.chatgpt-gpt4-gpt3-vscode) for this article, as it's pretty decent for demonstrating ChatGPT use cases in VS Code. It supports GPT-4 and GPT-3.5, has a free tier, and doesn't require an API key.

 To install the ChatGPT extension in VS Code:

1. Open VS Code and click the settings icon at the bottom left of the left sidebar.
2. Go to **Extensions**.  
![VS Code extensions option](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/vs-code-extensions-option.jpg)
3. Alternatively, press **Ctrl + Shift + X** (**Command + Shift + X** for Mac) to directly open the extensions' marketplace.
4. Type "ChatGPT - EasyCode" in the search bar at the top-left.
5. Click the extension when seen.
6. Finally, click **Install**.  
![ChatGPT extension marketplace](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/chatgpt-extension-marketplace.jpg)
7. You'll see the extension icon in the left sidebar once installed.
8. Click the extension icon. Click **Try Without Account**. But feel free to **Sign In** if you have an account or **Sign Up** for a new account with the extension provider.  
![ChatGPT extension in VS Code sidebar](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/chatgpt-extension-in-vs-code-sidebar.jpg)

### How to Use the ChatGPT Extension

1. To use a built-in prompt, highlight the target code and right-click it. Select any of the available prompts.  
![ChatGPT VS Code options](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/chatgpt-vs-code-options-1.jpg)
2. To write a custom prompt, right-click on the highlighted code and select Ask GPT. Type your prompt in the chat box at the top and press **Enter**.  

<!-- affiliate ads begin -->
<a href="https://bluettius.sjv.io/c/5597632/2139112/17108" target="_top" id="2139112">
  <img src="//a.impactradius-go.com/display-ad/17108-2139112" border="0" alt="https://techidaily.com" width="250" height="90"/>
</a>
<img height="0" width="0" src="https://bluettius.sjv.io/i/5597632/2139112/17108" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

![Debug prompt](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/debug-prompt.jpg)

### How to Use the ChatGPT Extension With Your Code Base

 If you've opened VS Code to your code base directory and want ChatGPT to access underlying modules:

![Extension usage example](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/extension-usage-example.jpg)

1. Click the extension icon on the left sidebar. Then check the **Ask Codebase** box.
2. Copy the target code and paste it into the chat box.
3. Type your prompt below the code (press **Shift + Enter**) in the chat box.
4. Press **Enter** or click the send icon.

 Now let's see the various ways to use ChatGPT in VS Code.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2027167/19272" target="_top" id="2027167">
  <img src="//a.impactradius-go.com/display-ad/19272-2027167" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2027167/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

## 1\. Refactor and Modify Code

 ChatGPT has proven helpful for modifying procedural, functional, and object-oriented code.

 For example, using this extension, we asked ChatGPT to refactor the faulty code below, a Python function to create an arbitrary dictionary and add "Buy" to each value.

`def makeDict(n: str, **kwargs)->dict:  
    some : dict  
    for key, value in kwargs.items():  
        some = n+" "+value  
    return some  
  
newDict = makeDict("Buy", item1="GPT Book", item2="Java Tutorial", item3="Hiking Guide")  
`

 It did pretty well producing the correct code that gives the expected output, with detailed reasons for the modification:

![Refactored code correction example](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/refactored-code-correction-example-3.jpg)

<!-- affiliate ads begin -->
<a href="https://ephamedtechinc.pxf.io/c/5597632/2137226/26400" target="_top" id="2137226">
  <img src="//a.impactradius-go.com/display-ad/26400-2137226" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://ephamedtechinc.pxf.io/i/5597632/2137226/26400" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Further, you can use the **Ask a followup** box to tell ChtGPT to convert the code into a class and show how to instantiate it:

![Follow up box refactored into a class](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/follow-up-box-refactor-1.jpg)

 The generated code above is more modular and reusable.

## 2\. Debug Your Code

 If your code throws an error or doesn't work as it should, asking ChatGPT to debug it directly inside VS Code saves time.

 Although there's no built-in prompt for debugging, you can use the **Ask GPT** option to create a custom prompt to debug your code.

 We asked the ChatGPT extension to debug the code we used earlier. Not only did it debug. It explained it and generated the correct one, including its expected output.

![Debugged code output](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/debugged-code-output-1.jpg)

## 3\. Write Your Code in Another Language

 You might want to write a program in a particular language besides your core. You can write your code in your core language and ask ChatGPT to rewrite it in the chosen programming language.

 However, the generated code might require little human input, as ChatGPT might fail to provide a fully working converted code in some instances.

 For instance, we converted the following Python code into its C equivalent using VS Code ChatGPT extension:

![Code to to convert to C example](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/code-to-tp-convert-to-c-example.jpeg)

 You can achieve this by right-clicking on the highlighted code and selecting the **Ask GPT** option.

 Here's our prompt in VS Code:

![VS Code chatGPT code convert prompt](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/vs-code-chatgpt-code-convert-prompt.jpg)

<!-- affiliate ads begin -->
<a href="https://laganoo.pxf.io/c/5597632/1657396/16446" target="_top" id="1657396">
  <img src="//a.impactradius-go.com/display-ad/16446-1657396" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://laganoo.pxf.io/i/5597632/1657396/16446" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Although it generated the C equivalent twice before getting it right, the final code works.

![Generated C code](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/generated-c-code.jpg)

## 4\. Generate a Frontend Component for Your API

 If you've written an API with different endpoints, you can ask the ChatGPT extension to provide a frontend component to consume it using a particular framework. This could be React, Vue, or Angular.

 For instance, we used the extension to generate a React component for creating a meeting schedule based on an API endpoint created using Python's FastAPI:

![ChatGPT extension component prompt](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/chatgpt-extension-component-prompt-1.jpg)

 As done above, you might want to check the **Ask Codebase** box if you're dealing with a large code base.

 After referencing our code base, the VS Code ChatGPT extension provided a handy React component to use the provided endpoint:

![Generated react component](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/generated-react-component.jpg)

<!-- affiliate ads begin -->
<a href="https://ursime.pxf.io/c/5597632/2136548/16384" target="_top" id="2136548">
  <img src="//a.impactradius-go.com/display-ad/16384-2136548" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://ursime.pxf.io/i/5597632/2136548/16384" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

## 5\. Explain Code Blocks

 Assume you grabbed a piece of code from Stack Overflow or a GitHub repository. You can ask the ChatGPT extension in VS Code to explain how it works for better comprehension. This helps you debug such code easily if bugs arise due to future code changes.

 In this example use case, we asked the ChatGPT extension to explain the following code; a Python class for verifying users' email addresses.

![Code to to explain example](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/code-to-to-explain-example.jpeg)

 It generated the following response:

![Code explained example output](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/code-explained-example-output.jpg)

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2144278/7443" target="_top" id="2144278">
  <img src="//a.impactradius-go.com/display-ad/7443-2144278" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2144278/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2080328/19272" target="_top" id="2080328">
  <img src="//a.impactradius-go.com/display-ad/19272-2080328" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2080328/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

## 6\. Generate HTML Templates for Your Application

 Using the ChatGPT extension in VS Code, you can create an HTML template (like input fields) from scratch—using the extension chat box directly. For instance, you can tell it to create an HTML template for user registration.

![User registration template example](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/user-registration-template-example.jpg)

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2049378/7443" target="_top" id="2049378">
  <img src="//a.impactradius-go.com/display-ad/7443-2049378" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2049378/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 But what if you're writing an application that renders data into HTML directly (a non-SPA) and wants a project-specific template? You can use the ChatGPT extension in VS Code to create HTML templates that display the backend data to users.

 For instance, if you're using an [MVT architecture-based framework like Django](https://www.makeuseof.com/django-mvt-architecture/), you can use the extension to forge HTML templates for your Django views.

![Generated HMTL template example](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/generated-hmtl-template-example.jpg)

 Again, for this type of use case, you might want to click the **Ask Codebase** checkbox for ChatGPT to access your code base.

## 7\. Unit-Test Your Code

 As essential as unit testing is, it can be a time consumer. You can leverage the VS Code ChatGPT extension to generate unit tests for your code and save valuable development time.

 Although the ChatGPT extension has a built-in prompt for generating unit tests, you might want to write a custom prompt using the **Ask Codebase** option for specificity and a better result.

 We asked ChatGPT to write a unit test for a registration endpoint created using Python's FastAPI:

![Unit test prompt](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/unit-test-prompt.jpg)

 It sampled the code base efficiently to generate the required unit test:

![Generated unit tests](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/generated-unit-tests.jpg)

## 8\. Find Potential Security Vulnerabilities

 While it may not provide detailed security analysis, the VS Code ChatGPT extension can be a handy tool to quickly [check for security vulnerabilities in your application](https://www.makeuseof.com/find-web-application-vulnerabilities/) code base and save you time scanning manually.

![Security vulnerability prompt VS Code](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/security-vulnerability-prompt-vs-code.jpg)

 To allow ChatGPT to scan your code base, use the **Ask Codebase** option (click the extension icon and check the **Ask Codebase** box).

## 9\. Ask VS Code-Related Questions

 If you usually gamble your way around some old or [new VS Code features](http://www.makeuseof.com/new-features-in-vscode-v169/), feel free to ask your way around the IDE from the ChatGPT extension.

 For instance, you can ask the extension to recommend the best extensions for debugging a particular programming language.

![VS Code specific prompt](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/vs-code-specific-prompt.jpg)

 Or you can ask it a more technical question, like how to open VS Code from the command line.

![VS Code specific prompt technical](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/vs-code-specific-prompt-technical.jpg)

## 10\. Write Documentation Directly From VS Code

 You can write detailed documentation for a piece of code directly from VS Code with ease using the ChatGPT extension.

 For example, here's a detailed documentation of a Zoom link creation function (in HTML format) that we generated using the VS Code ChatGPT extension:

![Generated documentation example](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/generated-documentation-example.jpg)

## Code Efficiently With ChatGPT in VS Code

 As a programmer in a rapidly paced internet, you want to achieve a minimum viable product in the barest minimum time. Although ChatGPT isn't wholely dependable, it might aid your development journey if used creatively. And there are many more use cases of ChatGPT in programming. However, with all that said, ensure you validate ChatGPT's results, as they can be misleading sometimes.

**SCROLL TO CONTINUE WITH CONTENT**

 You can leverage ChatGPT's vast coding model to complete your projects more efficiently and quicker—right inside the IDE. Here are handy ways you can use ChatGPT with VS Code.

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
<li><a href="https://youtube-blog.techidaily.com/024-approved-mobile-and-desktop-techniques-for-youtube-short-video-submission/"><u>[New] 2024 Approved Mobile & Desktop Techniques for YouTube Short Video Submission</u></a></li>
<li><a href="https://vp-tips.techidaily.com/updated-the-definitive-srt-file-generation-manual/"><u>[Updated] The Definitive SRT File Generation Manual</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/construct-a-subsidized-windows-platform-for-gpt-mimicry/"><u>Construct a Subsidized Windows Platform for GPT Mimicry</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/decoding-the-revolution-in-language-tech-palm-2-by-google/"><u>Decoding the Revolution in Language Tech: PaLM 2 by Google</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/gpt-4-demystified-inclusive-ai-revolution/"><u>GPT-4 Demystified: Inclusive AI Revolution</u></a></li>
<li><a href="https://android-unlock.techidaily.com/in-2024-everything-you-need-to-know-about-lock-screen-settings-on-your-samsung-galaxy-a05s-by-drfone-android/"><u>In 2024, Everything You Need to Know about Lock Screen Settings on your Samsung Galaxy A05s</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/process-of-screen-sharing-xiaomi-redmi-note-12r-to-pc-detailed-steps-drfone-by-drfone-android/"><u>Process of Screen Sharing Xiaomi Redmi Note 12R to PC- Detailed Steps | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/protecting-prose-from-pseudo-penned-pages-by-algorithms/"><u>Protecting Prose From Pseudo-Penned Pages by Algorithms</u></a></li>
<li><a href="https://fix-guide.techidaily.com/realme-gt-neo-5-not-connecting-to-wi-fi-12-quick-ways-to-fix-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>Realme GT Neo 5 Not Connecting to Wi-Fi? 12 Quick Ways to Fix | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/sipping-on-chatgpt-cocktail-quality-insight/"><u>Sipping on ChatGPT: Cocktail Quality Insight</u></a></li>
<li><a href="https://techidaily.com/undelete-lost-music-from-asus-rog-phone-8-pro-by-fonelab-android-recover-music/"><u>Undelete lost music from Asus ROG Phone 8 Pro</u></a></li>
</ul></div>

