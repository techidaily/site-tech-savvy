---
title: Evaluating Auto-GPT without GPT-4 Backup
date: 2024-11-24T16:44:11.168Z
updated: 2024-11-27T16:02:19.355Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Evaluating Auto-GPT without GPT-4 Backup
excerpt: This Article Describes Evaluating Auto-GPT without GPT-4 Backup
thumbnail: https://thmb.techidaily.com/e7a938c8213dc5d370405bab4afa736e010a188d2f4d2dd7c34adab834ad1c13.jpg
---

## Evaluating Auto-GPT without GPT-4 Backup

>  Disclaimer: This post includes affiliate links
>
>  If you click on a link and make a purchase, I may receive a commission at no extra cost to you.
>

### Key Takeaways

* Auto-GPT is an automation AI model that uses GPT-3.5 or GPT-4 to complete tasks independently, making it like a personal assistant that can automate most of your tasks.
* Auto-GPT can be accessed on your PC by following a step-by-step guide that involves downloading Python, setting up API keys, and launching Auto-GPT through the Terminal.
* Auto-GPT with GPT-4 API is more accurate and better at crawling the internet compared to GPT-3.5 API, but both versions can automate tasks with simple defined goals, although it's recommended to verify the information after completion.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 AI technology is accelerating fast, and we're moving towards artificial general intelligence that could change everything. We're not there yet, but ChatGPT-4 is widely considered the most advanced AI model.

 Well, there is a new kid on the block that makes it even easier to use GPT-4: Auto-GPT. How does it work? And can you use it without GPT-4?

## What Is Auto-GPT?

![Woman working on a laptop with a cup of coffee](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/laptop-on-desk.jpg)

 Auto-GPT is an automation AI model that uses GPT-3.5 or GPT-4 to complete tasks independently. In other words, Auto-GPT can develop its own prompts and answer autonomously to complete an objective. [Auto-GPT differs from ChatGPT](https://www.makeuseof.com/what-is-auto-gpt-how-differ-from-chatgpt/) because it doesn't need a human agent to prompt it every step of the way.

 What's more, Auto-GPT uses ChatGPT API to communicate with software, apps, and websites. This means Auto-GPT can reply to your emails, develop apps or websites, and even analyze the stock market autonomously with a single prompt.

 Basically, Auto-GPT is like your personal assistant that can automate most of your tasks, and there are already several [practical ways you can put Auto-GPT to use](https://www.makeuseof.com/ways-you-can-use-auto-gpt/).

## How Do You Access Auto-GPT on Your PC?

![A grey laptop and a phone on a table](https://thmb.techidaily.com/21f134ff6252e8b65e4072cbcc9d1f7716bea3abeb6dec26820e9ae291c1ae1c.jpg)

 For starters, you can access Auto-GPT using Windows, MacOS, or Linux. You also need an OpenAI API account before you start.

 Here is a step-by-step guide on how to install Auto-GPT on your PC:

1. First, download the latest version of Python to your computer. Here is a guide on [how to install Python PIP](https://www.makeuseof.com/tag/install-pip-for-python/) on Windows, Mac, and Linux. If you're using Windows, [add Python to the Windows PATH variable](https://www.makeuseof.com/python-windows-path/) before installation.  
![A tab showing a tab to install Python](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/2-install-python.jpg)
2. Download [Auto-GPT source code](http://github.com/Significant-Gravitas/Auto-GPT) from GitHub.
3. Extract the ZIP archive and copy the Auto-GPT folder to your preferred location.
4. Search for the ".env" file in the folder, right-click it, and select **Open with Notepad.**
5. Visit your OpenAI account, and on the top right of your screen, click **Personal** and select **View** **API keys**. This should take you to the [OpenAI API keys page](https://platform.openai.com/account/api-keys) while you're signed in.  
![OpenAI home page showing Personal section with View API keys](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/openai-home-page.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/XoC2TGp1PLY?si=iH9xs76NhWn4pP-E&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

1. Copy your secret API keys from Open AI. If you don't have API keys, click on **Create new secret key**.  
![Screenshot showing blurred out OpenAI API keys](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/api-keys.jpg)
2. Replace the "your-openai-api-key" text in the ".env.template" file with the API keys.  
![A notepad showing blurred out OpenAI key](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/notepad.jpg)
3. Create a free account on [pinecone.io](https://www.pinecone.io/). Once you've signed in to your account, select **API Keys** and click **Create API Key**. However, it's not mandatory you use pinecone.io to install Auto-GPT—if you're put on a waiting list, you can skip to step 12\.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/K4lRBnNnd9k?si=5e0MbdOz-fF6Ry_k&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

4. After naming and creating the new API key on Pinecone, copy the **Key Value** and paste it to replace "your-pinecone-api-key—this is on the third line under "PINECONE"on the".env" file you've opened using Notepad.
5. On the pinecone.io account, copy the details under **Environment** and paste it on the ".env." file next to PINECONE\_ENV—it should replace "your-pinecone-region".  
![A screenshot showing blurred Pinecone API key on Notepad](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/pinecone.jpg)

1. Save the ".env" file.
2. Right-click the Auto-GPT folder and select **Open in Terminal**.  
![Open AutoGPT environment](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/10-open-terminal.jpg)
3. After you've opened the Terminal, enter "pip install -r requirements.txt" to automatically download and install the necessary libraries for Auto-GPT.  
![Pip install requirements](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/11-pip-install-requirements.jpg)
4. Launch Auto-GPT on your computer by executing the following command: "python -m autogpt".  
![AutoGPT installation success](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/weldom.jpg)
5. Once you've launched Auto-GPT on your computer, the API will prompt you to give it a name and specific goals. For instance, you can define its role and tell it to analyze the stock market and save the report on a file.

 Next, Auto-GPT will ask for your permission to start—you can approve it by pressing "Y" and the Enter key. Alternatively, you can press "y-(number of actions)". More succinctly, if you want Auto-GPT to perform ten actions without seeking your authorization, you can press "Y-10" and hit **Enter**.

 If you want to stop an ongoing task quickly, you can utilize the **Ctrl + C** keyboard shortcut.

### Auto-GPT Benchmarking Tool

 The Auto-GPT August 2023 update introduced a new benchmarking tool designed to track the performance of the agents deployed. [Auto-GPT Benchmarks](https://github.com/Significant-Gravitas/AutoGPT/tree/master/benchmark) is still in development, but it gives you an idea of how your automated agents are performing in areas like "code, retrieval, memory, and safety."

## How Do You Access Auto-GPT on Your Browser?

![A screenshot of Agent GPT with name and goal defined.](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/agent-gpt.png)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/yr0yS_Ywrjs?si=QxzYiX1KmUaExmlo&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 If accessing Auto-GPT on your PC is too complicated, especially if you're unfamiliar with the Windows Terminal, you can still access it on your browser using AgentGPT. It could also be a safer option if you're concerned about privacy on your PC.

 Here is a step-by-step guide on how to install Auto-GPT on your PC:

1. Visit [AgentGPT](https://agentgpt.reworkd.ai/) and select **Settings** in the lower-left corner.
2. You will be prompted with a tab to input your OpenAI API key for GPT-4 or GPT-3.5-turbo.
3. After saving the API key, you will be prompted to name it and define its goal.
4. Click **Deploy Agent** to initiate the process.

 Once it's done, you can copy or save the information.

## Auto-GPT 3.5 API vs. Auto-GPT 4 API

![Art of an AI robot](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/rup-ai-chatgpt4.jpg)

 If you've subscribed to ChatGPT-4, you can access the GPT-4 API. But if you're using the free version of ChatGPT, you will be limited to GPT-3.5 API. What's the difference between using GPT-3.5 and GPT-4 to access Auto-GPT?

 The biggest difference is that Auto-GPT with GPT-3.5 API is much faster than GPT-4 API at completing tasks. However, in some cases, Auto-GPT with GPT-3.5 API is inaccurate with AI hallucinations. It also tends to go off-topic when you set up a goal.

 On the other hand, Auto-GPT with GPT-4 API is less likely to hallucinate and go off-topic compared to Auto-GPT with GPT-3.5 API. Its responses are similar to GPT-4, but the biggest difference is that it can crawl the internet in real-time and prompt itself until the task is complete. It actually does a better job of crawling the internet and compiling a thorough report than Microsoft's Bing AI—even Auto-GPT with GPT-3.5 API can outperform Bing AI.

 But the biggest shortcoming of Auto-GPT is that it can be stuck in a loop trying to complete a task—this happens whether you're using GPT-3.5 or GPT-4 API. For instance, if it prompts itself to "do nothing" in a planned action, it can be stuck on a loop instead of proceeding to the next course of action to complete a task.

 Auto-GPT with GPT-3.5 or GPT-4 API is also not fine-tuned to complete complex actions in one session. This is because Auto-GPT doesn't retain its previous findings after completing a session. Also, you can only add up to five goals on Auto-GPT per session if installed on your PC.

 However, the updated Auto-GPT has been improved with planning and task management capabilities that make it better to execute a task. In addition to that, the AI will let you know its thoughts, reasoning, plan, and criticism when performing an action.

![AutoGPT downloading file](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/3-recipe-generator.jpg)

 In retrospect, Auto-GPT with either GPT-3.5 or GPT-4 API can automate some of your tasks with simple defined goals. Of course, Auto-GPT with GPT-4 API has the edge over GPT-3.5 because it's more accurate and better at making sense of images. Here are the [key differences between GPT-4 and GPT 3.5 explained](https://www.makeuseof.com/gpt-4-vs-gpt-35-differences-explained).

## Is It Worth Using Auto-GPT Without GPT-4?

 Even though Auto-GPT with GPT-4 API performs better than Auto-GPT-3.5, you can still use Auto-GPT 3.5 to complete tasks autonomously. For example, I prompted Auto-GPT with GPT-3.5 API to search the internet for the best laptops on the market and give me a report with pros and cons.

![auto-gpt with gpt 3.5 output example](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/auto-gpt-with-gpt-3-5-output-example.jpg)

 Similarly, I prompted Auto-GPT with GPT-4 API with the same goals, and it gave me a report.

![auto-gpt with gpt 4 output example](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/auto-gpt-with-gpt-4-output-example.jpg)

 Based on the results, we can deduce that Auto-GPT is still a useful tool without GPT-4 API. In fact, Auto-GPT-3.5 tokens are way cheaper than GPT-4 tokens. Here is what you need to know about the [ChatGPT token limit](https://www.makeuseof.com/what-is-chatgpt-token-limit-can-you-exceed-it/).

 Auto-GPT with GPT-3.5 API can also automate the process of developing apps, coding, organizing events, and analyzing the crypto markets.

 However, according to its developers, Auto-GPT is not yet polished enough to completely rely on it without counter-checking the information—even if you're using GPT-4 API. It could also be expensive if you don't limit its token usage. Therefore, we recommend you terminate its connection after a task is complete.

 Besides that, Auto-GPT's developers acknowledge that Auto-GPT is experimental and may not be ideal for real-world situations.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/LaWcXdTn5SE?si=QbxEkX-4a17J5RVs&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## Auto-GPT Is a Game Changer

 Auto-GPT is the closest thing we have to artificial general intelligence, consideringit'ss an AI agent that can perform most tasks autonomously with just a few prompts.It'ss also easy to set up, and you can use it with GPT-3.5 or GPT-4\. However, Auto-GPT has its flaws, and it requires a human to verify the information after autonomously completing the tasks.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 AI technology is accelerating fast, and we're moving towards artificial general intelligence that could change everything. We're not there yet, but ChatGPT-4 is widely considered the most advanced AI model.

 Well, there is a new kid on the block that makes it even easier to use GPT-4: Auto-GPT. How does it work? And can you use it without GPT-4?

## What Is Auto-GPT?

![Woman working on a laptop with a cup of coffee](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/laptop-on-desk.jpg)

 Auto-GPT is an automation AI model that uses GPT-3.5 or GPT-4 to complete tasks independently. In other words, Auto-GPT can develop its own prompts and answer autonomously to complete an objective. [Auto-GPT differs from ChatGPT](https://www.makeuseof.com/what-is-auto-gpt-how-differ-from-chatgpt/) because it doesn't need a human agent to prompt it every step of the way.

 What's more, Auto-GPT uses ChatGPT API to communicate with software, apps, and websites. This means Auto-GPT can reply to your emails, develop apps or websites, and even analyze the stock market autonomously with a single prompt.

 Basically, Auto-GPT is like your personal assistant that can automate most of your tasks, and there are already several [practical ways you can put Auto-GPT to use](https://www.makeuseof.com/ways-you-can-use-auto-gpt/).

## How Do You Access Auto-GPT on Your PC?

![A grey laptop and a phone on a table](https://thmb.techidaily.com/21f134ff6252e8b65e4072cbcc9d1f7716bea3abeb6dec26820e9ae291c1ae1c.jpg)

 For starters, you can access Auto-GPT using Windows, MacOS, or Linux. You also need an OpenAI API account before you start.

 Here is a step-by-step guide on how to install Auto-GPT on your PC:

1. First, download the latest version of Python to your computer. Here is a guide on [how to install Python PIP](https://www.makeuseof.com/tag/install-pip-for-python/) on Windows, Mac, and Linux. If you're using Windows, [add Python to the Windows PATH variable](https://www.makeuseof.com/python-windows-path/) before installation.  
![A tab showing a tab to install Python](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/2-install-python.jpg)
2. Download [Auto-GPT source code](http://github.com/Significant-Gravitas/Auto-GPT) from GitHub.
3. Extract the ZIP archive and copy the Auto-GPT folder to your preferred location.
4. Search for the ".env" file in the folder, right-click it, and select **Open with Notepad.**
5. Visit your OpenAI account, and on the top right of your screen, click **Personal** and select **View** **API keys**. This should take you to the [OpenAI API keys page](https://platform.openai.com/account/api-keys) while you're signed in.  
![OpenAI home page showing Personal section with View API keys](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/openai-home-page.jpg)

1. Copy your secret API keys from Open AI. If you don't have API keys, click on **Create new secret key**.  
![Screenshot showing blurred out OpenAI API keys](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/api-keys.jpg)
2. Replace the "your-openai-api-key" text in the ".env.template" file with the API keys.  
![A notepad showing blurred out OpenAI key](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/notepad.jpg)
3. Create a free account on [pinecone.io](https://www.pinecone.io/). Once you've signed in to your account, select **API Keys** and click **Create API Key**. However, it's not mandatory you use pinecone.io to install Auto-GPT—if you're put on a waiting list, you can skip to step 12\.
4. After naming and creating the new API key on Pinecone, copy the **Key Value** and paste it to replace "your-pinecone-api-key—this is on the third line under "PINECONE"on the".env" file you've opened using Notepad.
5. On the pinecone.io account, copy the details under **Environment** and paste it on the ".env." file next to PINECONE\_ENV—it should replace "your-pinecone-region".  
![A screenshot showing blurred Pinecone API key on Notepad](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/pinecone.jpg)

1. Save the ".env" file.
2. Right-click the Auto-GPT folder and select **Open in Terminal**.  
![Open AutoGPT environment](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/10-open-terminal.jpg)
3. After you've opened the Terminal, enter "pip install -r requirements.txt" to automatically download and install the necessary libraries for Auto-GPT.  
![Pip install requirements](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/11-pip-install-requirements.jpg)
4. Launch Auto-GPT on your computer by executing the following command: "python -m autogpt".  
![AutoGPT installation success](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/weldom.jpg)
5. Once you've launched Auto-GPT on your computer, the API will prompt you to give it a name and specific goals. For instance, you can define its role and tell it to analyze the stock market and save the report on a file.

 Next, Auto-GPT will ask for your permission to start—you can approve it by pressing "Y" and the Enter key. Alternatively, you can press "y-(number of actions)". More succinctly, if you want Auto-GPT to perform ten actions without seeking your authorization, you can press "Y-10" and hit **Enter**.

 If you want to stop an ongoing task quickly, you can utilize the **Ctrl + C** keyboard shortcut.

### Auto-GPT Benchmarking Tool

 The Auto-GPT August 2023 update introduced a new benchmarking tool designed to track the performance of the agents deployed. [Auto-GPT Benchmarks](https://github.com/Significant-Gravitas/AutoGPT/tree/master/benchmark) is still in development, but it gives you an idea of how your automated agents are performing in areas like "code, retrieval, memory, and safety."

## How Do You Access Auto-GPT on Your Browser?

![A screenshot of Agent GPT with name and goal defined.](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/agent-gpt.png)

 If accessing Auto-GPT on your PC is too complicated, especially if you're unfamiliar with the Windows Terminal, you can still access it on your browser using AgentGPT. It could also be a safer option if you're concerned about privacy on your PC.

 Here is a step-by-step guide on how to install Auto-GPT on your PC:

1. Visit [AgentGPT](https://agentgpt.reworkd.ai/) and select **Settings** in the lower-left corner.
2. You will be prompted with a tab to input your OpenAI API key for GPT-4 or GPT-3.5-turbo.
3. After saving the API key, you will be prompted to name it and define its goal.
4. Click **Deploy Agent** to initiate the process.

 Once it's done, you can copy or save the information.

## Auto-GPT 3.5 API vs. Auto-GPT 4 API

![Art of an AI robot](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/rup-ai-chatgpt4.jpg)

 If you've subscribed to ChatGPT-4, you can access the GPT-4 API. But if you're using the free version of ChatGPT, you will be limited to GPT-3.5 API. What's the difference between using GPT-3.5 and GPT-4 to access Auto-GPT?

 The biggest difference is that Auto-GPT with GPT-3.5 API is much faster than GPT-4 API at completing tasks. However, in some cases, Auto-GPT with GPT-3.5 API is inaccurate with AI hallucinations. It also tends to go off-topic when you set up a goal.

 On the other hand, Auto-GPT with GPT-4 API is less likely to hallucinate and go off-topic compared to Auto-GPT with GPT-3.5 API. Its responses are similar to GPT-4, but the biggest difference is that it can crawl the internet in real-time and prompt itself until the task is complete. It actually does a better job of crawling the internet and compiling a thorough report than Microsoft's Bing AI—even Auto-GPT with GPT-3.5 API can outperform Bing AI.

 But the biggest shortcoming of Auto-GPT is that it can be stuck in a loop trying to complete a task—this happens whether you're using GPT-3.5 or GPT-4 API. For instance, if it prompts itself to "do nothing" in a planned action, it can be stuck on a loop instead of proceeding to the next course of action to complete a task.

 Auto-GPT with GPT-3.5 or GPT-4 API is also not fine-tuned to complete complex actions in one session. This is because Auto-GPT doesn't retain its previous findings after completing a session. Also, you can only add up to five goals on Auto-GPT per session if installed on your PC.

 However, the updated Auto-GPT has been improved with planning and task management capabilities that make it better to execute a task. In addition to that, the AI will let you know its thoughts, reasoning, plan, and criticism when performing an action.

![AutoGPT downloading file](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/3-recipe-generator.jpg)

 In retrospect, Auto-GPT with either GPT-3.5 or GPT-4 API can automate some of your tasks with simple defined goals. Of course, Auto-GPT with GPT-4 API has the edge over GPT-3.5 because it's more accurate and better at making sense of images. Here are the [key differences between GPT-4 and GPT 3.5 explained](https://www.makeuseof.com/gpt-4-vs-gpt-35-differences-explained).

## Is It Worth Using Auto-GPT Without GPT-4?

 Even though Auto-GPT with GPT-4 API performs better than Auto-GPT-3.5, you can still use Auto-GPT 3.5 to complete tasks autonomously. For example, I prompted Auto-GPT with GPT-3.5 API to search the internet for the best laptops on the market and give me a report with pros and cons.

![auto-gpt with gpt 3.5 output example](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/auto-gpt-with-gpt-3-5-output-example.jpg)

 Similarly, I prompted Auto-GPT with GPT-4 API with the same goals, and it gave me a report.

![auto-gpt with gpt 4 output example](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/auto-gpt-with-gpt-4-output-example.jpg)

 Based on the results, we can deduce that Auto-GPT is still a useful tool without GPT-4 API. In fact, Auto-GPT-3.5 tokens are way cheaper than GPT-4 tokens. Here is what you need to know about the [ChatGPT token limit](https://www.makeuseof.com/what-is-chatgpt-token-limit-can-you-exceed-it/).

 Auto-GPT with GPT-3.5 API can also automate the process of developing apps, coding, organizing events, and analyzing the crypto markets.

 However, according to its developers, Auto-GPT is not yet polished enough to completely rely on it without counter-checking the information—even if you're using GPT-4 API. It could also be expensive if you don't limit its token usage. Therefore, we recommend you terminate its connection after a task is complete.

 Besides that, Auto-GPT's developers acknowledge that Auto-GPT is experimental and may not be ideal for real-world situations.

## Auto-GPT Is a Game Changer

 Auto-GPT is the closest thing we have to artificial general intelligence, consideringit'ss an AI agent that can perform most tasks autonomously with just a few prompts.It'ss also easy to set up, and you can use it with GPT-3.5 or GPT-4\. However, Auto-GPT has its flaws, and it requires a human to verify the information after autonomously completing the tasks.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 AI technology is accelerating fast, and we're moving towards artificial general intelligence that could change everything. We're not there yet, but ChatGPT-4 is widely considered the most advanced AI model.

 Well, there is a new kid on the block that makes it even easier to use GPT-4: Auto-GPT. How does it work? And can you use it without GPT-4?

## What Is Auto-GPT?

![Woman working on a laptop with a cup of coffee](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/laptop-on-desk.jpg)

 Auto-GPT is an automation AI model that uses GPT-3.5 or GPT-4 to complete tasks independently. In other words, Auto-GPT can develop its own prompts and answer autonomously to complete an objective. [Auto-GPT differs from ChatGPT](https://www.makeuseof.com/what-is-auto-gpt-how-differ-from-chatgpt/) because it doesn't need a human agent to prompt it every step of the way.

 What's more, Auto-GPT uses ChatGPT API to communicate with software, apps, and websites. This means Auto-GPT can reply to your emails, develop apps or websites, and even analyze the stock market autonomously with a single prompt.

 Basically, Auto-GPT is like your personal assistant that can automate most of your tasks, and there are already several [practical ways you can put Auto-GPT to use](https://www.makeuseof.com/ways-you-can-use-auto-gpt/).

## How Do You Access Auto-GPT on Your PC?

![A grey laptop and a phone on a table](https://thmb.techidaily.com/21f134ff6252e8b65e4072cbcc9d1f7716bea3abeb6dec26820e9ae291c1ae1c.jpg)

 For starters, you can access Auto-GPT using Windows, MacOS, or Linux. You also need an OpenAI API account before you start.

 Here is a step-by-step guide on how to install Auto-GPT on your PC:

1. First, download the latest version of Python to your computer. Here is a guide on [how to install Python PIP](https://www.makeuseof.com/tag/install-pip-for-python/) on Windows, Mac, and Linux. If you're using Windows, [add Python to the Windows PATH variable](https://www.makeuseof.com/python-windows-path/) before installation.  
![A tab showing a tab to install Python](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/2-install-python.jpg)
2. Download [Auto-GPT source code](http://github.com/Significant-Gravitas/Auto-GPT) from GitHub.
3. Extract the ZIP archive and copy the Auto-GPT folder to your preferred location.
4. Search for the ".env" file in the folder, right-click it, and select **Open with Notepad.**
5. Visit your OpenAI account, and on the top right of your screen, click **Personal** and select **View** **API keys**. This should take you to the [OpenAI API keys page](https://platform.openai.com/account/api-keys) while you're signed in.  
![OpenAI home page showing Personal section with View API keys](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/openai-home-page.jpg)

1. Copy your secret API keys from Open AI. If you don't have API keys, click on **Create new secret key**.  
![Screenshot showing blurred out OpenAI API keys](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/api-keys.jpg)
2. Replace the "your-openai-api-key" text in the ".env.template" file with the API keys.  
![A notepad showing blurred out OpenAI key](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/notepad.jpg)
3. Create a free account on [pinecone.io](https://www.pinecone.io/). Once you've signed in to your account, select **API Keys** and click **Create API Key**. However, it's not mandatory you use pinecone.io to install Auto-GPT—if you're put on a waiting list, you can skip to step 12\.
4. After naming and creating the new API key on Pinecone, copy the **Key Value** and paste it to replace "your-pinecone-api-key—this is on the third line under "PINECONE"on the".env" file you've opened using Notepad.
5. On the pinecone.io account, copy the details under **Environment** and paste it on the ".env." file next to PINECONE\_ENV—it should replace "your-pinecone-region".  
![A screenshot showing blurred Pinecone API key on Notepad](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/pinecone.jpg)

1. Save the ".env" file.
2. Right-click the Auto-GPT folder and select **Open in Terminal**.  
![Open AutoGPT environment](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/10-open-terminal.jpg)
3. After you've opened the Terminal, enter "pip install -r requirements.txt" to automatically download and install the necessary libraries for Auto-GPT.  
![Pip install requirements](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/11-pip-install-requirements.jpg)
4. Launch Auto-GPT on your computer by executing the following command: "python -m autogpt".  
![AutoGPT installation success](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/weldom.jpg)
5. Once you've launched Auto-GPT on your computer, the API will prompt you to give it a name and specific goals. For instance, you can define its role and tell it to analyze the stock market and save the report on a file.

 Next, Auto-GPT will ask for your permission to start—you can approve it by pressing "Y" and the Enter key. Alternatively, you can press "y-(number of actions)". More succinctly, if you want Auto-GPT to perform ten actions without seeking your authorization, you can press "Y-10" and hit **Enter**.

 If you want to stop an ongoing task quickly, you can utilize the **Ctrl + C** keyboard shortcut.

### Auto-GPT Benchmarking Tool

 The Auto-GPT August 2023 update introduced a new benchmarking tool designed to track the performance of the agents deployed. [Auto-GPT Benchmarks](https://github.com/Significant-Gravitas/AutoGPT/tree/master/benchmark) is still in development, but it gives you an idea of how your automated agents are performing in areas like "code, retrieval, memory, and safety."

## How Do You Access Auto-GPT on Your Browser?

![A screenshot of Agent GPT with name and goal defined.](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/agent-gpt.png)

 If accessing Auto-GPT on your PC is too complicated, especially if you're unfamiliar with the Windows Terminal, you can still access it on your browser using AgentGPT. It could also be a safer option if you're concerned about privacy on your PC.

 Here is a step-by-step guide on how to install Auto-GPT on your PC:

1. Visit [AgentGPT](https://agentgpt.reworkd.ai/) and select **Settings** in the lower-left corner.
2. You will be prompted with a tab to input your OpenAI API key for GPT-4 or GPT-3.5-turbo.
3. After saving the API key, you will be prompted to name it and define its goal.
4. Click **Deploy Agent** to initiate the process.

 Once it's done, you can copy or save the information.

## Auto-GPT 3.5 API vs. Auto-GPT 4 API

![Art of an AI robot](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/rup-ai-chatgpt4.jpg)

 If you've subscribed to ChatGPT-4, you can access the GPT-4 API. But if you're using the free version of ChatGPT, you will be limited to GPT-3.5 API. What's the difference between using GPT-3.5 and GPT-4 to access Auto-GPT?

 The biggest difference is that Auto-GPT with GPT-3.5 API is much faster than GPT-4 API at completing tasks. However, in some cases, Auto-GPT with GPT-3.5 API is inaccurate with AI hallucinations. It also tends to go off-topic when you set up a goal.

 On the other hand, Auto-GPT with GPT-4 API is less likely to hallucinate and go off-topic compared to Auto-GPT with GPT-3.5 API. Its responses are similar to GPT-4, but the biggest difference is that it can crawl the internet in real-time and prompt itself until the task is complete. It actually does a better job of crawling the internet and compiling a thorough report than Microsoft's Bing AI—even Auto-GPT with GPT-3.5 API can outperform Bing AI.

 But the biggest shortcoming of Auto-GPT is that it can be stuck in a loop trying to complete a task—this happens whether you're using GPT-3.5 or GPT-4 API. For instance, if it prompts itself to "do nothing" in a planned action, it can be stuck on a loop instead of proceeding to the next course of action to complete a task.

 Auto-GPT with GPT-3.5 or GPT-4 API is also not fine-tuned to complete complex actions in one session. This is because Auto-GPT doesn't retain its previous findings after completing a session. Also, you can only add up to five goals on Auto-GPT per session if installed on your PC.

 However, the updated Auto-GPT has been improved with planning and task management capabilities that make it better to execute a task. In addition to that, the AI will let you know its thoughts, reasoning, plan, and criticism when performing an action.

![AutoGPT downloading file](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/3-recipe-generator.jpg)

 In retrospect, Auto-GPT with either GPT-3.5 or GPT-4 API can automate some of your tasks with simple defined goals. Of course, Auto-GPT with GPT-4 API has the edge over GPT-3.5 because it's more accurate and better at making sense of images. Here are the [key differences between GPT-4 and GPT 3.5 explained](https://www.makeuseof.com/gpt-4-vs-gpt-35-differences-explained).

## Is It Worth Using Auto-GPT Without GPT-4?

 Even though Auto-GPT with GPT-4 API performs better than Auto-GPT-3.5, you can still use Auto-GPT 3.5 to complete tasks autonomously. For example, I prompted Auto-GPT with GPT-3.5 API to search the internet for the best laptops on the market and give me a report with pros and cons.

![auto-gpt with gpt 3.5 output example](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/auto-gpt-with-gpt-3-5-output-example.jpg)

 Similarly, I prompted Auto-GPT with GPT-4 API with the same goals, and it gave me a report.

![auto-gpt with gpt 4 output example](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/auto-gpt-with-gpt-4-output-example.jpg)

 Based on the results, we can deduce that Auto-GPT is still a useful tool without GPT-4 API. In fact, Auto-GPT-3.5 tokens are way cheaper than GPT-4 tokens. Here is what you need to know about the [ChatGPT token limit](https://www.makeuseof.com/what-is-chatgpt-token-limit-can-you-exceed-it/).

 Auto-GPT with GPT-3.5 API can also automate the process of developing apps, coding, organizing events, and analyzing the crypto markets.

 However, according to its developers, Auto-GPT is not yet polished enough to completely rely on it without counter-checking the information—even if you're using GPT-4 API. It could also be expensive if you don't limit its token usage. Therefore, we recommend you terminate its connection after a task is complete.

 Besides that, Auto-GPT's developers acknowledge that Auto-GPT is experimental and may not be ideal for real-world situations.

## Auto-GPT Is a Game Changer

 Auto-GPT is the closest thing we have to artificial general intelligence, consideringit'ss an AI agent that can perform most tasks autonomously with just a few prompts.It'ss also easy to set up, and you can use it with GPT-3.5 or GPT-4\. However, Auto-GPT has its flaws, and it requires a human to verify the information after autonomously completing the tasks.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 AI technology is accelerating fast, and we're moving towards artificial general intelligence that could change everything. We're not there yet, but ChatGPT-4 is widely considered the most advanced AI model.

 Well, there is a new kid on the block that makes it even easier to use GPT-4: Auto-GPT. How does it work? And can you use it without GPT-4?

## What Is Auto-GPT?

![Woman working on a laptop with a cup of coffee](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/laptop-on-desk.jpg)

 Auto-GPT is an automation AI model that uses GPT-3.5 or GPT-4 to complete tasks independently. In other words, Auto-GPT can develop its own prompts and answer autonomously to complete an objective. [Auto-GPT differs from ChatGPT](https://www.makeuseof.com/what-is-auto-gpt-how-differ-from-chatgpt/) because it doesn't need a human agent to prompt it every step of the way.

 What's more, Auto-GPT uses ChatGPT API to communicate with software, apps, and websites. This means Auto-GPT can reply to your emails, develop apps or websites, and even analyze the stock market autonomously with a single prompt.

 Basically, Auto-GPT is like your personal assistant that can automate most of your tasks, and there are already several [practical ways you can put Auto-GPT to use](https://www.makeuseof.com/ways-you-can-use-auto-gpt/).

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/LdVT_-3gESA?si=_HfjpbUEHSRKTXjt&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## How Do You Access Auto-GPT on Your PC?

![A grey laptop and a phone on a table](https://thmb.techidaily.com/21f134ff6252e8b65e4072cbcc9d1f7716bea3abeb6dec26820e9ae291c1ae1c.jpg)

 For starters, you can access Auto-GPT using Windows, MacOS, or Linux. You also need an OpenAI API account before you start.

 Here is a step-by-step guide on how to install Auto-GPT on your PC:

1. First, download the latest version of Python to your computer. Here is a guide on [how to install Python PIP](https://www.makeuseof.com/tag/install-pip-for-python/) on Windows, Mac, and Linux. If you're using Windows, [add Python to the Windows PATH variable](https://www.makeuseof.com/python-windows-path/) before installation.  
![A tab showing a tab to install Python](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/2-install-python.jpg)
2. Download [Auto-GPT source code](http://github.com/Significant-Gravitas/Auto-GPT) from GitHub.
3. Extract the ZIP archive and copy the Auto-GPT folder to your preferred location.
4. Search for the ".env" file in the folder, right-click it, and select **Open with Notepad.**
5. Visit your OpenAI account, and on the top right of your screen, click **Personal** and select **View** **API keys**. This should take you to the [OpenAI API keys page](https://platform.openai.com/account/api-keys) while you're signed in.  
![OpenAI home page showing Personal section with View API keys](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/openai-home-page.jpg)

1. Copy your secret API keys from Open AI. If you don't have API keys, click on **Create new secret key**.  
![Screenshot showing blurred out OpenAI API keys](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/api-keys.jpg)
2. Replace the "your-openai-api-key" text in the ".env.template" file with the API keys.  
![A notepad showing blurred out OpenAI key](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/notepad.jpg)
3. Create a free account on [pinecone.io](https://www.pinecone.io/). Once you've signed in to your account, select **API Keys** and click **Create API Key**. However, it's not mandatory you use pinecone.io to install Auto-GPT—if you're put on a waiting list, you can skip to step 12\.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/Q_69vX9wnRE?si=FtLxkpRhPORqcMeE&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

4. After naming and creating the new API key on Pinecone, copy the **Key Value** and paste it to replace "your-pinecone-api-key—this is on the third line under "PINECONE"on the".env" file you've opened using Notepad.
5. On the pinecone.io account, copy the details under **Environment** and paste it on the ".env." file next to PINECONE\_ENV—it should replace "your-pinecone-region".  
![A screenshot showing blurred Pinecone API key on Notepad](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/pinecone.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/4qA2pGQ5qmw?si=1mAA9WTi2Z5F7n6s&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

1. Save the ".env" file.
2. Right-click the Auto-GPT folder and select **Open in Terminal**.  
![Open AutoGPT environment](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/10-open-terminal.jpg)
3. After you've opened the Terminal, enter "pip install -r requirements.txt" to automatically download and install the necessary libraries for Auto-GPT.  

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/RhLjZsruC9M?si=-861oUSfrUde2Ykt&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

![Pip install requirements](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/11-pip-install-requirements.jpg)
4. Launch Auto-GPT on your computer by executing the following command: "python -m autogpt".  
![AutoGPT installation success](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/weldom.jpg)
5. Once you've launched Auto-GPT on your computer, the API will prompt you to give it a name and specific goals. For instance, you can define its role and tell it to analyze the stock market and save the report on a file.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/jjGL9wFdlbo?si=Vb1JgZqRXNc03UGG&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Next, Auto-GPT will ask for your permission to start—you can approve it by pressing "Y" and the Enter key. Alternatively, you can press "y-(number of actions)". More succinctly, if you want Auto-GPT to perform ten actions without seeking your authorization, you can press "Y-10" and hit **Enter**.

 If you want to stop an ongoing task quickly, you can utilize the **Ctrl + C** keyboard shortcut.

### Auto-GPT Benchmarking Tool

 The Auto-GPT August 2023 update introduced a new benchmarking tool designed to track the performance of the agents deployed. [Auto-GPT Benchmarks](https://github.com/Significant-Gravitas/AutoGPT/tree/master/benchmark) is still in development, but it gives you an idea of how your automated agents are performing in areas like "code, retrieval, memory, and safety."

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/43goO8X0iX0?si=48Cqf6td2q_6T6h3&autoplay=1" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## How Do You Access Auto-GPT on Your Browser?

![A screenshot of Agent GPT with name and goal defined.](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/agent-gpt.png)

 If accessing Auto-GPT on your PC is too complicated, especially if you're unfamiliar with the Windows Terminal, you can still access it on your browser using AgentGPT. It could also be a safer option if you're concerned about privacy on your PC.

 Here is a step-by-step guide on how to install Auto-GPT on your PC:

1. Visit [AgentGPT](https://agentgpt.reworkd.ai/) and select **Settings** in the lower-left corner.
2. You will be prompted with a tab to input your OpenAI API key for GPT-4 or GPT-3.5-turbo.
3. After saving the API key, you will be prompted to name it and define its goal.
4. Click **Deploy Agent** to initiate the process.

 Once it's done, you can copy or save the information.

## Auto-GPT 3.5 API vs. Auto-GPT 4 API

![Art of an AI robot](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/rup-ai-chatgpt4.jpg)

 If you've subscribed to ChatGPT-4, you can access the GPT-4 API. But if you're using the free version of ChatGPT, you will be limited to GPT-3.5 API. What's the difference between using GPT-3.5 and GPT-4 to access Auto-GPT?

 The biggest difference is that Auto-GPT with GPT-3.5 API is much faster than GPT-4 API at completing tasks. However, in some cases, Auto-GPT with GPT-3.5 API is inaccurate with AI hallucinations. It also tends to go off-topic when you set up a goal.

 On the other hand, Auto-GPT with GPT-4 API is less likely to hallucinate and go off-topic compared to Auto-GPT with GPT-3.5 API. Its responses are similar to GPT-4, but the biggest difference is that it can crawl the internet in real-time and prompt itself until the task is complete. It actually does a better job of crawling the internet and compiling a thorough report than Microsoft's Bing AI—even Auto-GPT with GPT-3.5 API can outperform Bing AI.

 But the biggest shortcoming of Auto-GPT is that it can be stuck in a loop trying to complete a task—this happens whether you're using GPT-3.5 or GPT-4 API. For instance, if it prompts itself to "do nothing" in a planned action, it can be stuck on a loop instead of proceeding to the next course of action to complete a task.

 Auto-GPT with GPT-3.5 or GPT-4 API is also not fine-tuned to complete complex actions in one session. This is because Auto-GPT doesn't retain its previous findings after completing a session. Also, you can only add up to five goals on Auto-GPT per session if installed on your PC.

 However, the updated Auto-GPT has been improved with planning and task management capabilities that make it better to execute a task. In addition to that, the AI will let you know its thoughts, reasoning, plan, and criticism when performing an action.

![AutoGPT downloading file](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/3-recipe-generator.jpg)

 In retrospect, Auto-GPT with either GPT-3.5 or GPT-4 API can automate some of your tasks with simple defined goals. Of course, Auto-GPT with GPT-4 API has the edge over GPT-3.5 because it's more accurate and better at making sense of images. Here are the [key differences between GPT-4 and GPT 3.5 explained](https://www.makeuseof.com/gpt-4-vs-gpt-35-differences-explained).

## Is It Worth Using Auto-GPT Without GPT-4?

 Even though Auto-GPT with GPT-4 API performs better than Auto-GPT-3.5, you can still use Auto-GPT 3.5 to complete tasks autonomously. For example, I prompted Auto-GPT with GPT-3.5 API to search the internet for the best laptops on the market and give me a report with pros and cons.

![auto-gpt with gpt 3.5 output example](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/auto-gpt-with-gpt-3-5-output-example.jpg)

 Similarly, I prompted Auto-GPT with GPT-4 API with the same goals, and it gave me a report.

![auto-gpt with gpt 4 output example](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/05/auto-gpt-with-gpt-4-output-example.jpg)

 Based on the results, we can deduce that Auto-GPT is still a useful tool without GPT-4 API. In fact, Auto-GPT-3.5 tokens are way cheaper than GPT-4 tokens. Here is what you need to know about the [ChatGPT token limit](https://www.makeuseof.com/what-is-chatgpt-token-limit-can-you-exceed-it/).

 Auto-GPT with GPT-3.5 API can also automate the process of developing apps, coding, organizing events, and analyzing the crypto markets.

 However, according to its developers, Auto-GPT is not yet polished enough to completely rely on it without counter-checking the information—even if you're using GPT-4 API. It could also be expensive if you don't limit its token usage. Therefore, we recommend you terminate its connection after a task is complete.

 Besides that, Auto-GPT's developers acknowledge that Auto-GPT is experimental and may not be ideal for real-world situations.

## Auto-GPT Is a Game Changer

 Auto-GPT is the closest thing we have to artificial general intelligence, consideringit'ss an AI agent that can perform most tasks autonomously with just a few prompts.It'ss also easy to set up, and you can use it with GPT-3.5 or GPT-4\. However, Auto-GPT has its flaws, and it requires a human to verify the information after autonomously completing the tasks.

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
<li><a href="https://fox-access.techidaily.com/new-2024-approved-navigating-video-conversion-in-vlc-from-mp4-onward/"><u>[New] 2024 Approved Navigating Video Conversion in VLC From MP4 Onward</u></a></li>
<li><a href="https://vp-tips.techidaily.com/new-in-2024-top-5-macos-safari-video-conversion-apps/"><u>[New] In 2024, Top 5 macOS Safari Video Conversion Apps</u></a></li>
<li><a href="https://extra-support.techidaily.com/new-pixelpop-complete-examination-and-manual-24/"><u>[New] PixelPop Complete Examination & Manual '24</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/updated-2024-approved-a-guide-to-gauging-igtv-video-impressions/"><u>[Updated] 2024 Approved A Guide to Gauging IGTV Video Impressions</u></a></li>
<li><a href="https://extra-support.techidaily.com/updated-quick-and-easy-iphone-burst-techniques/"><u>[Updated] Quick and Easy iPhone Burst Techniques</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1726030489207-pc/"><u>「撮影素材の組み込みが楽 - PCとスマートフォンで動画への加工方法」</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/44cm44k544og44os44kq5aplusplus5bplusc44oy44od44oj44ov44kp44oz44oe44kk44kv44gn6auy5zob6loq44gq6yyy6zplusz44gr44gk44ge44gm5a2m44g244cn/"><u>「ステレオ対応ヘッドフォンマイクで高品質な録音について学ぶ」</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1726029764512-android/"><u>最新の自由音楽プレイヤー - Androidユーザによるベスト選び！</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/airplayyoutube/"><u>AirPlay機能が使えない状況での動画再生方法：YouTubeやその他について学ぶ</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/androidiso-iso/"><u>Android上でISO画像ファイルのプレーヤー設定 - ISOファイル導入手順</u></a></li>
<li><a href="https://hardware-help.techidaily.com/ensure-superior-sound-quality-with-the-updated-realtek-drivers-for-windows-11-10-and-7-free-downloads/"><u>Ensure Superior Sound Quality with the Updated Realtek Drivers for Windows 11, 10 and 7 – Free Downloads</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1726029880424-handbrake/"><u>HandBrakeで動画を最適化するための簡単なガイド: コンパクト形式へ</u></a></li>
<li><a href="https://location-social.techidaily.com/in-2024-how-to-send-and-fake-live-location-on-facebook-messenger-of-your-xiaomi-13t-pro-drfone-by-drfone-virtual-android/"><u>In 2024, How to Send and Fake Live Location on Facebook Messenger Of your Xiaomi 13T Pro | Dr.fone</u></a></li>
<li><a href="https://some-skills.techidaily.com/in-2024-the-ultimate-edge-testing-gopros-hero5-black-against-sessions/"><u>In 2024, The Ultimate Edge Testing GoPro's Hero5 Black Against Sessions</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1726030144340-iphone/"><u>IPhone動画フォーマット変換ガイド集</u></a></li>
<li><a href="https://video-content-creator.techidaily.com/new-2024-approved-take-a-screenshot-share-the-fun-a-guide-to-ps4-online-sharing/"><u>New 2024 Approved Take a Screenshot, Share the Fun A Guide to PS4 Online Sharing</u></a></li>
<li><a href="https://network-issues.techidaily.com/overcoming-code-43-failure-for-nvidia-geforce-gtx-950-on-windows-11-systems-solutions-proven-effective/"><u>Overcoming 'Code 43' Failure for NVIDIA GeForce GTX 950 on Windows 11 Systems - Solutions Proven Effective</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/44ko44od44k444ow44op44km44k244gl44kj57ch5y2y44gr5pig5yop44ov44kh44kk44or44ks44oa44km44oz44ot44o844oj44gz44kl5oml5byv44gn/"><u>エッジブラウザから簡単に映像ファイルをダウンロードする手引き</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/44k544ox44o844oz44gu5q2j44gx44ge6kiy6yyy44go6yyy6zplusz5oml5rov44gr44gk44ge44gm5a2m44g2ic0g5yq55p6c55qe44gq44og44kv44ol44od44kv/"><u>スプーンの正しい記録と録音手法について学ぶ - 効果的なテクニック</u></a></li>
</ul></div>

