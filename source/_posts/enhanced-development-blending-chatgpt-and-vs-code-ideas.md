---
title: "Enhanced Development: Blending ChatGPT & VS Code Ideas"
date: 2024-10-02T02:59:59.029Z
updated: 2024-10-08T18:52:04.329Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Enhanced Development: Blending ChatGPT & VS Code Ideas"
excerpt: "This Article Describes Enhanced Development: Blending ChatGPT & VS Code Ideas"
thumbnail: https://thmb.techidaily.com/3826690fad2bdad4d7aa62bd8a31b6771b07791104399fd4c0b5ca08b831fc4c.jpg
---

## Enhanced Development: Blending ChatGPT & VS Code Ideas

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

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2123733/7443" target="_top" id="2123733">
  <img src="//a.impactradius-go.com/display-ad/7443-2123733" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2123733/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2135397/19272" target="_top" id="2135397">
  <img src="//a.impactradius-go.com/display-ad/19272-2135397" border="0" alt="https://techidaily.com" width="180" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135397/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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

## 4\. Generate a Frontend Component for Your API

 If you've written an API with different endpoints, you can ask the ChatGPT extension to provide a frontend component to consume it using a particular framework. This could be React, Vue, or Angular.

 For instance, we used the extension to generate a React component for creating a meeting schedule based on an API endpoint created using Python's FastAPI:

![ChatGPT extension component prompt](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/chatgpt-extension-component-prompt-1.jpg)

 As done above, you might want to check the **Ask Codebase** box if you're dealing with a large code base.

 After referencing our code base, the VS Code ChatGPT extension provided a handy React component to use the provided endpoint:

![Generated react component](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/generated-react-component.jpg)

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2135367/19272" target="_top" id="2135367">
  <img src="//a.impactradius-go.com/display-ad/19272-2135367" border="0" alt="https://techidaily.com" width="180" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135367/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

<!-- affiliate ads begin -->
<span id="1983471">
					<video width="576" height="240" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1983471.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/22993-1983471">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1983471.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:360px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fhomestyler.sjv.io%2Fc%2F5597632%2F1983471%2F22993'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1983471/22993" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

## 5\. Explain Code Blocks

 Assume you grabbed a piece of code from Stack Overflow or a GitHub repository. You can ask the ChatGPT extension in VS Code to explain how it works for better comprehension. This helps you debug such code easily if bugs arise due to future code changes.

 In this example use case, we asked the ChatGPT extension to explain the following code; a Python class for verifying users' email addresses.

![Code to to explain example](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/code-to-to-explain-example.jpeg)

 It generated the following response:

![Code explained example output](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/code-explained-example-output.jpg)

<!-- affiliate ads begin -->
<a href="https://bluettius.sjv.io/c/5597632/2139117/17108" target="_top" id="2139117">
  <img src="//a.impactradius-go.com/display-ad/17108-2139117" border="0" alt="https://techidaily.com" width="320" height="90"/>
</a>
<img height="0" width="0" src="https://bluettius.sjv.io/i/5597632/2139117/17108" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

## 6\. Generate HTML Templates for Your Application

 Using the ChatGPT extension in VS Code, you can create an HTML template (like input fields) from scratch—using the extension chat box directly. For instance, you can tell it to create an HTML template for user registration.

![User registration template example](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/user-registration-template-example.jpg)

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

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2144308/7443" target="_top" id="2144308">
  <img src="//a.impactradius-go.com/display-ad/7443-2144308" border="0" alt="https://techidaily.com" width="600" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2144308/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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

<!-- affiliate ads begin -->
<a href="https://imp.i357552.net/c/5597632/1006793/11832" target="_top" id="1006793">
  <img src="//a.impactradius-go.com/display-ad/11832-1006793" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://imp.i357552.net/i/5597632/1006793/11832" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

## 10\. Write Documentation Directly From VS Code

 You can write detailed documentation for a piece of code directly from VS Code with ease using the ChatGPT extension.

 For example, here's a detailed documentation of a Zoom link creation function (in HTML format) that we generated using the VS Code ChatGPT extension:

![Generated documentation example](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/generated-documentation-example.jpg)

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1948891/19272" target="_top" id="1948891">
  <img src="//a.impactradius-go.com/display-ad/19272-1948891" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1948891/19272" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://facebook-video-share.techidaily.com/new-8-best-youtube-video-promotion-services-real-for-2024/"><u>[New] 8 Best YouTube Video Promotion Services (Real) for 2024</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/updated-in-2024-discreetly-watch-instas-hidden-gems-here/"><u>[Updated] In 2024, Discreetly Watch Insta's Hidden Gems, Here</u></a></li>
<li><a href="https://screen-sharing-recording.techidaily.com/updated-professional-window-capturer-version-11-for-2024/"><u>[Updated] Professional Window Capturer - Version 11 for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1726225984690-mp4-movavi/"><u>「オンラインでも簡単！無料MP4への変換 - Movavi」</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/2024-approved-mac-windows-vmx-substitute/"><u>2024 Approved Mac-Windows VMX Substitute</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/conversion-sin-costo-de-videos-3gp-a-mkv-por-internet-utilizando-movavis-soluciones-digitales/"><u>Conversión Sin Costo De Vídeos 3GP a MKV Por Internet Utilizando Movavi's Soluciones Digitales</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/convertir-formatos-mka-al-formato-de-alta-fidelidad-flac-por-internet-sin-gastar-un-centimo-usando-el-servicio-gratuitamente-disponible-en-movavi/"><u>Convertir Formatos MKA Al Formato De Alta Fidelidad FLAC Por Internet Sin Gastar Un Céntimo, Usando El Servicio Gratuitamente Disponible en Movavi</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/guide-complet-comment-effectuer-une-capture-decran-sur-ordinateur-en-2024/"><u>Guide Complet: Comment Effectuer Une Capture D'Écran Sur Ordinateur en 2024</u></a></li>
<li><a href="https://change-location.techidaily.com/how-to-get-the-dragon-scale-and-evolution-enabled-pokemon-on-vivo-y100i-drfone-by-drfone-virtual-android/"><u>How to get the dragon scale and evolution-enabled pokemon On Vivo Y100i? | Dr.fone</u></a></li>
<li><a href="https://youtube-video-recordings.techidaily.com/in-2024-accelerating-engagement-with-optimized-youtube-video-speeds/"><u>In 2024, Accelerating Engagement with Optimized YouTube Video Speeds</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/optimize-your-videobewerking-with-movavi-suite-elite-software-solutions-from-a-bvba-company/"><u>Optimize Your Videobewerking with Movavi Suite: Elite Software Solutions From a BVBA Company</u></a></li>
<li><a href="https://youtube-webster.techidaily.com/ing-off-on-channel-titling-tips-from-experienced-filmmakers/"><u>Sounding Off on Channel Titling Tips From Experienced Filmmakers</u></a></li>
</ul></div>

