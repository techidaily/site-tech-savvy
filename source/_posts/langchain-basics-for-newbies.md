---
title: LangChain Basics for Newbies
date: 2024-12-20T18:50:51.270Z
updated: 2024-12-27T17:35:11.767Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes LangChain Basics for Newbies
excerpt: This Article Describes LangChain Basics for Newbies
thumbnail: https://thmb.techidaily.com/826e213581d156558e6f234936866c0f136b901791e5cc9453b472a1e6024dd2.jpeg
---

## LangChain Basics for Newbies

 With the introduction of large language models (LLMs), Natural Language Processing has been the talk of the internet. New applications are being developed daily due to LLMs like ChatGPT and LangChain.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 LangChain is an open-source Python framework enabling developers to develop applications powered by large language models. Its applications are chatbots, summarization, generative questioning and answering, and many more.

 This article will provide an introduction to LangChain LLM. It will cover the basic concepts, how it compares to other language models, and how to get started with it.

>  Disclaimer: This post includes affiliate links
>
>  If you click on a link and make a purchase, I may receive a commission at no extra cost to you.
>

## Understanding the LangChain LLM

 Before explaining how LangChain works, first, you need to understand [how large language models work](https://www.makeuseof.com/what-are-large-langauge-models-how-do-they-work/). A large language model is a type of artificial intelligence (AI) that [uses deep learning](https://www.makeuseof.com/deep-learning-vs-machine-learning-difference/) to train the machine learning models on big data consisting of textual, numerical, and code data.

 The vast amount of data enables the model to learn the existing patterns and relationships between words, figures, and symbols. This feature allows the model to perform an array of tasks, such as:

* Text generation, language translation, creative, technical, and academic content writing, and accurate and relevant question answering.
* Object detection in images.
* Summarization of books, articles, and research papers.

 LLMs’ most significant limitation is that the models are very general. This feature means that despite their ability to perform several tasks effectively, they may sometimes provide general answers to questions or prompts requiring expertise and deep domain knowledge instead of specific answers.

 Developed by Harrison Chase in late 2022, the LangChain framework offers an innovative approach to LLMs. The process starts by preprocessing the dataset texts by breaking it down into smaller parts or summaries. The summaries are then embedded in a vector space. The model receives a question, searches the summaries, and provides the appropriate response.

 LangChain’s preprocessing method is a critical feature that is unavoidable as LLMs become more powerful and data-intensive. This method is mainly used in code and semantic search cases because it provides real-time collection and interaction with the LLMs.

## LangChain LLM vs. Other Language Models

 The following comparative overview aims to highlight the unique features and capabilities that set LangChain LLM apart from other existing language models in the market:

* **Memory**: Several LLMs have a short memory, which usually results in context loss if prompts exceed the memory limit. LangChain, however, provides the previous chat prompts and responses, solving the issue of memory limits. The message history enables a user to repeat the previous messages to the LLM to recap the previous context.
* **LLM Switching**: Compared to other LLMs that lock your software with a single model’s API, LangChain provides an abstraction that simplifies the switching of LLMs or integrating multiple LLMs into your application. This is useful when you want to upgrade your software capabilities using a compact model, such as Stability AI’s StableLM say from OpenAI’s GPT-3.5\.
* **Integration**: Integrating LangChain into your application is easy compared to other LLMs. It provides pipeline workflows through [chains](https://docs.langchain.com/docs/components/chains/chain) and [agents](https://docs.langchain.com/docs/components/agents/agent), allowing you to quickly incorporate LangChain into your application. In terms of linear pipelines, chains are objects that essentially connect numerous parts. Agents are more advanced, allowing you to choose how the components should interact using business logic. For instance, you might want to use conditional logic to determine the next course of action based on the results of an LLM.
* **Data Passing**: Due to the general text-based nature of LLMs, it is usually tricky to pass data to the model. LangChain solves this problem by using [indexes](https://docs.langchain.com/docs/components/indexing/). Indexes enable an application to import data in variable formats and store it in a way that makes it possible to serve it row-by-row to an LLM.
* **Responses**: LangChain provides output parser tools to give answers in a suitable format as opposed to other LLMs whose model response consists of general text. When using AI in an application, it is preferred to have a structured response that you can program against.

## Getting Started With LangChain LLM

 Now you will learn how to implement LangChain in a real use-case scenario to understand how it works. Before starting the development, you need to set up the development environment.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/rdNq2Sp031s?si=3FcJa3dQLraUDHKv" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

### Setting Up Your Development Environment

 First, [create a virtual environment](https://www.makeuseof.com/create-manage-python-virtual-environments/) and install the dependencies below:

* **OpenAI**: To integrate GPT-3 API into your application.
* **LangChain**: To integrate LangChain into your application.

 Using pip, run the command below to install the dependencies:

`pipenv install langchain openai  
`

 The command above installs the packages and creates a virtual environment.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/Xq2r4ZKM-Po?si=fA2DdEB1op-atCkz" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

### Import the Installed Dependencies

 First, import the necessary classes such as **LLMChain**, **OpenAI**, **ConversationChain**, and **PromptTemplate** from the **langchain** package.

`from langchain import ConversationChain, OpenAI, PromptTemplate, LLMChain  
  
from langchain.memory import ConversationBufferWindowMemory`

 The LangChain classes outline and execute the language model chains.

### Access OpenAI API Key

 Next, get the OpenAI API key. To access OpenAI’s API key, you must have an OpenAI account, then move to the [OpenAI API platform](https://platform.openai.com/).

 On the dashboard, click on the Profile icon. Then, click the **View API keys** button.

![OpenAI API key dashboard](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/introduction-to-langchain-dashboard.jpeg)

 Next, click the **Create new secret key** button to get a new API key.

![OpenAI API key page](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/introduction-to-langchain-api-key-page.jpeg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/nWu29cqFjZA?si=TNZyCbPq68PQ0JIb" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Enter the requested name of the API key.

![OpenAI API key naming](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/introduction-to-langchain-api-key-naming.jpeg)

 You will receive a **secret key** prompt.

![OpenAI API key generated](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/introduction-to-langchain-api-key-generated.jpeg)

 Copy and store the API key in a safe place for future use.

## Developing an Application Using LangChain LLM

 You will now proceed to develop a simple chat application as follows:

`# Customize the LLM template
template = """Assistant is a large language model trained by OpenAI.  
  
{history}  
Human: {human_input}  
Assistant:"""  
  
prompt = PromptTemplate(input_variables=["history", "human_input"], template=template)`

 Next, you will load the ChatGPT chain using the API key you stored earlier.

`chatgpt_chain = LLMChain(  
  
           llm=OpenAI(openai_api_key="OPENAI_API_KEY",temperature=0),  
           prompt=prompt,  
           verbose=True,  
           memory=ConversationBufferWindowMemory(k=2),  
  
           )  

# Predict a sentence using the chatgpt chain

output = chatgpt_chain.predict(  
       human_input="What is MakeUseOf?"  
       )  

# Display the model's response

print(output)`

 This code loads the LLM chain with the OpenAI API key and the prompt template. User input is then provided, and its output is displayed.

![Output of developing an application using LangChain](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/introduction-to-langchain-output.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/mK1lEBRm_1w?si=FSaM0OKO0XBCgjtT" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Above is the expected output.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/HaM818fFKXQ?si=ZZLA4lFSHSgCpSE0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## The Rising Influence of LLMs

 LLMs consumption is growing rapidly and changing how humans interact with knowledge machines. Frameworks like LangChain are at the forefront of providing developers with a smooth and simple way to serve the LLMs to applications. Generative AI models like ChatGPT, Bard, and Hugging Face are also not left behind in advancing LLM applications.

**SCROLL TO CONTINUE WITH CONTENT**

 LangChain is an open-source Python framework enabling developers to develop applications powered by large language models. Its applications are chatbots, summarization, generative questioning and answering, and many more.

 This article will provide an introduction to LangChain LLM. It will cover the basic concepts, how it compares to other language models, and how to get started with it.

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
<li><a href="https://facebook-video-recording.techidaily.com/new-13-key-tactics-for-enhanced-visibility-in-facebook-videography/"><u>[New] 13 Key Tactics for Enhanced Visibility in Facebook Videography</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/new-epic-imagery-crafting-inspiring-instagram-posts-top20-for-2024/"><u>[New] Epic Imagery Crafting Inspiring Instagram Posts #Top20 for 2024</u></a></li>
<li><a href="https://article-posts.techidaily.com/new-essentials-for-successful-google-podcast-upload-for-2024/"><u>[New] Essentials for Successful Google Podcast Upload for 2024</u></a></li>
<li><a href="https://youtube-video-recordings.techidaily.com/2024-approved-enhance-clips-best-winter-bgs-for-video-warmth/"><u>2024 Approved Enhance Clips Best Winter Bg's for Video Warmth</u></a></li>
<li><a href="https://techno-recovery.techidaily.com/2024s-leading-smart-home-innovations-professional-evaluation-and-rankings-zdnet/"><u>2024'S Leading Smart Home Innovations: Professional Evaluation & Rankings | ZDNet</u></a></li>
<li><a href="https://driver-install.techidaily.com/achieving-peak-performance-with-updated-hyperx-soundcard-drivers/"><u>Achieving Peak Performance with Updated HyperX Soundcard Drivers</u></a></li>
<li><a href="https://extra-tips.techidaily.com/assessing-luminance-for-hd-raises-questions-for-2024/"><u>Assessing Luminance for HD Raises Questions for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/enhancing-teamwork-in-libreoffice-a-guide-to-adjusting-comment-styles/"><u>Enhancing Teamwork in LibreOffice: A Guide to Adjusting Comment Styles</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-82-of-executives-are-embracing-remote-work-trends-over-the-next-couple-of-years-insights-from-zdnet/"><u>How 82% of Executives Are Embracing Remote Work Trends Over the Next Couple of Years – Insights From ZDNet</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-manage-and-prevent-discomfort-in-your-mice-operating-hand-tips-shared-by-zdnet/"><u>How to Manage and Prevent Discomfort in Your Mice-Operating Hand – Tips Shared by ZDNet</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/hybrid-work-success-top-5-tips-from-industry-experts-as-featured-on-zdnet/"><u>Hybrid Work Success: Top 5 Tips From Industry Experts as Featured on ZDNet</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/in-2024-catchemall-celebrate-national-pokemon-day-with-virtual-location-on-infinix-smart-8-plus-drfone-by-drfone-virtual-android/"><u>In 2024, CatchEmAll Celebrate National Pokémon Day with Virtual Location On Infinix Smart 8 Plus | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/leveraging-notion-for-peak-productivity-a-comprehensive-reveal-of-its-benefits-and-usage/"><u>Leveraging Notion for Peak Productivity: A Comprehensive Reveal of Its Benefits and Usage</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-pitch-perfection-how-to-persuade-decision-makers-of-the-value-in-your-revolutionary-idea-expert-tips-by-zdnet/"><u>Mastering Pitch Perfection: How to Persuade Decision-Makers of the Value in Your Revolutionary Idea | Expert Tips by ZDNET</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-tab-management-in-the-arc-browser-boost-performance-by-utilizing-space-innovations/"><u>Mastering Tab Management in the Arc Browser: Boost Performance by Utilizing Space Innovations</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-the-mix-of-home-and-office-insights-for-a-winning-hybrid-work-strategy-advice-from-leaders-zdnet/"><u>Mastering the Mix of Home and Office: Insights for a Winning Hybrid Work Strategy - Advice From Leaders | ZDNET</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/maximize-productivity-using-the-opera-pop-up-function-insights-by-zdnet/"><u>Maximize Productivity Using the Opera Pop-Up Function - Insights by ZDNet</u></a></li>
<li><a href="https://tech-haven.techidaily.com/unlock-the-secrets-of-storytelling-mastery-using-chatgpt-techniques/"><u>Unlock the Secrets of Storytelling Mastery Using ChatGPT Techniques</u></a></li>
<li><a href="https://extra-resources.techidaily.com/unlocking-data-movement-best-ways-to-transition-files-to-pc/"><u>Unlocking Data Movement Best Ways to Transition Files to PC</u></a></li>
</ul></div>

