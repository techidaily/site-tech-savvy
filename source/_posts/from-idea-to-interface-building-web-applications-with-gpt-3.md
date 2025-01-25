---
title: "From Idea to Interface: Building Web Applications with GPT-3"
date: 2025-01-21T00:17:58.937Z
updated: 2025-01-24T20:12:15.569Z
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

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/n4cc4BSqJls?si=Hkd9vwQDqeCGN7XG" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/zXUt81WsQpI?si=W3DKIAsa2-qbGadJ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## Step 2: Splitting the Blueprint Into Smaller Modules

 Now that we have the big picture laid out, we asked ChatGPT for help in splitting the app into smaller components that we can develop separately and then integrate to form the complete web app. ChatGPT suggested breaking it into three components:

1. Registration module
2. Login module
3. Chat module

 We had other ideas, but the goal here is to let ChatGPT call the shots.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/0OxkndZbIA4?si=TWJlkTbYKsVag8-q" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

### 1\. Building the Registration Component

 We jumped right into building the registration component. We asked ChatGPT to draw out an appropriate algorithm. Here we intervened by specifying we needed only the user's username, email, and avatar for registration. Here's the prompt:

![Prompt for building the registration component](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/prompt-for-building-the-registration-component.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/vFQCEZiYA08?si=xjIu5IAy77RlHWii" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 And here's the result:

![Algorithm for user registration](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/algorithm-for-user-registration.jpg)

 Up next, we prompted ChatGPT to build the registration component.

![prompt to generate the registration component](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/prompt-to-generate-the-registration-component-2.jpg)

 Although we didn't include the password field as part of the registration process, ChatGPT made the right call by including it in the generated HTML code. We copied the code without any modifications, and here's how it looks on a browser.

![Registration page generated by ChatGPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/registration-page-generated-by-chatgpt.jpg)

 Up next, we prompted ChatGPT to generate the PHP registration script. At first, we prompted with "Write a PHP code for the server-side logic for handling the form submission." Although the generated script worked fine, it had a lot of vulnerabilities.

 There was no password hashing, no error handling, and was prone to SQL injection—ChatGPT did only the bare minimum. Fixing this was relatively easy. We simply asked ChatGPT to "identify everything wrong with the code you just generated, and then use the identified points to optimize the code." With that, our PHP registration script was ready to go.

 The wording of your prompt matters. You need to be very clear and specific with what you need ChatGPT to do. When we simply asked it to "fix the problem with this code," it didn't fix most of what we had hoped it would fix. For more guidance on writing ChatGPT prompts, here are [some places to learn how to write effective prompts](https://www.makeuseof.com/write-effective-chatgpt-prompts-for-ai-answers/).

 Up next, we asked ChatGPT to "**Write an SQL code to create a database for the data captured in the PHP script.**" Here's the resulting SQL code:

![Generated SQL code for the creating database by ChatGPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/06/generated-sql-code-for-the-creating-database-by-chatgpt.jpg)

 And here's the table created by executing the SQL:

![Database created by ChatGPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/06/database-created-by-chatgpt.jpg)

 With the database set up, we tried our first registration, and it worked without any errors.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/M5pwd2mwaQQ?si=qyZHgdTlbQbc32Mp" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

### 2\. Building the Login Component

 With the registration component out of the way, we took on the Login component. Surprisingly, it was the easiest to build despite the additional logic of session management.

![Prompt to generate login script](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/06/prompt-to-generate-login-script.jpg)

 Here's the generated login page. A key highlight is that it uses the same color options as the registration page.

![ChatGPT-generated login page](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/06/chatgpt-generated-login-page.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/LlYIdWQc-jw?si=ZQ5809CbQGEar0vg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 After creating a "server.login.php" file as instructed by ChatGPT and adding the generated PHP script, we made our first successful login without any modifications or debugging.

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

 After running the generated HTML code, we had a chat interface without a message input box. To fix this, we simply prompted ChatGPT to "**rewrite the code to include a message input box and a send button.**" Here's how the generated code looks on a browser on the second trial.

![sample chat interface generated by ChatGPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/06/sample-chat-interface-generated-by-chatgpt.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/PUDdKOsEN74?si=tkZf-KVinjuwmgx9" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Whenever generated code fails to give the desired results or omits an important component, simply prompt ChatGPT to rewrite the last code. Tell it to include the component or do whatever wasn't done in the initial code. Here are [some tips on how to use ChatGPT for programming](https://www.makeuseof.com/chatgpt-programming-practical-uses/).

### Creating the "send-messages.php" and "Fetch-messages" Page

 Satisfied with the interface, we proceeded to build the script to handle the chatting logic. To be able to send and fetch messages from the database, ChatGPT rightly highlighted that we'll be needing a "messages" table. We asked the chatbot to create an SQL for the messages table.

![SQL to create chat messages table](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/06/sql-to-create-chat-messages-table.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/qfCSLAhd4FY?si=CUBztmilaeAwl1lw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 After generating an SQL code, we asked the chatbot to generate a PHP script to handle the messaging logic.

![ChatGPT prompts to send and receive messages](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/06/chatgpt-prompts-to-send-and-receive-messages.jpg)

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

<span class="atpl-alsoreadstyle">Also read:</span>
<div><ul>
<li><a href="https://instagram-clips.techidaily.com/new-2024-approved-instagrams-mirage-identifying-false-friends-at-no-price/"><u>[New] 2024 Approved Instagram's Mirage Identifying False Friends at No Price</u></a></li>
<li><a href="https://youtube-data.techidaily.com/ed-icon-and-logo-inspiration-the-top-6-website-roundup/"><u>[Updated] Icon & Logo Inspiration The Top 6 Website Roundup</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/updated-in-2024-live-stream-perfection-an-experts-take-on-webcams/"><u>[Updated] In 2024, Live Stream Perfection An Expert's Take on WebCams</u></a></li>
<li><a href="https://some-skills.techidaily.com/2024-approved-transform-your-podcast-with-these-google-upload-insights/"><u>2024 Approved Transform Your Podcast with These Google Upload Insights</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/anker-bluetooth-speaker-review-high-quality-sound-at-surprisingly-low-prices-according-to-zdnet/"><u>Anker Bluetooth Speaker Review: High-Quality Sound at Surprisingly Low Prices, According to ZDNet</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/discover-why-philips-fidelio-fb1-soundbar-is-a-must-have-for-serious-music-lovers-as-recommended-by-zdnet/"><u>Discover Why Philips Fidelio FB1 Soundbar Is a Must-Have for Serious Music Lovers, as Recommended by ZDNet</u></a></li>
<li><a href="https://mondly-stories.techidaily.com/engage-anytime-anywhere-mondly-and-huawei/"><u>Engage Anytime, Anywhere - Mondly and Huawei</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/enhanced-sonos-roam/"><u>Enhanced Sonos Roam</u></a></li>
<li><a href="https://hardware-updates.techidaily.com/1722974374046-get-the-latest-canon-imageclass-mf4800-driver-software-for-free/"><u>Get the Latest Canon ImageCLASS MF4800 Driver Software for Free</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/grab-the-perfect-bluetooth-sound-companion-get-your-handheld-aqua-proof-jbl-charge-4-for-a-steal-at-just-89-on-black-friday-from-walmart/"><u>Grab the Perfect Bluetooth Sound Companion! Get Your Handheld, Aqua-Proof JBL Charge 4 for a Steal at Just $89 on Black Friday From Walmart!</u></a></li>
<li><a href="https://program-issues.techidaily.com/magic-the-gathering-platform-troubleshoot-beating-the-black-screen-glitches-easily/"><u>Magic: The Gathering Platform TroubleShoot: Beating the Black Screen Glitches Easily</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/portable-handheld-bluetooth-speaker-powerful-sound-dynamics-in-a-palm-sized-package-techradar-review/"><u>Portable Handheld Bluetooth Speaker: Powerful Sound Dynamics in a Palm-Sized Package | TechRadar Review</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unbeatable-black-friday-offer-snag-the-durable-jbl-charge-nwireless-speaker-at-walmart-for-only-89-your-guide-to-top-savings/"><u>Unbeatable Black Friday Offer: Snag the Durable JBL Charge nWireless Speaker at Walmart for Only $89! - Your Guide to Top Savings</u></a></li>
<li><a href="https://fox-blue.techidaily.com/understanding-cropping-settings-in-digital-editors-for-2024/"><u>Understanding Cropping Settings in Digital Editors for 2024</u></a></li>
</ul></div>

