---
title: Keeping Secrets Safe in Custom GPT Environments
date: 2024-10-09T12:14:16.257Z
updated: 2024-10-14T16:31:32.597Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Keeping Secrets Safe in Custom GPT Environments
excerpt: This Article Describes Keeping Secrets Safe in Custom GPT Environments
thumbnail: https://thmb.techidaily.com/d6473782f31868e794fc3ab8460fc67b139be82f000417effd74e9124ff9dff3.jpg
---

## Keeping Secrets Safe in Custom GPT Environments

>  Disclaimer: This post includes affiliate links
>
>  If you click on a link and make a purchase, I may receive a commission at no extra cost to you.
>

### Key Takeaways

* Custom GPTs allow you to create personalized AI tools for various purposes and share them with others, amplifying expertise in specific areas.
* However, sharing your custom GPTs can expose your data to a global audience, potentially compromising privacy and security.
* To protect your data, be cautious when sharing custom GPTs and avoid uploading sensitive materials. Be mindful of prompt engineering and be wary of malicious links that could access and steal your files.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 ChatGPT's custom GPT feature allows anyone to create a custom AI tool for almost anything you can think of; creative, technical, gaming, custom GPTs can do it all. Better still, you can share your custom GPT creations with anyone.

 However, by sharing your custom GPTs, you could be making a costly mistake that exposes your data to thousands of people globally.

<!-- affiliate ads begin -->
<span id="2135472">
					<video width="864" height="1536" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/2135472.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/18498-2135472">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/2135472.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:540px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Funicoeye.pxf.io%2Fc%2F5597632%2F2135472%2F18498'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/2135472/18498" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

## What Are Custom GPTs?

[Custom GPTs are programmable mini versions of ChatGPT](https://www.makeuseof.com/how-use-chatgpt-my-gpt-bots/) that can be trained to be more helpful on specific tasks. It is like molding ChatGPT into a chatbot that behaves the way you want and teaching it to become an expert in fields that really matter to you.

 For instance, a Grade 6 teacher could build a GPT that specializes in answering questions with a tone, word choice, and mannerism that is suitable for Grade 6 students. The GPT could be programmed such that whenever the teacher asks the GPT a question, the chatbot will formulate responses that speak directly to a 6th grader's level of understanding. It would avoid complex terminology, keep sentence length manageable, and adopt an encouraging tone. The allure of Custom GPTs is the ability to personalize the chatbot in this manner while also amplifying its expertise in certain areas.

## How Custom GPTs Can Expose Your Data

 To [create Custom GPTs](https://www.makeuseof.com/how-use-create-a-gpt-to-create-a-customized-version-of-chatgpt/), you typically instruct ChatGPT’s GPT creator on which areas you want the GPT to focus on, give it a profile picture, then a name, and you're ready to go. Using this approach, you get a GPT, but it doesn't make it any significantly better than classic ChatGPT without the fancy name and profile picture.

 The power of Custom GPT comes from the specific data and instructions provided to train it. By uploading relevant files and datasets, the model can become specialized in ways that broad pre-trained classic ChatGPT cannot. The knowledge contained in those uploaded files allows a Custom GPT to excel at certain tasks compared to ChatGPT, which may not have access to that specialized information. Ultimately, it is the custom data that enables greater capability.

 But uploading files to improve your GPT is a double-edged sword. It creates a privacy problem just as much as it boosts your GPT’s capabilities. Consider a scenario where you created a GPT to help customers learn more about you or your company. Anyone who has a link to your Custom GPT or somehow gets you to use a public prompt with a malicious link can access the files you've uploaded to your GPT.

 Here’s a simple illustration.

 I discovered a Custom GPT supposed to help users go viral on TikTok by recommending trending hashtags and topics. After the Custom GPT, it took little to no effort to get it to leak the instructions it was given when it was set up. Here's a sneak peek:

![Prompting a Custom GPT to leak its instructions](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/prompting-a-custom-gpt-to-leak-its-instructions.jpg)

 And here's the second part of the instruction.

![Prompting a Custom GPT to leak its instructions 2](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/prompting-a-custom-gpt-to-leak-its-instructions-2.jpg)

<!-- affiliate ads begin -->
<a href="https://25home.pxf.io/c/5597632/2148634/16836" target="_top" id="2148634">
  <img src="//a.impactradius-go.com/display-ad/16836-2148634" border="0" alt="https://techidaily.com" width="80" height="31"/>
</a>
<img height="0" width="0" src="https://25home.pxf.io/i/5597632/2148634/16836" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 If you look closely, the second part of the instruction tells the model not to "share the names of the files directly with end users and under no circumstances should you provide a download link to any of the files." Of course, if you ask the custom GPT at first, it refuses, but with a little bit of prompt engineering, that changes. The custom GPT reveals the lone text file in its knowledge base.

![files in knowledge base-1](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/files-in-knowledge-base-1.jpg)

 With the file name, it took little effort to get the GPT to print the exact content of the file and subsequently download the file itself. In this case, the actual file wasn't sensitive. After poking around a few more GPTs, there were a lot with dozens of files sitting in the open.

![files in knowledge base2](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/files-in-knowledge-base2.jpg)

<!-- affiliate ads begin -->
<span id="1982570">
					<video width="576" height="240" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1982570.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/22993-1982570">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1982570.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:360px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fhomestyler.sjv.io%2Fc%2F5597632%2F1982570%2F22993'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1982570/22993" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 There are hundreds of publicly available GPTs out there that contain sensitive files that are just sitting there waiting for malicious actors to grab.

## How to Protect Your Custom GPT Data

![chatgpt custom gpt share and publish options](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/chatgpt-custom-gpt-share-and-publish-options.jpg)

 First, consider how you will share (or not!) the custom GPT you just created. In the top-right corner of the custom GPT creation screen, you'll find the **Save** button. Press the dropdown arrow icon, and from here, select how you want to share your creation:

* **Only me**: The custom GPT is not published and is only usable by you
* **Only people with a link:** Any one with the link to your custom GPT can use it and potentially access your data
* **Public:** Your custom GPT is available to anyone and can be indexed by Google and found in general internet searches. Anyone with access could potentially access your data.

 Unfortunately, there's currently no 100 percent foolproof way to protect the data you upload to a custom GPT that is shared publicly. You can get creative and give it strict instructions not to reveal the data in its knowledge base, but that's usually not enough, as our demonstration above has shown. If someone really wants to gain access to the knowledge base and has experience with AI prompt engineering and some time, eventually, the custom GPT will break and reveal the data.

 This is why the safest bet is not to upload any sensitive materials to a custom GPT you intend to share with the public. Once you upload private and sensitive data to a custom GPT and it leaves your computer, that data is effectively out of your control.

 Also, be very careful when using prompts you copy online. Make sure you understand them thoroughly and avoid obfuscated prompts that contain links. These could be malicious links that hijack, encode, and upload your files to remote servers.

## Use Custom GPTs with Caution

 Custom GPTs are a powerful but potentially risky feature. While they allow you to create customized models that are highly capable in specific domains, the data you use to enhance their abilities can be exposed. To mitigate risk, avoid uploading truly sensitive data to your Custom GPTs whenever possible. Additionally, be wary of malicious prompt engineering that can exploit certain loopholes to steal your files.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 ChatGPT's custom GPT feature allows anyone to create a custom AI tool for almost anything you can think of; creative, technical, gaming, custom GPTs can do it all. Better still, you can share your custom GPT creations with anyone.

 However, by sharing your custom GPTs, you could be making a costly mistake that exposes your data to thousands of people globally.

## What Are Custom GPTs?

[Custom GPTs are programmable mini versions of ChatGPT](https://www.makeuseof.com/how-use-chatgpt-my-gpt-bots/) that can be trained to be more helpful on specific tasks. It is like molding ChatGPT into a chatbot that behaves the way you want and teaching it to become an expert in fields that really matter to you.

 For instance, a Grade 6 teacher could build a GPT that specializes in answering questions with a tone, word choice, and mannerism that is suitable for Grade 6 students. The GPT could be programmed such that whenever the teacher asks the GPT a question, the chatbot will formulate responses that speak directly to a 6th grader's level of understanding. It would avoid complex terminology, keep sentence length manageable, and adopt an encouraging tone. The allure of Custom GPTs is the ability to personalize the chatbot in this manner while also amplifying its expertise in certain areas.

## How Custom GPTs Can Expose Your Data

 To [create Custom GPTs](https://www.makeuseof.com/how-use-create-a-gpt-to-create-a-customized-version-of-chatgpt/), you typically instruct ChatGPT’s GPT creator on which areas you want the GPT to focus on, give it a profile picture, then a name, and you're ready to go. Using this approach, you get a GPT, but it doesn't make it any significantly better than classic ChatGPT without the fancy name and profile picture.

 The power of Custom GPT comes from the specific data and instructions provided to train it. By uploading relevant files and datasets, the model can become specialized in ways that broad pre-trained classic ChatGPT cannot. The knowledge contained in those uploaded files allows a Custom GPT to excel at certain tasks compared to ChatGPT, which may not have access to that specialized information. Ultimately, it is the custom data that enables greater capability.

 But uploading files to improve your GPT is a double-edged sword. It creates a privacy problem just as much as it boosts your GPT’s capabilities. Consider a scenario where you created a GPT to help customers learn more about you or your company. Anyone who has a link to your Custom GPT or somehow gets you to use a public prompt with a malicious link can access the files you've uploaded to your GPT.

 Here’s a simple illustration.

 I discovered a Custom GPT supposed to help users go viral on TikTok by recommending trending hashtags and topics. After the Custom GPT, it took little to no effort to get it to leak the instructions it was given when it was set up. Here's a sneak peek:

![Prompting a Custom GPT to leak its instructions](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/prompting-a-custom-gpt-to-leak-its-instructions.jpg)

 And here's the second part of the instruction.

![Prompting a Custom GPT to leak its instructions 2](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/prompting-a-custom-gpt-to-leak-its-instructions-2.jpg)

 If you look closely, the second part of the instruction tells the model not to "share the names of the files directly with end users and under no circumstances should you provide a download link to any of the files." Of course, if you ask the custom GPT at first, it refuses, but with a little bit of prompt engineering, that changes. The custom GPT reveals the lone text file in its knowledge base.

![files in knowledge base-1](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/files-in-knowledge-base-1.jpg)

 With the file name, it took little effort to get the GPT to print the exact content of the file and subsequently download the file itself. In this case, the actual file wasn't sensitive. After poking around a few more GPTs, there were a lot with dozens of files sitting in the open.

![files in knowledge base2](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/files-in-knowledge-base2.jpg)

 There are hundreds of publicly available GPTs out there that contain sensitive files that are just sitting there waiting for malicious actors to grab.

## How to Protect Your Custom GPT Data

![chatgpt custom gpt share and publish options](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/chatgpt-custom-gpt-share-and-publish-options.jpg)

 First, consider how you will share (or not!) the custom GPT you just created. In the top-right corner of the custom GPT creation screen, you'll find the **Save** button. Press the dropdown arrow icon, and from here, select how you want to share your creation:

* **Only me**: The custom GPT is not published and is only usable by you
* **Only people with a link:** Any one with the link to your custom GPT can use it and potentially access your data
* **Public:** Your custom GPT is available to anyone and can be indexed by Google and found in general internet searches. Anyone with access could potentially access your data.

 Unfortunately, there's currently no 100 percent foolproof way to protect the data you upload to a custom GPT that is shared publicly. You can get creative and give it strict instructions not to reveal the data in its knowledge base, but that's usually not enough, as our demonstration above has shown. If someone really wants to gain access to the knowledge base and has experience with AI prompt engineering and some time, eventually, the custom GPT will break and reveal the data.

 This is why the safest bet is not to upload any sensitive materials to a custom GPT you intend to share with the public. Once you upload private and sensitive data to a custom GPT and it leaves your computer, that data is effectively out of your control.

 Also, be very careful when using prompts you copy online. Make sure you understand them thoroughly and avoid obfuscated prompts that contain links. These could be malicious links that hijack, encode, and upload your files to remote servers.

## Use Custom GPTs with Caution

 Custom GPTs are a powerful but potentially risky feature. While they allow you to create customized models that are highly capable in specific domains, the data you use to enhance their abilities can be exposed. To mitigate risk, avoid uploading truly sensitive data to your Custom GPTs whenever possible. Additionally, be wary of malicious prompt engineering that can exploit certain loopholes to steal your files.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 ChatGPT's custom GPT feature allows anyone to create a custom AI tool for almost anything you can think of; creative, technical, gaming, custom GPTs can do it all. Better still, you can share your custom GPT creations with anyone.

 However, by sharing your custom GPTs, you could be making a costly mistake that exposes your data to thousands of people globally.

## What Are Custom GPTs?

[Custom GPTs are programmable mini versions of ChatGPT](https://www.makeuseof.com/how-use-chatgpt-my-gpt-bots/) that can be trained to be more helpful on specific tasks. It is like molding ChatGPT into a chatbot that behaves the way you want and teaching it to become an expert in fields that really matter to you.

 For instance, a Grade 6 teacher could build a GPT that specializes in answering questions with a tone, word choice, and mannerism that is suitable for Grade 6 students. The GPT could be programmed such that whenever the teacher asks the GPT a question, the chatbot will formulate responses that speak directly to a 6th grader's level of understanding. It would avoid complex terminology, keep sentence length manageable, and adopt an encouraging tone. The allure of Custom GPTs is the ability to personalize the chatbot in this manner while also amplifying its expertise in certain areas.

## How Custom GPTs Can Expose Your Data

 To [create Custom GPTs](https://www.makeuseof.com/how-use-create-a-gpt-to-create-a-customized-version-of-chatgpt/), you typically instruct ChatGPT’s GPT creator on which areas you want the GPT to focus on, give it a profile picture, then a name, and you're ready to go. Using this approach, you get a GPT, but it doesn't make it any significantly better than classic ChatGPT without the fancy name and profile picture.

 The power of Custom GPT comes from the specific data and instructions provided to train it. By uploading relevant files and datasets, the model can become specialized in ways that broad pre-trained classic ChatGPT cannot. The knowledge contained in those uploaded files allows a Custom GPT to excel at certain tasks compared to ChatGPT, which may not have access to that specialized information. Ultimately, it is the custom data that enables greater capability.

 But uploading files to improve your GPT is a double-edged sword. It creates a privacy problem just as much as it boosts your GPT’s capabilities. Consider a scenario where you created a GPT to help customers learn more about you or your company. Anyone who has a link to your Custom GPT or somehow gets you to use a public prompt with a malicious link can access the files you've uploaded to your GPT.

 Here’s a simple illustration.

 I discovered a Custom GPT supposed to help users go viral on TikTok by recommending trending hashtags and topics. After the Custom GPT, it took little to no effort to get it to leak the instructions it was given when it was set up. Here's a sneak peek:

![Prompting a Custom GPT to leak its instructions](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/prompting-a-custom-gpt-to-leak-its-instructions.jpg)

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2123748/7443" target="_top" id="2123748">
  <img src="//a.impactradius-go.com/display-ad/7443-2123748" border="0" alt="https://techidaily.com" width="600" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2123748/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 And here's the second part of the instruction.

![Prompting a Custom GPT to leak its instructions 2](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/prompting-a-custom-gpt-to-leak-its-instructions-2.jpg)

 If you look closely, the second part of the instruction tells the model not to "share the names of the files directly with end users and under no circumstances should you provide a download link to any of the files." Of course, if you ask the custom GPT at first, it refuses, but with a little bit of prompt engineering, that changes. The custom GPT reveals the lone text file in its knowledge base.

![files in knowledge base-1](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/files-in-knowledge-base-1.jpg)

 With the file name, it took little effort to get the GPT to print the exact content of the file and subsequently download the file itself. In this case, the actual file wasn't sensitive. After poking around a few more GPTs, there were a lot with dozens of files sitting in the open.

![files in knowledge base2](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/files-in-knowledge-base2.jpg)

 There are hundreds of publicly available GPTs out there that contain sensitive files that are just sitting there waiting for malicious actors to grab.

## How to Protect Your Custom GPT Data

![chatgpt custom gpt share and publish options](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/chatgpt-custom-gpt-share-and-publish-options.jpg)

<!-- affiliate ads begin -->
<a href="https://dhgate.sjv.io/c/5597632/1186864/12108" target="_top" id="1186864">
  <img src="//a.impactradius-go.com/display-ad/12108-1186864" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://dhgate.sjv.io/i/5597632/1186864/12108" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 First, consider how you will share (or not!) the custom GPT you just created. In the top-right corner of the custom GPT creation screen, you'll find the **Save** button. Press the dropdown arrow icon, and from here, select how you want to share your creation:

* **Only me**: The custom GPT is not published and is only usable by you
* **Only people with a link:** Any one with the link to your custom GPT can use it and potentially access your data
* **Public:** Your custom GPT is available to anyone and can be indexed by Google and found in general internet searches. Anyone with access could potentially access your data.

 Unfortunately, there's currently no 100 percent foolproof way to protect the data you upload to a custom GPT that is shared publicly. You can get creative and give it strict instructions not to reveal the data in its knowledge base, but that's usually not enough, as our demonstration above has shown. If someone really wants to gain access to the knowledge base and has experience with AI prompt engineering and some time, eventually, the custom GPT will break and reveal the data.

 This is why the safest bet is not to upload any sensitive materials to a custom GPT you intend to share with the public. Once you upload private and sensitive data to a custom GPT and it leaves your computer, that data is effectively out of your control.

 Also, be very careful when using prompts you copy online. Make sure you understand them thoroughly and avoid obfuscated prompts that contain links. These could be malicious links that hijack, encode, and upload your files to remote servers.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2037335/7443" target="_top" id="2037335">
  <img src="//a.impactradius-go.com/display-ad/7443-2037335" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2037335/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

## Use Custom GPTs with Caution

 Custom GPTs are a powerful but potentially risky feature. While they allow you to create customized models that are highly capable in specific domains, the data you use to enhance their abilities can be exposed. To mitigate risk, avoid uploading truly sensitive data to your Custom GPTs whenever possible. Additionally, be wary of malicious prompt engineering that can exploit certain loopholes to steal your files.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 ChatGPT's custom GPT feature allows anyone to create a custom AI tool for almost anything you can think of; creative, technical, gaming, custom GPTs can do it all. Better still, you can share your custom GPT creations with anyone.

 However, by sharing your custom GPTs, you could be making a costly mistake that exposes your data to thousands of people globally.

## What Are Custom GPTs?

[Custom GPTs are programmable mini versions of ChatGPT](https://www.makeuseof.com/how-use-chatgpt-my-gpt-bots/) that can be trained to be more helpful on specific tasks. It is like molding ChatGPT into a chatbot that behaves the way you want and teaching it to become an expert in fields that really matter to you.

 For instance, a Grade 6 teacher could build a GPT that specializes in answering questions with a tone, word choice, and mannerism that is suitable for Grade 6 students. The GPT could be programmed such that whenever the teacher asks the GPT a question, the chatbot will formulate responses that speak directly to a 6th grader's level of understanding. It would avoid complex terminology, keep sentence length manageable, and adopt an encouraging tone. The allure of Custom GPTs is the ability to personalize the chatbot in this manner while also amplifying its expertise in certain areas.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2037351/7443" target="_top" id="2037351">
  <img src="//a.impactradius-go.com/display-ad/7443-2037351" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2037351/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

## How Custom GPTs Can Expose Your Data

 To [create Custom GPTs](https://www.makeuseof.com/how-use-create-a-gpt-to-create-a-customized-version-of-chatgpt/), you typically instruct ChatGPT’s GPT creator on which areas you want the GPT to focus on, give it a profile picture, then a name, and you're ready to go. Using this approach, you get a GPT, but it doesn't make it any significantly better than classic ChatGPT without the fancy name and profile picture.

 The power of Custom GPT comes from the specific data and instructions provided to train it. By uploading relevant files and datasets, the model can become specialized in ways that broad pre-trained classic ChatGPT cannot. The knowledge contained in those uploaded files allows a Custom GPT to excel at certain tasks compared to ChatGPT, which may not have access to that specialized information. Ultimately, it is the custom data that enables greater capability.

 But uploading files to improve your GPT is a double-edged sword. It creates a privacy problem just as much as it boosts your GPT’s capabilities. Consider a scenario where you created a GPT to help customers learn more about you or your company. Anyone who has a link to your Custom GPT or somehow gets you to use a public prompt with a malicious link can access the files you've uploaded to your GPT.

 Here’s a simple illustration.

 I discovered a Custom GPT supposed to help users go viral on TikTok by recommending trending hashtags and topics. After the Custom GPT, it took little to no effort to get it to leak the instructions it was given when it was set up. Here's a sneak peek:

![Prompting a Custom GPT to leak its instructions](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/prompting-a-custom-gpt-to-leak-its-instructions.jpg)

 And here's the second part of the instruction.

![Prompting a Custom GPT to leak its instructions 2](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/prompting-a-custom-gpt-to-leak-its-instructions-2.jpg)

 If you look closely, the second part of the instruction tells the model not to "share the names of the files directly with end users and under no circumstances should you provide a download link to any of the files." Of course, if you ask the custom GPT at first, it refuses, but with a little bit of prompt engineering, that changes. The custom GPT reveals the lone text file in its knowledge base.

![files in knowledge base-1](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/files-in-knowledge-base-1.jpg)

 With the file name, it took little effort to get the GPT to print the exact content of the file and subsequently download the file itself. In this case, the actual file wasn't sensitive. After poking around a few more GPTs, there were a lot with dozens of files sitting in the open.

![files in knowledge base2](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/files-in-knowledge-base2.jpg)

 There are hundreds of publicly available GPTs out there that contain sensitive files that are just sitting there waiting for malicious actors to grab.

## How to Protect Your Custom GPT Data

![chatgpt custom gpt share and publish options](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/chatgpt-custom-gpt-share-and-publish-options.jpg)

 First, consider how you will share (or not!) the custom GPT you just created. In the top-right corner of the custom GPT creation screen, you'll find the **Save** button. Press the dropdown arrow icon, and from here, select how you want to share your creation:

* **Only me**: The custom GPT is not published and is only usable by you
* **Only people with a link:** Any one with the link to your custom GPT can use it and potentially access your data
* **Public:** Your custom GPT is available to anyone and can be indexed by Google and found in general internet searches. Anyone with access could potentially access your data.

 Unfortunately, there's currently no 100 percent foolproof way to protect the data you upload to a custom GPT that is shared publicly. You can get creative and give it strict instructions not to reveal the data in its knowledge base, but that's usually not enough, as our demonstration above has shown. If someone really wants to gain access to the knowledge base and has experience with AI prompt engineering and some time, eventually, the custom GPT will break and reveal the data.

 This is why the safest bet is not to upload any sensitive materials to a custom GPT you intend to share with the public. Once you upload private and sensitive data to a custom GPT and it leaves your computer, that data is effectively out of your control.

 Also, be very careful when using prompts you copy online. Make sure you understand them thoroughly and avoid obfuscated prompts that contain links. These could be malicious links that hijack, encode, and upload your files to remote servers.

<!-- affiliate ads begin -->
<a href="https://ephamedtechinc.pxf.io/c/5597632/2136626/26400" target="_top" id="2136626">
  <img src="//a.impactradius-go.com/display-ad/26400-2136626" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://ephamedtechinc.pxf.io/i/5597632/2136626/26400" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

## Use Custom GPTs with Caution

 Custom GPTs are a powerful but potentially risky feature. While they allow you to create customized models that are highly capable in specific domains, the data you use to enhance their abilities can be exposed. To mitigate risk, avoid uploading truly sensitive data to your Custom GPTs whenever possible. Additionally, be wary of malicious prompt engineering that can exploit certain loopholes to steal your files.

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
<li><a href="https://vp-tips.techidaily.com/new-2024-approved-techniques-for-writing-eye-catching-podcast-summaries/"><u>[New] 2024 Approved Techniques for Writing Eye-Catching Podcast Summaries</u></a></li>
<li><a href="https://extra-tips.techidaily.com/updated-a-step-by-step-guide-to-masterful-editing/"><u>[Updated] A Step-by-Step Guide to Masterful Editing</u></a></li>
<li><a href="https://youtube-sure.techidaily.com/ed-cultivate-1000-fanbase-followers-quickly-for-2024/"><u>[Updated] Cultivate 1,000 Fanbase Followers Quickly for 2024</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-evaluating-m1s-capabilities-for-heavy-duty-media-editing/"><u>2024 Approved Evaluating M1's Capabilities for Heavy-Duty Media Editing</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/2024-approved-from-beginner-to-champion-essential-drone-races-tips-and-best-models/"><u>2024 Approved From Beginner to Champion Essential Drone Races Tips and Best Models</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/decoding-auto-gpts-efficacy-without-gpt-4/"><u>Decoding Auto-GPT’s Efficacy without GPT-4</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/googles-palm-2-clashes-with-openais-gpt-4/"><u>Google's PaLM 2 Clashes with OpenAI's GPT-4</u></a></li>
<li><a href="https://easy-unlock-android.techidaily.com/how-to-remove-screen-lock-pin-on-oneplus-nord-ce-3-lite-5g-like-a-pro-5-easy-ways-by-drfone-android/"><u>How To Remove Screen Lock PIN On OnePlus Nord CE 3 Lite 5G Like A Pro 5 Easy Ways</u></a></li>
<li><a href="https://apple-account.techidaily.com/in-2024-how-to-unlock-iphone-15-pro-max-when-we-dont-have-apple-id-or-password-by-drfone-ios/"><u>In 2024, How to Unlock iPhone 15 Pro Max When We Dont Have Apple ID or Password?</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/in-2024-the-best-8-vpn-hardware-devices-reviewed-on-motorola-moto-g84-5g-drfone-by-drfone-virtual-android/"><u>In 2024, The Best 8 VPN Hardware Devices Reviewed On Motorola Moto G84 5G | Dr.fone</u></a></li>
<li><a href="https://location-social.techidaily.com/in-2024-why-your-whatsapp-live-location-is-not-updating-and-how-to-fix-on-your-samsung-galaxy-m34-drfone-by-drfone-virtual-android/"><u>In 2024, Why Your WhatsApp Live Location is Not Updating and How to Fix on your Samsung Galaxy M34 | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/innovating-conversation-designing-unique-chatgpts/"><u>Innovating Conversation: Designing Unique ChatGPTs</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/keeping-your-conversational-data-intact-with-chatgpt/"><u>Keeping Your Conversational Data Intact with ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-character-creation-11-pivotal-chatgpt-tips/"><u>Mastering Character Creation: 11 Pivotal ChatGPT Tips</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/personalized-book-selection-simplified-top-5-ai-driven-literature-services/"><u>Personalized Book Selection Simplified: Top 5 AI-Driven Literature Services</u></a></li>
<li><a href="https://win-superb.techidaily.com/save-big-with-a-discounted-microsoft-office-2019-key-get-windows-or-mac-access-now-at-only-25-on-zdnet/"><u>Save Big with a Discounted Microsoft Office 2019 Key - Get Windows or Mac Access Now at Only $25 on ZDNET!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/streamlining-your-watchlist-with-chatgpt-insights/"><u>Streamlining Your Watchlist with ChatGPT Insights</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/trading-highs-and-lows-gpts-role-in-digital-asset-markets/"><u>Trading Highs & Lows: GPT's Role in Digital Asset Markets</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/vehicle-personalization-pathways-via-chatterbot-guidance/"><u>Vehicle Personalization Pathways via Chatterbot Guidance</u></a></li>
</ul></div>

