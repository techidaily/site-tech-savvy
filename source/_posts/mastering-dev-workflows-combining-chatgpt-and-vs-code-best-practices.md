---
title: "Mastering Dev Workflows: Combining ChatGPT & VS Code Best Practices"
date: 2024-09-02T20:41:12.871Z
updated: 2024-09-03T20:41:12.871Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Mastering Dev Workflows: Combining ChatGPT & VS Code Best Practices"
excerpt: "This Article Describes Mastering Dev Workflows: Combining ChatGPT & VS Code Best Practices"
thumbnail: https://thmb.techidaily.com/b92970fb02a09749baa6f2838ddd89dd174bd2bb3f33370dc3c96100a7eda776.jpg
---

## Mastering Dev Workflows: Combining ChatGPT & VS Code Best Practices

 You can be the boss of your tasks and boost your productivity when you learn to leverage the AI tools trooping out of research labs daily. VS Code features the ChatGPT extension to bring you an OpenAI-enabled coding environment.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 You can leverage ChatGPT's vast coding model to complete your projects more efficiently and quicker—right inside the IDE. Here are handy ways you can use ChatGPT with VS Code.

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

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2082526/7443" target="_top" id="2082526"><img src="//a.impactradius-go.com/display-ad/7443-2082526" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2082526/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 The generated code above is more modular and reusable.

## 2\. Debug Your Code

 If your code throws an error or doesn't work as it should, asking ChatGPT to debug it directly inside VS Code saves time.

 Although there's no built-in prompt for debugging, you can use the **Ask GPT** option to create a custom prompt to debug your code.

 We asked the ChatGPT extension to debug the code we used earlier. Not only did it debug. It explained it and generated the correct one, including its expected output.

![Debugged code output](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/debugged-code-output-1.jpg)

<!-- affiliate ads begin -->
<a href="https://estore.macxdvd.com/order/checkout.php?PRODS=4526659&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.macxdvd.com/affiliate/new-banner/vcp-500x500.jpg" border="0"></a>
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

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=19080710&QTY=1&AFFILIATE=108875&CART=1"><img src="https://smart-seo-tool.com/images/SmartSEOAuditorBox.png" border="0"></a>
<!-- affiliate ads end -->
<!-- affiliate ads begin -->
<a href="https://store.advancedwebranking.com/order/checkout.php?PRODS=4715051&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/14edc6ebfdae2e23bbed83d67f50e983/products/33_awr%20logo.png" border="0"></a>
<!-- affiliate ads end -->
## 4\. Generate a Frontend Component for Your API

 If you've written an API with different endpoints, you can ask the ChatGPT extension to provide a frontend component to consume it using a particular framework. This could be React, Vue, or Angular.

 For instance, we used the extension to generate a React component for creating a meeting schedule based on an API endpoint created using Python's FastAPI:

![ChatGPT extension component prompt](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/chatgpt-extension-component-prompt-1.jpg)

<!-- affiliate ads begin -->
<a href="https://store.bitdefender.com/affiliate.php?ACCOUNT=BITLATIN&AFFILIATE=108875&PATH=http%3A%2F%2Fwww.bitdefender.com%2Fbusiness%3FAFFILIATE%3D108875%26RESOURCE%3D30%2525%2BOff%2Ball%2BGravityZone%2BProducts"><img src="https://www.bitdefender.com/content/dam/bitdefender/business/campaign/1200X628.png" border="0"></a>
<!-- affiliate ads end -->
 As done above, you might want to check the **Ask Codebase** box if you're dealing with a large code base.

 After referencing our code base, the VS Code ChatGPT extension provided a handy React component to use the provided endpoint:

![Generated react component](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/generated-react-component.jpg)

## 5\. Explain Code Blocks

 Assume you grabbed a piece of code from Stack Overflow or a GitHub repository. You can ask the ChatGPT extension in VS Code to explain how it works for better comprehension. This helps you debug such code easily if bugs arise due to future code changes.

 In this example use case, we asked the ChatGPT extension to explain the following code; a Python class for verifying users' email addresses.

![Code to to explain example](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/code-to-to-explain-example.jpeg)

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=3727260&QTY=1&AFFILIATE=108875&CART=1"><img src="http://www.aiseesoft.com/avangate/30p/banner.jpg" border="0"></a>
<!-- affiliate ads end -->
 It generated the following response:

![Code explained example output](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/code-explained-example-output.jpg)

## 6\. Generate HTML Templates for Your Application

 Using the ChatGPT extension in VS Code, you can create an HTML template (like input fields) from scratch—using the extension chat box directly. For instance, you can tell it to create an HTML template for user registration.

![User registration template example](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/user-registration-template-example.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4709458&QTY=1&AFFILIATE=108875&CART=1"><img src="https://3d-kstudio.com/wp-content/uploads/2019/10/Project-Manager-version-3-1600x900-768x419.jpg" border="0">Project Manager - Asset Browser for 3Ds Max</a>
<!-- affiliate ads end -->
 But what if you're writing an application that renders data into HTML directly (a non-SPA) and wants a project-specific template? You can use the ChatGPT extension in VS Code to create HTML templates that display the backend data to users.

 For instance, if you're using an [MVT architecture-based framework like Django](https://www.makeuseof.com/django-mvt-architecture/), you can use the extension to forge HTML templates for your Django views.

![Generated HMTL template example](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/generated-hmtl-template-example.jpg)

<!-- affiliate ads begin -->
<a href="https://cowinaudio.pxf.io/c/5597632/1116855/13794" target="_top" id="1116855"><img src="//a.impactradius-go.com/display-ad/13794-1116855" border="0" alt="" width="767" height="285"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1116855/13794" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 Again, for this type of use case, you might want to click the **Ask Codebase** checkbox for ChatGPT to access your code base.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=37100474&QTY=1&AFFILIATE=108875&CART=1"><img src="https://awario.com/images/pages/index/img-leads-1280@1x.avif" border="0"></a>
<!-- affiliate ads end -->
## 7\. Unit-Test Your Code

 As essential as unit testing is, it can be a time consumer. You can leverage the VS Code ChatGPT extension to generate unit tests for your code and save valuable development time.

 Although the ChatGPT extension has a built-in prompt for generating unit tests, you might want to write a custom prompt using the **Ask Codebase** option for specificity and a better result.

 We asked ChatGPT to write a unit test for a registration endpoint created using Python's FastAPI:

![Unit test prompt](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/unit-test-prompt.jpg)

 It sampled the code base efficiently to generate the required unit test:

![Generated unit tests](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/generated-unit-tests.jpg)

<!-- affiliate ads begin -->
<a href="https://vapordna.pxf.io/c/5597632/1494880/17238" target="_top" id="1494880"><img src="//a.impactradius-go.com/display-ad/17238-1494880" border="0" alt="" width="728" height="90"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1494880/17238" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## 8\. Find Potential Security Vulnerabilities

 While it may not provide detailed security analysis, the VS Code ChatGPT extension can be a handy tool to quickly [check for security vulnerabilities in your application](https://www.makeuseof.com/find-web-application-vulnerabilities/) code base and save you time scanning manually.

![Security vulnerability prompt VS Code](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/security-vulnerability-prompt-vs-code.jpg)

<!-- affiliate ads begin -->
<a href="https://newchic.sjv.io/c/5597632/1659704/14420" target="_top" id="1659704"><img src="//a.impactradius-go.com/display-ad/14420-1659704" border="0" alt="" width="728" height="90"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1659704/14420" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 To allow ChatGPT to scan your code base, use the **Ask Codebase** option (click the extension icon and check the **Ask Codebase** box).

## 9\. Ask VS Code-Related Questions

 If you usually gamble your way around some old or [new VS Code features](http://www.makeuseof.com/new-features-in-vscode-v169/), feel free to ask your way around the IDE from the ChatGPT extension.

 For instance, you can ask the extension to recommend the best extensions for debugging a particular programming language.

![VS Code specific prompt](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/vs-code-specific-prompt.jpg)

 Or you can ask it a more technical question, like how to open VS Code from the command line.

![VS Code specific prompt technical](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/vs-code-specific-prompt-technical.jpg)

<!-- affiliate ads begin -->
<a href="https://store.nero.com/order/checkout.php?PRODS=42296740&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.nero.com/nero-com-wAssets/img/banners/2023/biu/Nero_BackItUp_Screen_2.webp" border="0"></a>
<!-- affiliate ads end -->
<!-- affiliate ads begin -->
<a href="https://imp.i357552.net/c/5597632/863039/11832" target="_top" id="863039"><img src="//a.impactradius-go.com/display-ad/11832-863039" border="0" alt="" width="300" height="250"/></a>
<!-- affiliate ads end -->
## 10\. Write Documentation Directly From VS Code

 You can write detailed documentation for a piece of code directly from VS Code with ease using the ChatGPT extension.

 For example, here's a detailed documentation of a Zoom link creation function (in HTML format) that we generated using the VS Code ChatGPT extension:

![Generated documentation example](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/generated-documentation-example.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4530091&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.pearlmountainsoft.com/n_img/product/cit_win/banScrn.jpg" border="0">CollageIt Pro</a>
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
<li><a href="https://remote-screen-capture.techidaily.com/new-nocturnal-nuances-essential-tips-for-moonlit-portraiture-for-2024/"><u>[New] Nocturnal Nuances  Essential Tips for Moonlit Portraiture for 2024</u></a></li>
<li><a href="https://video-capture.techidaily.com/updated-2024-approved-step-by-step-guide-to-zoom-call-recordings/"><u>[Updated] 2024 Approved  Step-by-Step Guide to Zoom Call Recordings</u></a></li>
<li><a href="https://on-screen-recording.techidaily.com/updated-capture-video-perfection-in-minutes/"><u>[Updated] Capture Video Perfection in Minutes</u></a></li>
<li><a href="https://screen-capture.techidaily.com/updated-in-2024-chasingpeakperformance-after-mycam/"><u>[Updated] In 2024, ChasingPeakPerformance After MyCam</u></a></li>
<li><a href="https://instagram-clips.techidaily.com/updated-instagram-fraud-busters-efficient-and-economical-methods-for-2024/"><u>[Updated] Instagram Fraud Busters  Efficient & Economical Methods for 2024</u></a></li>
<li><a href="https://extra-approaches.techidaily.com/updated-premier-filmmakers-digital-backdrop-changer/"><u>[Updated] Premier Filmmaker's Digital Backdrop Changer</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/2024-approved-curb-instagrams-auto-suggest-feature/"><u>2024 Approved  Curb Instagram's Auto-Suggest Feature</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/adaptive-language-learning-via-chatgpt-plus-interface/"><u>Adaptive Language Learning via ChatGPT Plus Interface</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-revolution-which-professions-might-be-abolished/"><u>AI Revolution: Which Professions Might Be Abolished?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/an-in-depth-look-at-claude-pros-differences-from-gptplusplus/"><u>An In-Depth Look at Claude Pro’s Differences From GPT++</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/augmenting-crypto-dialogues-gpts-top-8-integrative-tools-revealed/"><u>Augmenting Crypto Dialogues: GPT's Top 8 Integrative Tools Revealed</u></a></li>
<li><a href="https://unlock-android.techidaily.com/best-ways-on-how-to-unlockbypassswiperemove-xiaomi-14-ultra-fingerprint-lock-by-drfone-android/"><u>Best Ways on How to Unlock/Bypass/Swipe/Remove Xiaomi 14 Ultra Fingerprint Lock</u></a></li>
<li><a href="https://techtrends.techidaily.com/code-39-barcode-problems-in-windows-fixing-procedures/"><u>Code 39 Barcode Problems in Windows: Fixing Procedures</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/cyber-threat-alert-the-risky-side-of-google-bard-download/"><u>Cyber Threat Alert: The Risky Side of Google Bard Download</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/deciphering-codegpt-the-future-of-programming-with-ai/"><u>Deciphering CodeGPT: The Future of Programming with AI?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/dive-into-smooth-chatgpt-interactions-chrome-powered-solution/"><u>Dive Into Smooth ChatGPT Interactions - Chrome-Powered Solution</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/essential-tweaks-required-for-better-gpt-plugin-management/"><u>Essential Tweaks Required for Better GPT Plugin Management</u></a></li>
<li><a href="https://article-helps.techidaily.com/excellence-in-capturing-slow-motions-for-2024/"><u>Excellence in Capturing Slow Motions for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/fantasy-fused-with-fact-leading-ai-trajectories/"><u>Fantasy Fused with Fact: Leading AI Trajectories</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/fools-errand-of-intelligent-machines-recognizing-ai-hallucination/"><u>Fool's Errand of Intelligent Machines: Recognizing AI Hallucination</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/harnessing-gpts-potential-for-eq-improvement/"><u>Harnessing GPT's Potential for EQ Improvement</u></a></li>
<li><a href="https://android-transfer.techidaily.com/how-to-transfer-photos-from-nokia-xr21-to-samsung-galaxy-s21-ultra-drfone-by-drfone-transfer-from-android-transfer-from-android/"><u>How to Transfer Photos From Nokia XR21 to Samsung Galaxy S21 Ultra | Dr.fone</u></a></li>
<li><a href="https://article-knowledge.techidaily.com/in-2024-nows-vr-tech-landscape/"><u>In 2024, Now’s VR Tech Landscape</u></a></li>
<li><a href="https://screen-recording.techidaily.com/in-2024-securing-your-gaming-victories-through-fbx/"><u>In 2024, Securing Your Gaming Victories Through FBX</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/in-2024-top-11-free-apps-to-check-imei-on-samsung-galaxy-s24plus-phones-by-drfone-android/"><u>In 2024, Top 11 Free Apps to Check IMEI on Samsung Galaxy S24+ Phones</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-gpt-8-essential-methods/"><u>Mastering GPT: 8 Essential Methods</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/precision-in-patient-care-how-to-confirm-ai-health-advice/"><u>Precision in Patient Care: How to Confirm AI Health Advice</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/setting-standards-for-smart-systems/"><u>Setting Standards for Smart Systems</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/stop-matching-siri-with-chatgpt-their-uniqueness-spotlighted/"><u>Stop Matching Siri with ChatGPT: Their Uniqueness Spotlighted</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/sweet-success-crafting-ideal-cookie-consistency/"><u>Sweet Success: Crafting Ideal Cookie Consistency</u></a></li>
<li><a href="https://some-guidance.techidaily.com/the-guide-to-softening-volume-levels-on-lumafusion-for-2024/"><u>The Guide to Softening Volume Levels on Lumafusion for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-new-age-of-programming-with-ai/"><u>The New Age of Programming with AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-rise-of-virtual-therapy-top-5-bot-innovations/"><u>The Rise of Virtual Therapy: Top 5 Bot Innovations</u></a></li>
<li><a href="https://some-skills.techidaily.com/tips-for-shaping-images-with-photoshop-curves-for-2024/"><u>Tips for Shaping Images with Photoshop Curves for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/uncover-hidden-insights-power-of-perplexity-ai/"><u>Uncover Hidden Insights: Power of Perplexity AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unlocking-potential-with-local-vs-non-local-llm-models/"><u>Unlocking Potential with Local vs Non-Local LLM Models</u></a></li>
<li><a href="https://hardware-help.techidaily.com/1722977614305-update-your-canon-pixma-ts3222-direct-download-links-available-now/"><u>Update Your Canon PIXMA TS3222: Direct Download Links Available Now</u></a></li>
</ul></div>
