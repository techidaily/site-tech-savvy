---
title: Getting Started with LangChain & LLM
date: 2024-12-24T18:03:41.041Z
updated: 2024-12-27T21:27:42.330Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Getting Started with LangChain & LLM
excerpt: This Article Describes Getting Started with LangChain & LLM
thumbnail: https://thmb.techidaily.com/965654acbd64cd762e18be6423e980e53d1c3fa7dd1512b5cfdc18b0e2b93a57.jpg
---

## Getting Started with LangChain & LLM

 With the introduction of large language models (LLMs), Natural Language Processing has been the talk of the internet. New applications are being developed daily due to LLMs like ChatGPT and LangChain.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 LangChain is an open-source Python framework enabling developers to develop applications powered by large language models. Its applications are chatbots, summarization, generative questioning and answering, and many more.

 This article will provide an introduction to LangChain LLM. It will cover the basic concepts, how it compares to other language models, and how to get started with it.

>  Disclaimer: This post includes affiliate links
>
>  If you click on a link and make a purchase, I may receive a commission at no extra cost to you.
>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/S0b9szh8vEk?si=NlGzpJ6MN_SJNk5A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/LaWcXdTn5SE?si=QbxEkX-4a17J5RVs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## Getting Started With LangChain LLM

 Now you will learn how to implement LangChain in a real use-case scenario to understand how it works. Before starting the development, you need to set up the development environment.

### Setting Up Your Development Environment

 First, [create a virtual environment](https://www.makeuseof.com/create-manage-python-virtual-environments/) and install the dependencies below:

* **OpenAI**: To integrate GPT-3 API into your application.
* **LangChain**: To integrate LangChain into your application.

 Using pip, run the command below to install the dependencies:

`pipenv install langchain openai  
`

 The command above installs the packages and creates a virtual environment.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/vPGg53vbOsk?si=CkSEN5HFPS7vDuAa" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/ZeYbTVeaXg0?si=rwLL1DbBoX26BGjm" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/LI9nKlbhnw8?si=uUXFVbuEqXtFHHv0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Above is the expected output.

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
<li><a href="https://screen-mirroring-recording.techidaily.com/new-2024-approved-outwiththeold-camerasbeyondmycam/"><u>[New] 2024 Approved OutWithTheOld CamerasBeyondMyCam</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/2024-approved-expert-evaluation-of-vsdc-features-and-best-competitor-software/"><u>2024 Approved Expert Evaluation of VSDC Features and Best Competitor Software</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/analyzing-gpts-reference-to-external-data-sets/"><u>Analyzing GPT's Reference to External Data Sets</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/enhancing-writing-skills-through-chatgpt-practice/"><u>Enhancing Writing Skills Through ChatGPT Practice</u></a></li>
<li><a href="https://win-blog.techidaily.com/fixing-cod-black-ops-cold-war-error-80070057-a-step-by-step-guide/"><u>Fixing Cod: Black Ops Cold War Error 80070057 - A Step-by-Step Guide</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-will-apple-revolutionize-domestic-automation-unveiling-the-potential-of-homebound-bots-techfuture-insights/"><u>How Will Apple Revolutionize Domestic Automation? Unveiling the Potential of Homebound Bots | TechFuture Insights</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/in-2024-network-locked-sim-card-inserted-on-your-samsung-galaxy-a05-phone-unlock-it-now-by-drfone-android/"><u>In 2024, Network Locked SIM Card Inserted On Your Samsung Galaxy A05 Phone? Unlock It Now</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revolutionary-charging-solutions-discover-how-esrs-new-qi2-magsafe-adapters-power-up-iphone-16-devices-quickly-and-coolly-exclusive-on-zdnet/"><u>Revolutionary Charging Solutions: Discover How ESR's New Qi2 MagSafe Adapters Power Up iPhone 16 Devices Quickly and Coolly – Exclusive on ZDNET</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/secure-your-iphone-15-pro-max-at-a-penny-on-amazon-exclusive-guide-and-blowout-offer-details/"><u>Secure Your iPhone 15 Pro Max at a Penny on Amazon - Exclusive Guide & Blowout Offer Details!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/streamlining-numbers-with-gpt-3-6-efficient-methodologies/"><u>Streamlining Numbers with GPT-3: 6 Efficient Methodologies</u></a></li>
<li><a href="https://hardware-help.techidaily.com/unveiling-the-hidden-gems-of-tech-dells-best-kept-secrets-in-affordable-laptops-a-deep-dive/"><u>Unveiling the Hidden Gems of Tech: Dell's Best-Kept Secrets in Affordable Laptops - A Deep Dive</u></a></li>
<li><a href="https://ai-video-apps.techidaily.com/updated-2024-approved-avs-video-editor-is-only-available-on-windows-you-need-to-get-avs-video-editor-alternative-for-mac/"><u>Updated 2024 Approved AVS Video Editor Is only Available on Windows, You Need to Get AVS Video Editor Alternative for Mac</u></a></li>
<li><a href="https://smart-video-editing.techidaily.com/vn-video-editor-apk-pros-cons-and-features-review-for-2024/"><u>VN Video Editor APK Pros, Cons, and Features Review for 2024</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/what-pokemon-evolve-with-a-dawn-stone-for-tecno-pop-7-pro-drfone-by-drfone-virtual-android/"><u>What Pokémon Evolve with A Dawn Stone For Tecno Pop 7 Pro? | Dr.fone</u></a></li>
</ul></div>

