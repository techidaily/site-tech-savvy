---
title: Guarding Against Unintended Data Leakage in Custom GPTs
date: 2024-12-05T21:39:25.995Z
updated: 2024-12-06T22:23:03.254Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Guarding Against Unintended Data Leakage in Custom GPTs
excerpt: This Article Describes Guarding Against Unintended Data Leakage in Custom GPTs
thumbnail: https://thmb.techidaily.com/8787ab7f7fcdda2f4df516fbd446b3033c8b29f5461b80857fa8c26a8b142de0.jpg
---

## Guarding Against Unintended Data Leakage in Custom GPTs

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

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/oB9V7rZzotw?si=d4xrCbq1jKHXGAWN" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 With the file name, it took little effort to get the GPT to print the exact content of the file and subsequently download the file itself. In this case, the actual file wasn't sensitive. After poking around a few more GPTs, there were a lot with dozens of files sitting in the open.

![files in knowledge base2](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/files-in-knowledge-base2.jpg)

 There are hundreds of publicly available GPTs out there that contain sensitive files that are just sitting there waiting for malicious actors to grab.

## How to Protect Your Custom GPT Data

![chatgpt custom gpt share and publish options](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/chatgpt-custom-gpt-share-and-publish-options.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/eMEJvwMM0vk?si=EQF_jo_4u9v5iJ_C" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/grbt-5VvbuI?si=qnoirlmljslpqcQj" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/it8VkxDUdAc?si=ef6VZWR7kW4P9ikh" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 With the file name, it took little effort to get the GPT to print the exact content of the file and subsequently download the file itself. In this case, the actual file wasn't sensitive. After poking around a few more GPTs, there were a lot with dozens of files sitting in the open.

![files in knowledge base2](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/files-in-knowledge-base2.jpg)

 There are hundreds of publicly available GPTs out there that contain sensitive files that are just sitting there waiting for malicious actors to grab.

## How to Protect Your Custom GPT Data

![chatgpt custom gpt share and publish options](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/chatgpt-custom-gpt-share-and-publish-options.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/wNhKhWc0wLc?si=1XLYV0sXV52Xc0lu" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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
<iframe width="560" height="315" src="https://www.youtube.com/embed/qObsqoJB9LI?si=ppqxfXzP0UL4J6Tp" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 And here's the second part of the instruction.

![Prompting a Custom GPT to leak its instructions 2](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/prompting-a-custom-gpt-to-leak-its-instructions-2.jpg)

 If you look closely, the second part of the instruction tells the model not to "share the names of the files directly with end users and under no circumstances should you provide a download link to any of the files." Of course, if you ask the custom GPT at first, it refuses, but with a little bit of prompt engineering, that changes. The custom GPT reveals the lone text file in its knowledge base.

![files in knowledge base-1](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/files-in-knowledge-base-1.jpg)

 With the file name, it took little effort to get the GPT to print the exact content of the file and subsequently download the file itself. In this case, the actual file wasn't sensitive. After poking around a few more GPTs, there were a lot with dozens of files sitting in the open.

![files in knowledge base2](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/files-in-knowledge-base2.jpg)

 There are hundreds of publicly available GPTs out there that contain sensitive files that are just sitting there waiting for malicious actors to grab.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/Lp78eFEGwVU?si=-4orJBLvJJrggCJ2" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/PD0vq5qAYkw?si=5H3KWtCfUOYg1Nlv" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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

 If you look closely, the second part of the instruction tells the model not to "share the names of the files directly with end users and under no circumstances should you provide a download link to any of the files." Of course, if you ask the custom GPT at first, it refuses, but with a little bit of prompt engineering, that changes. The custom GPT reveals the lone text file in its knowledge base.

![files in knowledge base-1](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/files-in-knowledge-base-1.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/LBCobAYzzcc?si=J3eSTQ3AdyxWAjGo" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 With the file name, it took little effort to get the GPT to print the exact content of the file and subsequently download the file itself. In this case, the actual file wasn't sensitive. After poking around a few more GPTs, there were a lot with dozens of files sitting in the open.

![files in knowledge base2](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/files-in-knowledge-base2.jpg)

 There are hundreds of publicly available GPTs out there that contain sensitive files that are just sitting there waiting for malicious actors to grab.

## How to Protect Your Custom GPT Data

![chatgpt custom gpt share and publish options](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/11/chatgpt-custom-gpt-share-and-publish-options.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/_O8m9KphYzs?si=jITthzeyX_Kmt9X2" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 First, consider how you will share (or not!) the custom GPT you just created. In the top-right corner of the custom GPT creation screen, you'll find the **Save** button. Press the dropdown arrow icon, and from here, select how you want to share your creation:

* **Only me**: The custom GPT is not published and is only usable by you
* **Only people with a link:** Any one with the link to your custom GPT can use it and potentially access your data
* **Public:** Your custom GPT is available to anyone and can be indexed by Google and found in general internet searches. Anyone with access could potentially access your data.

 Unfortunately, there's currently no 100 percent foolproof way to protect the data you upload to a custom GPT that is shared publicly. You can get creative and give it strict instructions not to reveal the data in its knowledge base, but that's usually not enough, as our demonstration above has shown. If someone really wants to gain access to the knowledge base and has experience with AI prompt engineering and some time, eventually, the custom GPT will break and reveal the data.

 This is why the safest bet is not to upload any sensitive materials to a custom GPT you intend to share with the public. Once you upload private and sensitive data to a custom GPT and it leaves your computer, that data is effectively out of your control.

 Also, be very careful when using prompts you copy online. Make sure you understand them thoroughly and avoid obfuscated prompts that contain links. These could be malicious links that hijack, encode, and upload your files to remote servers.

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
<li><a href="https://fox-access.techidaily.com/new-2024-approved-beyond-code-the-story-of-virtual-reality/"><u>[New] 2024 Approved Beyond Code The Story of Virtual Reality</u></a></li>
<li><a href="https://youtube-blog.techidaily.com/n-2024-mastering-video-edits-in-youtube-studios-editor/"><u>[New] In 2024, Mastering Video Edits in YouTube Studio's Editor</u></a></li>
<li><a href="https://instagram-video-files.techidaily.com/updated-2024-approved-from-camera-to-feed-instagram-video-upload-on-desktop/"><u>[Updated] 2024 Approved From Camera to Feed Instagram Video Upload on Desktop</u></a></li>
<li><a href="https://fox-access.techidaily.com/2024-approved-editors-deep-dive-visionx-pro-and-its-features/"><u>2024 Approved Editor's Deep Dive VisionX Pro and Its Features</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/8-persuasive-reasons-for-educators-to-embrace-ai/"><u>8 Persuasive Reasons for Educators to Embrace AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-guide-to-harnessing-gpt-3s-full-capabilities-in-openai-arena/"><u>A Guide to Harnessing GPT-3's Full Capabilities in OpenAI Arena</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-timeline-to-artificial-intelligences-beginnings/"><u>A Timeline to Artificial Intelligence's Beginnings</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721410096261-avoid-data-theft-expose-fraudulent-chatgpt-sites-now/"><u>Avoid Data Theft: Expose Fraudulent ChatGPT Sites Now!</u></a></li>
<li><a href="https://screen-video-capture.techidaily.com/cutting-edge-methods-for-recording-presentations-for-2024/"><u>Cutting Edge Methods for Recording Presentations for 2024</u></a></li>
<li><a href="https://easy-unlock-android.techidaily.com/in-2024-unlock-your-poco-f5-pro-5gs-potential-the-top-20-lock-screen-apps-you-need-to-try-by-drfone-android/"><u>In 2024, Unlock Your Poco F5 Pro 5Gs Potential The Top 20 Lock Screen Apps You Need to Try</u></a></li>
</ul></div>

