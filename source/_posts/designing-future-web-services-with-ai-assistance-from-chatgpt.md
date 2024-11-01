---
title: Designing Future Web Services with AI Assistance From ChatGPT
date: 2024-10-28T17:14:38.293Z
updated: 2024-11-01T16:20:20.791Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Designing Future Web Services with AI Assistance From ChatGPT
excerpt: This Article Describes Designing Future Web Services with AI Assistance From ChatGPT
thumbnail: https://thmb.techidaily.com/289107adae482c208effdc1eb510e9f1c669fd2ac79f6588ee6f56110294810a.jpg
---

## Designing Future Web Services with AI Assistance From ChatGPT

 One of the biggest claims of the hype surrounding ChatGPT is that it can be an effective programming tool. The idea goes as follows: you describe what you want in natural language; the chatbot generates code that does just that. But how good actually is ChatGPT at doing this?

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 What better way to find out than putting it to the test? We asked ChatGPT to build a simple web app from scratch. Here's the result of our test and the steps you can use to build a website from scratch using ChatGPT.

>  Disclaimer: This post includes affiliate links
>
>  If you click on a link and make a purchase, I may receive a commission at no extra cost to you.
>

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
<a href="https://aligracehair.sjv.io/c/5597632/1938698/19272" target="_top" id="1938698">
  <img src="//a.impactradius-go.com/display-ad/19272-1938698" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1938698/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

## Step 2: Splitting the Blueprint Into Smaller Modules

 Now that we have the big picture laid out, we asked ChatGPT for help in splitting the app into smaller components that we can develop separately and then integrate to form the complete web app. ChatGPT suggested breaking it into three components:

1. Registration module
2. Login module
3. Chat module

 We had other ideas, but the goal here is to let ChatGPT call the shots.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2037319/7443" target="_top" id="2037319">
  <img src="//a.impactradius-go.com/display-ad/7443-2037319" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2037319/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

### 1\. Building the Registration Component

 We jumped right into building the registration component. We asked ChatGPT to draw out an appropriate algorithm. Here we intervened by specifying we needed only the user's username, email, and avatar for registration. Here's the prompt:

![Prompt for building the registration component](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/prompt-for-building-the-registration-component.jpg)

 And here's the result:

![Algorithm for user registration](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/algorithm-for-user-registration.jpg)

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2037345/7443" target="_top" id="2037345">
  <img src="//a.impactradius-go.com/display-ad/7443-2037345" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2037345/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Up next, we prompted ChatGPT to build the registration component.

![prompt to generate the registration component](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/prompt-to-generate-the-registration-component-2.jpg)

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1934142/19272" target="_top" id="1934142">
  <img src="//a.impactradius-go.com/display-ad/19272-1934142" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1934142/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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

### 2\. Building the Login Component

 With the registration component out of the way, we took on the Login component. Surprisingly, it was the easiest to build despite the additional logic of session management.

![Prompt to generate login script](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/06/prompt-to-generate-login-script.jpg)

 Here's the generated login page. A key highlight is that it uses the same color options as the registration page.

![ChatGPT-generated login page](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/06/chatgpt-generated-login-page.jpg)

 After creating a "server.login.php" file as instructed by ChatGPT and adding the generated PHP script, we made our first successful login without any modifications or debugging.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1902273/19272" target="_top" id="1902273">
  <img src="//a.impactradius-go.com/display-ad/19272-1902273" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1902273/19272" style="position:absolute;visibility:hidden;" border="0" />
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

 After running the generated HTML code, we had a chat interface without a message input box. To fix this, we simply prompted ChatGPT to "**rewrite the code to include a message input box and a send button.**" Here's how the generated code looks on a browser on the second trial.

![sample chat interface generated by ChatGPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/06/sample-chat-interface-generated-by-chatgpt.jpg)

 Whenever generated code fails to give the desired results or omits an important component, simply prompt ChatGPT to rewrite the last code. Tell it to include the component or do whatever wasn't done in the initial code. Here are [some tips on how to use ChatGPT for programming](https://www.makeuseof.com/chatgpt-programming-practical-uses/).

### Creating the "send-messages.php" and "Fetch-messages" Page

 Satisfied with the interface, we proceeded to build the script to handle the chatting logic. To be able to send and fetch messages from the database, ChatGPT rightly highlighted that we'll be needing a "messages" table. We asked the chatbot to create an SQL for the messages table.

![SQL to create chat messages table](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/06/sql-to-create-chat-messages-table.jpg)

<!-- affiliate ads begin -->
<span id="1793213">
					<video width="864" height="1296" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1793213.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/19135-1793213">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1793213.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:540px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Ftinyland.pxf.io%2Fc%2F5597632%2F1793213%2F19135'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1793213/19135" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 After generating an SQL code, we asked the chatbot to generate a PHP script to handle the messaging logic.

![ChatGPT prompts to send and receive messages](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/06/chatgpt-prompts-to-send-and-receive-messages.jpg)

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2094419/7443" target="_top" id="2094419">
  <img src="//a.impactradius-go.com/display-ad/7443-2094419" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2094419/7443" style="position:absolute;visibility:hidden;" border="0" />
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

<span class="atpl-alsoreadstyle">Also read:</span>
<div><ul>
<li><a href="https://fox-blue.techidaily.com/new-2024-approved-instant-photographic-display-in-11-os/"><u>[New] 2024 Approved Instant Photographic Display in 11 OS</u></a></li>
<li><a href="https://fox-http.techidaily.com/new-high-end-streaming-gear-for-professionals-for-2024/"><u>[New] High-End Streaming Gear for Professionals for 2024</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/new-the-ultimate-path-to-igtv-popularity-top-strategies-unveiled/"><u>[New] The Ultimate Path to IGTV Popularity Top Strategies Unveiled</u></a></li>
<li><a href="https://youtube-lab.techidaily.com/he-video-gurus-playbook-smooth-transition-to-easy-youtube-cc-and-subtitles/"><u>[New] The Video Guru's Playbook Smooth Transition to Easy YouTube CC & Subtitles</u></a></li>
<li><a href="https://youtube-webster.techidaily.com/ed-boost-your-view-count-explore-these-12-effective-youtube-strategies-for-2024/"><u>[Updated] Boost Your View Count Explore These 12 Effective YouTube Strategies for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/iuoajomgupluse5geobquocteodsplusodlplusodqpluswhpueqhjog5zplus65pys44gl44kj5ael44kb44kl5zgo5roi5pww5asj5oplusb44gu44og44kv44ol44od44kv44ks44kk44oj44cnig/"><u>「頻繁なサンプル処理: 基本から始める周波数変換のテクニックガイド」</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-exclusive-discoveries-prime-websites-and-methods-to-download-tamil-ringtone-files/"><u>2024 Approved Exclusive Discoveries Prime Websites & Methods to Download Tamil Ringtone Files</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mkv3/"><u>完全無損失でMKVを切り分ける3方法：高画質維持のコツ</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/best-5-substitutes-for-screenflow-on-windows-and-macos-a-comprehensive-guide/"><u>Best 5 Substitutes for ScreenFlow on Windows and macOS: A Comprehensive Guide</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/easily-extract-and-save-animated-images-from-facebook-for-desktop-and-mobile-use/"><u>Easily Extract and Save Animated Images From Facebook for Desktop & Mobile Use</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/effortless-transfer-techniques-moving-the-dvd-film-interstellar-to-ios-devices/"><u>Effortless Transfer Techniques: Moving the DVD Film 'Interstellar' To iOS Devices</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/effortlessly-edit-your-tracks-length-in-itunes-a-simple-step-by-step-guide/"><u>Effortlessly Edit Your Track's Length in iTunes: A Simple Step-by-Step Guide</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/frozen-ground-ripped-apart-from-prey-to-predator-unleashed/"><u>Frozen Ground Ripped Apart: From Prey to Predator Unleashed</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-download-audiocasts-without-paying-tips-for-extracting-sound-from-social-media-clips/"><u>How to Download Audiocasts without Paying: Tips for Extracting Sound From Social Media Clips</u></a></li>
<li><a href="https://ios-unlock.techidaily.com/in-2024-complete-guide-for-iphone-11-lock-screen-by-drfone-ios/"><u>In 2024, Complete Guide For iPhone 11 Lock Screen</u></a></li>
<li><a href="https://audio-shaping.techidaily.com/new-efficient-mp3-dividing-techniques-mastering-audio-splitting-speedily/"><u>New Efficient MP3 Dividing Techniques Mastering Audio Splitting Speedily</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/simple-solutions-to-overcome-vlcs-cfhd-codec-error-and-ensure-smooth-playback/"><u>Simple Solutions to Overcome VLC's CFHD Codec Error and Ensure Smooth Playback</u></a></li>
<li><a href="https://extra-tips.techidaily.com/the-comprehensive-guide-to-editing-hauls-for-online-audiences/"><u>The Comprehensive Guide to Editing Hauls for Online Audiences</u></a></li>
<li><a href="https://fox-that.techidaily.com/what-you-need-to-know-about-retrieving-lost-notes-from-your-iphone/"><u>What You Need to Know About Retrieving Lost Notes From Your iPhone</u></a></li>
</ul></div>

