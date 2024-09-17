---
title: "Enhancing Coding Experience: 10 ChatGPT VS Code Combos"
date: 2024-09-16T16:16:46.434Z
updated: 2024-09-17T16:10:24.949Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Enhancing Coding Experience: 10 ChatGPT VS Code Combos"
excerpt: "This Article Describes Enhancing Coding Experience: 10 ChatGPT VS Code Combos"
thumbnail: https://thmb.techidaily.com/dc048da36d4f74b4d171bfb2845fad3bf8d729c04e77596617ba912c21778696.jpg
---

## Enhancing Coding Experience: 10 ChatGPT VS Code Combos

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
![Debug prompt](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/debug-prompt.jpg)

### How to Use the ChatGPT Extension With Your Code Base

 If you've opened VS Code to your code base directory and want ChatGPT to access underlying modules:

![Extension usage example](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/extension-usage-example.jpg)

1. Click the extension icon on the left sidebar. Then check the **Ask Codebase** box.
2. Copy the target code and paste it into the chat box.
3. Type your prompt below the code (press **Shift + Enter**) in the chat box.
4. Press **Enter** or click the send icon.

 Now let's see the various ways to use ChatGPT in VS Code.

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

 Although it generated the C equivalent twice before getting it right, the final code works.

![Generated C code](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/generated-c-code.jpg)

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2135416/19272" target="_top" id="2135416">
  <img src="//a.impactradius-go.com/display-ad/19272-2135416" border="0" alt="https://techidaily.com" width="336" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135416/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

## 4\. Generate a Frontend Component for Your API

 If you've written an API with different endpoints, you can ask the ChatGPT extension to provide a frontend component to consume it using a particular framework. This could be React, Vue, or Angular.

 For instance, we used the extension to generate a React component for creating a meeting schedule based on an API endpoint created using Python's FastAPI:

![ChatGPT extension component prompt](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/chatgpt-extension-component-prompt-1.jpg)

 As done above, you might want to check the **Ask Codebase** box if you're dealing with a large code base.

 After referencing our code base, the VS Code ChatGPT extension provided a handy React component to use the provided endpoint:

![Generated react component](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/generated-react-component.jpg)

## 5\. Explain Code Blocks

 Assume you grabbed a piece of code from Stack Overflow or a GitHub repository. You can ask the ChatGPT extension in VS Code to explain how it works for better comprehension. This helps you debug such code easily if bugs arise due to future code changes.

 In this example use case, we asked the ChatGPT extension to explain the following code; a Python class for verifying users' email addresses.

![Code to to explain example](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/code-to-to-explain-example.jpeg)

 It generated the following response:

![Code explained example output](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/code-explained-example-output.jpg)

<!-- affiliate ads begin -->
<span id="1982461">
					<video width="576" height="240" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1982461.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/22993-1982461">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1982461.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:360px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fhomestyler.sjv.io%2Fc%2F5597632%2F1982461%2F22993'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1982461/22993" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

## 6\. Generate HTML Templates for Your Application

 Using the ChatGPT extension in VS Code, you can create an HTML template (like input fields) from scratch—using the extension chat box directly. For instance, you can tell it to create an HTML template for user registration.

![User registration template example](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/user-registration-template-example.jpg)

 But what if you're writing an application that renders data into HTML directly (a non-SPA) and wants a project-specific template? You can use the ChatGPT extension in VS Code to create HTML templates that display the backend data to users.

 For instance, if you're using an [MVT architecture-based framework like Django](https://www.makeuseof.com/django-mvt-architecture/), you can use the extension to forge HTML templates for your Django views.

![Generated HMTL template example](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/generated-hmtl-template-example.jpg)

<!-- affiliate ads begin -->
<a href="https://wigfever.sjv.io/c/5597632/2014848/22899" target="_top" id="2014848">
  <img src="//a.impactradius-go.com/display-ad/22899-2014848" border="0" alt="https://techidaily.com" width="320" height="90"/>
</a>
<img height="0" width="0" src="https://wigfever.sjv.io/i/5597632/2014848/22899" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2123749/7443" target="_top" id="2123749">
  <img src="//a.impactradius-go.com/display-ad/7443-2123749" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2123749/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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

<!-- affiliate ads begin -->
<a href="https://unicoeye.pxf.io/c/5597632/2134491/18498" target="_top" id="2134491">
  <img src="//a.impactradius-go.com/display-ad/18498-2134491" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://unicoeye.pxf.io/i/5597632/2134491/18498" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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
<li><a href="https://facebook-clips.techidaily.com/new-in-2024-everything-about-facebook/"><u>[New] In 2024, Everything About Facebook</u></a></li>
<li><a href="https://screen-activity-recording.techidaily.com/new-mastery-in-stardew-navigating-the-intricacies-of-ginger-isle/"><u>[New] Mastery in Stardew Navigating the Intricacies of Ginger Isle</u></a></li>
<li><a href="https://youtube-web.techidaily.com/ed-in-2024-disciplined-device-use-effective-ways-to-remove-youtube-channels/"><u>[Updated] In 2024, Disciplined Device Use Effective Ways to Remove Youtube Channels</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/updated-swift-screen-tape-with-sound-included-for-2024/"><u>[Updated] Swift Screen Tape with Sound Included for 2024</u></a></li>
<li><a href="https://fox-access.techidaily.com/2024-approved-superior-screen-selection-top-10-picks/"><u>2024 Approved Superior Screen Selection – Top 10 Picks</u></a></li>
<li><a href="https://fox-cloud.techidaily.com/2024-approved-the-ultimate-guide-to-iphone-hdr-mastery/"><u>2024 Approved The Ultimate Guide to iPhone HDR Mastery</u></a></li>
<li><a href="https://win-amazing.techidaily.com/download-the-latest-thrustmaster-t300-steering-wheel-game-drivers-for-pcs-running-windows-1110/"><u>Download the Latest ThrustMaster T300 Steering Wheel Game Drivers for PCs Running Windows 11/10</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/easy-tips-and-tricks-for-successfully-securing-zdz-video-files-online/"><u>Easy Tips & Tricks for Successfully Securing ZDZ Video Files Online</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/easy-tutorial-on-downloading-and-converting-youtube-content-for-ios-devices/"><u>Easy Tutorial on Downloading & Converting YouTube Content for iOS Devices</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/effortless-guide-transforming-avi-files-into-xvid-compatible-format/"><u>Effortless Guide: Transforming AVI Files Into XVID-Compatible Format</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/effortlessly-change-your-videos-soundtrack-from-mp4-to-mp3-on-a-windows-machine/"><u>Effortlessly Change Your Video's Soundtrack From MP4 to MP3 on a Windows Machine</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/festive-fun-the-ultimate-list-of-kids-christmas-flicks/"><u>Festive Fun: The Ultimate List of Kids' Christmas Flicks</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/fixing-the-time-lag-in-handbrake-video-conversion-tips-and-tricks-for-perfect-audio-alignment/"><u>Fixing the Time Lag in HandBrake Video Conversion: Tips & Tricks for Perfect Audio Alignment</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/free-conference-call-ultimate-guide-to-recording-calls-without-fuss/"><u>Free Conference Call: Ultimate Guide to Recording Calls Without Fuss</u></a></li>
<li><a href="https://apple-account.techidaily.com/in-2024-3-ways-of-how-to-get-someones-apple-id-off-iphone-8-without-password-by-drfone-ios/"><u>In 2024, 3 Ways of How to Get Someones Apple ID Off iPhone 8 without Password</u></a></li>
</ul></div>

