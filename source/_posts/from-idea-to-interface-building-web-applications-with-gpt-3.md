---
title: "From Idea to Interface: Building Web Applications with GPT-3"
date: 2024-08-29T19:49:24.902Z
updated: 2024-08-30T19:49:24.902Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes From Idea to Interface: Building Web Applications with GPT-3"
excerpt: "This Article Describes From Idea to Interface: Building Web Applications with GPT-3"
thumbnail: https://thmb.techidaily.com/84dab43ab035d91cb56a4eae408b40758af9a9a2b096c95f61afee80ed15090c.jpg
---

## From Idea to Interface: Building Web Applications with GPT-3

 One of the biggest claims of the hype surrounding ChatGPT is that it can be an effective programming tool. The idea goes as follows: you describe what you want in natural language; the chatbot generates code that does just that. But how good actually is ChatGPT at doing this?

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 What better way to find out than putting it to the test? We asked ChatGPT to build a simple web app from scratch. Here's the result of our test and the steps you can use to build a website from scratch using ChatGPT.

## Step 1: Generating the Blueprint for Your Web App

 Just like you'd do when building a web app with any tool, you'd need to lay out the blueprint of what you want your app to look like and the steps you'll need to build it before letting ChatGPT run the show.

 For our first task, we asked ChatGPT to develop a blueprint for a simple chat app. To do this, we described the requirements for our web app and then asked the chatbot to detail a plan for developing the app.

![ChatGPT prompt to develop blueprint for web app](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/chatgpt-prompt-to-develop-blueprint-for-web-app.jpg)

 After using the prompt above, here's the result we got:

![Flowchart or blueprint of web app developed by chatgpt](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/flowchart-or-blueprint-of-web-app-developed-by-chatgpt.jpg)

 You'd need to have the "Show Me" plugin enabled on your ChatGPT account to generate a flowchart like ours above. You can [install and use ChatGPT plugins](https://www.makeuseof.com/how-install-and-use-chatgpt-plugins/) in just a few steps, although you will need a premium subscription.

 Without the plugin, you'll get a text-based blueprint or an ASCII-art flowchart. That's still okay. Even without the plugin, ChatGPT should still provide a clear blueprint of the app like the example below.

![text-based breakdown of web app by ChatGPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/text-based-breakdown-of-web-app-by-chatgpt.jpg)

## Step 2: Splitting the Blueprint Into Smaller Modules

 Now that we have the big picture laid out, we asked ChatGPT for help in splitting the app into smaller components that we can develop separately and then integrate to form the complete web app. ChatGPT suggested breaking it into three components:

1. Registration module
2. Login module
3. Chat module

 We had other ideas, but the goal here is to let ChatGPT call the shots.

### 1\. Building the Registration Component

 We jumped right into building the registration component. We asked ChatGPT to draw out an appropriate algorithm. Here we intervened by specifying we needed only the user's username, email, and avatar for registration. Here's the prompt:

![Prompt for building the registration component](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/prompt-for-building-the-registration-component.jpg)

 And here's the result:

![Algorithm for user registration](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/algorithm-for-user-registration.jpg)

 Up next, we prompted ChatGPT to build the registration component.

![prompt to generate the registration component](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/prompt-to-generate-the-registration-component-2.jpg)

 Although we didn't include the password field as part of the registration process, ChatGPT made the right call by including it in the generated HTML code. We copied the code without any modifications, and here's how it looks on a browser.

![Registration page generated by ChatGPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/registration-page-generated-by-chatgpt.jpg)

<!-- affiliate ads begin -->
<a href="https://shop.mondly.com/affiliate.php?ACCOUNT=ATISTUDI&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.mondly.com%3FAFFILIATE%3D108875%26RESOURCE%3D%2BGeneral%2B970x90%2B"><img src="https://secure.avangate.com/images/merchant/69c418c33ec2e1a4267fa9bb77fa1428/general-970x90.gif" border="0"></a>
<!-- affiliate ads end -->
 Up next, we prompted ChatGPT to generate the PHP registration script. At first, we prompted with "Write a PHP code for the server-side logic for handling the form submission." Although the generated script worked fine, it had a lot of vulnerabilities.

 There was no password hashing, no error handling, and was prone to SQL injection—ChatGPT did only the bare minimum. Fixing this was relatively easy. We simply asked ChatGPT to "identify everything wrong with the code you just generated, and then use the identified points to optimize the code." With that, our PHP registration script was ready to go.

 The wording of your prompt matters. You need to be very clear and specific with what you need ChatGPT to do. When we simply asked it to "fix the problem with this code," it didn't fix most of what we had hoped it would fix. For more guidance on writing ChatGPT prompts, here are [some places to learn how to write effective prompts](https://www.makeuseof.com/write-effective-chatgpt-prompts-for-ai-answers/).

 Up next, we asked ChatGPT to "**Write an SQL code to create a database for the data captured in the PHP script.**" Here's the resulting SQL code:

![Generated SQL code for the creating database by ChatGPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/06/generated-sql-code-for-the-creating-database-by-chatgpt.jpg)

 And here's the table created by executing the SQL:

![Database created by ChatGPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/06/database-created-by-chatgpt.jpg)

<!-- affiliate ads begin -->
<a href="https://estore.winxdvd.com/order/checkout.php?PRODS=12653808&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.winxdvd.com/affiliate/new-banner/wt-500x500.jpg" border="0"></a>
<!-- affiliate ads end -->
 With the database set up, we tried our first registration, and it worked without any errors.

<!-- affiliate ads begin -->
<a href="https://store.iobit.com/order/checkout.php?PRODS=1468905&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/184260348236f9554fe9375772ff966e/ascscan_728x90.png" border="0"></a>
<!-- affiliate ads end -->
### 2\. Building the Login Component

 With the registration component out of the way, we took on the Login component. Surprisingly, it was the easiest to build despite the additional logic of session management.

![Prompt to generate login script](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/06/prompt-to-generate-login-script.jpg)

 Here's the generated login page. A key highlight is that it uses the same color options as the registration page.

![ChatGPT-generated login page](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/06/chatgpt-generated-login-page.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=3727260&QTY=1&AFFILIATE=108875&CART=1"><img src="http://www.aiseesoft.com/avangate/30p/banner.jpg" border="0"></a>
<!-- affiliate ads end -->
 After creating a "server.login.php" file as instructed by ChatGPT and adding the generated PHP script, we made our first successful login without any modifications or debugging.

<!-- affiliate ads begin -->
<a href="https://boody-eco-wear.pxf.io/c/5597632/1567905/13846" target="_top" id="1567905"><img src="//a.impactradius-go.com/display-ad/13846-1567905" border="0" alt="" width="300" height="250"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1567905/13846" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
### 3\. Building the Chat Component

 Building the chat component was the final—and probably toughest part—of our little experiment. At first, we simply asked ChatGPT to write out the code for the chat component. Needless to say, it was a colossal failure. For more complex components of anything you want to create, you'll need to split it up into smaller components and tackle them one after another.

 We asked ChatGPT for suggestions on splitting up the chat component, and it suggested we create three pages:

1. Chat.php
2. Send-messages.php
3. Fetch-messages.php

 When ChatGPT suggests a file name, using a different name in your project might inadvertently cause problems as the chatbot will reference the same name in all the code it creates throughout the project. We found out the hard way. Don't make the same mistake.

### Creating the Chat.php Page

 To start, we gave ChatGPT detailed instructions on how we wanted the chat interface to look.

![ChatGPT prompt to generate HTML for the Chat interface](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/06/chatgpt-prompt-to-generate-html-for-the-chat-interface.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4550420&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.pearlmountainsoft.com/n_img/product/pic/f_02.jpg" border="0">PearlMountain Image Converter</a>
<!-- affiliate ads end -->
 After running the generated HTML code, we had a chat interface without a message input box. To fix this, we simply prompted ChatGPT to "**rewrite the code to include a message input box and a send button.**" Here's how the generated code looks on a browser on the second trial.

![sample chat interface generated by ChatGPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/06/sample-chat-interface-generated-by-chatgpt.jpg)

 Whenever generated code fails to give the desired results or omits an important component, simply prompt ChatGPT to rewrite the last code. Tell it to include the component or do whatever wasn't done in the initial code. Here are [some tips on how to use ChatGPT for programming](https://www.makeuseof.com/chatgpt-programming-practical-uses/).

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2082538/7443" target="_top" id="2082538"><img src="//a.impactradius-go.com/display-ad/7443-2082538" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2082538/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
### Creating the "send-messages.php" and "Fetch-messages" Page

 Satisfied with the interface, we proceeded to build the script to handle the chatting logic. To be able to send and fetch messages from the database, ChatGPT rightly highlighted that we'll be needing a "messages" table. We asked the chatbot to create an SQL for the messages table.

![SQL to create chat messages table](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/06/sql-to-create-chat-messages-table.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4940312&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/333ac5d90817d69113471fbb6e531bee/sps-partnership-728x90eng.png" border="0"></a>
<!-- affiliate ads end -->
 After generating an SQL code, we asked the chatbot to generate a PHP script to handle the messaging logic.

![ChatGPT prompts to send and receive messages](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/06/chatgpt-prompts-to-send-and-receive-messages.jpg)

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4693127&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.videosoftdev.com/images/video_editor/screenshots/1.jpg" border="0">
VSDC Pro Video Editor is a light professional non-linear video editing suite for creating a movie of any complexity. It supports the most popular video/audio formats and codecs, including 4K, HD and GoPro videos. Preconfigured profiles make the creation of videos for various multimedia and mobile devices absolutely hassle-free.

Key features:

•	Import from any devices and cams, including GoPro and drones. All formats supported. Сurrently the only free video editor that allows users to export in a new H265/HEVC codec, something essential for those working with 4K and HD.
•	Everything for hassle-free basic editing: cut, crop and merge files, add titles and favorite music
•	Visual effects, advanced color correction and trendy Instagram-like filters   
•	All multimedia processing done from one app: video editing capabilities reinforced by  a video converter, a screen capture, a video capture, a disc burner and a YouTube uploader
•	Non-linear editing: edit several files with simultaneously 
•	Easy export to social networks: special profiles for YouTube, Facebook, Vimeo, Twitter and Instagram
•	High quality export – no conversion quality loss, double export speed even of HD files due to hardware acceleration
•	Stabilization tool will turn shaky or jittery footage into a more stable video automatically. 
•	Essential toolset for professional video editing: blending modes, Mask tool, advanced multiple-color Chroma Key  
</a>
<!-- affiliate ads end -->
 ChatGPT generated the script for both the "send-messages.php" and the "fetch-messages.php" pages. On running both scripts, we finally had our very first error (which was oddly satisfying). Getting this far into the project without debugging a single line of code seemed a bit too good to be true, despite its relative simplicity.

 It turns out the error was caused by ChatGPT introducing a check for an undeclared session variable (**$\_SESSION\['user\_id'\]**) into our script. We suspect this was a result of taking a rather long break from the project resulting in ChatGPT forgetting some of the contexts and names of the variables used in the project.

 When using ChatGPT to build an app, ensure to use the same chat thread and try to complete related components as soon as possible. Using a new chat thread or taking a long break might introduce inconsistencies. ChatGPT tends to forget some details of the current project (e.g. the color scheme) if you take long breaks between coding sessions.

 That said, we fixed the bug and deployed the code. We registered, logged in, and tried the chat feature. While we were able to send messages from one registered user to another, the color and arrangement of the message bubbles were a bit off. However, for an app that took an hour and 23 minutes to complete, we won't judge it too harshly.

## ChatGPT: An Excellent Coding Assistant

 ChatGPT is clearly a powerful coding assistant. That the chatbot can turn up impressive code from simple, and sometimes not-so-clear, instructions is a testament to its coding prowess.

 Sure, it still has a lot of flaws. The issue with a limited context window and its ability to tie together the logic from multiple independently built components is a major problem. However, the chatbot can help you build fairly complex web apps rapidly if you know your way around.

**SCROLL TO CONTINUE WITH CONTENT**

 What better way to find out than putting it to the test? We asked ChatGPT to build a simple web app from scratch. Here's the result of our test and the steps you can use to build a website from scratch using ChatGPT.

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


