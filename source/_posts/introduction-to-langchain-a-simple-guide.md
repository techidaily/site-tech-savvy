---
title: "Introduction to LangChain: A Simple Guide"
date: 2024-08-10T02:06:22.171Z
updated: 2024-08-11T02:06:22.171Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Introduction to LangChain: A Simple Guide"
excerpt: "This Article Describes Introduction to LangChain: A Simple Guide"
thumbnail: https://thmb.techidaily.com/3c560b5f84950935f235a17f57ab9b2b0c297df9b81f28e15578b876da96606b.jpg
---

## Introduction to LangChain: A Simple Guide

 With the introduction of large language models (LLMs), Natural Language Processing has been the talk of the internet. New applications are being developed daily due to LLMs like ChatGPT and LangChain.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 LangChain is an open-source Python framework enabling developers to develop applications powered by large language models. Its applications are chatbots, summarization, generative questioning and answering, and many more.

 This article will provide an introduction to LangChain LLM. It will cover the basic concepts, how it compares to other language models, and how to get started with it.

## Understanding the LangChain LLM

 Before explaining how LangChain works, first, you need to understand [how large language models work](https://www.makeuseof.com/what-are-large-langauge-models-how-do-they-work/). A large language model is a type of artificial intelligence (AI) that [uses deep learning](https://www.makeuseof.com/deep-learning-vs-machine-learning-difference/) to train the machine learning models on big data consisting of textual, numerical, and code data.

 The vast amount of data enables the model to learn the existing patterns and relationships between words, figures, and symbols. This feature allows the model to perform an array of tasks, such as:

* Text generation, language translation, creative, technical, and academic content writing, and accurate and relevant question answering.
* Object detection in images.
* Summarization of books, articles, and research papers.

 LLMs’ most significant limitation is that the models are very general. This feature means that despite their ability to perform several tasks effectively, they may sometimes provide general answers to questions or prompts requiring expertise and deep domain knowledge instead of specific answers.

 Developed by Harrison Chase in late 2022, the LangChain framework offers an innovative approach to LLMs. The process starts by preprocessing the dataset texts by breaking it down into smaller parts or summaries. The summaries are then embedded in a vector space. The model receives a question, searches the summaries, and provides the appropriate response.

 LangChain’s preprocessing method is a critical feature that is unavoidable as LLMs become more powerful and data-intensive. This method is mainly used in code and semantic search cases because it provides real-time collection and interaction with the LLMs.

<!-- affiliate ads begin -->
<a href="https://otszone.ots7.com/order/checkout.php?PRODS=4713324&QTY=1&AFFILIATE=108875&CART=1"><img src="https://green.ots7.com/screenshots/OtsAV/OtsAVTV1.90-300x188.jpg" border="0">OtsAV TV Webcaster</a>
<!-- affiliate ads end -->
## LangChain LLM vs. Other Language Models

 The following comparative overview aims to highlight the unique features and capabilities that set LangChain LLM apart from other existing language models in the market:

* **Memory**: Several LLMs have a short memory, which usually results in context loss if prompts exceed the memory limit. LangChain, however, provides the previous chat prompts and responses, solving the issue of memory limits. The message history enables a user to repeat the previous messages to the LLM to recap the previous context.
* **LLM Switching**: Compared to other LLMs that lock your software with a single model’s API, LangChain provides an abstraction that simplifies the switching of LLMs or integrating multiple LLMs into your application. This is useful when you want to upgrade your software capabilities using a compact model, such as Stability AI’s StableLM say from OpenAI’s GPT-3.5\.
* **Integration**: Integrating LangChain into your application is easy compared to other LLMs. It provides pipeline workflows through [chains](https://docs.langchain.com/docs/components/chains/chain) and [agents](https://docs.langchain.com/docs/components/agents/agent), allowing you to quickly incorporate LangChain into your application. In terms of linear pipelines, chains are objects that essentially connect numerous parts. Agents are more advanced, allowing you to choose how the components should interact using business logic. For instance, you might want to use conditional logic to determine the next course of action based on the results of an LLM.
* **Data Passing**: Due to the general text-based nature of LLMs, it is usually tricky to pass data to the model. LangChain solves this problem by using [indexes](https://docs.langchain.com/docs/components/indexing/). Indexes enable an application to import data in variable formats and store it in a way that makes it possible to serve it row-by-row to an LLM.
* **Responses**: LangChain provides output parser tools to give answers in a suitable format as opposed to other LLMs whose model response consists of general text. When using AI in an application, it is preferred to have a structured response that you can program against.

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
<iframe id="iframe_672" src="//a.impactradius-go.com/gen-ad-code/5597632/1959812/17834/" width="720" height="300" scrolling="no" frameborder="0" marginheight="0" marginwidth="0"></iframe>
<!-- affiliate ads end -->
### Import the Installed Dependencies

 First, import the necessary classes such as **LLMChain**, **OpenAI**, **ConversationChain**, and **PromptTemplate** from the **langchain** package.

`from langchain import ConversationChain, OpenAI, PromptTemplate, LLMChain  
  
from langchain.memory import ConversationBufferWindowMemory`

 The LangChain classes outline and execute the language model chains.

### Access OpenAI API Key

 Next, get the OpenAI API key. To access OpenAI’s API key, you must have an OpenAI account, then move to the [OpenAI API platform](https://platform.openai.com/).

 On the dashboard, click on the Profile icon. Then, click the **View API keys** button.

<!-- affiliate ads begin -->
<a href="https://order.glarysoft.com/order/checkout.php?PRODS=4691139&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/6734fa703f6633ab896eecbdfad8953a/products/SU-200-1.png" border="0">Software Update Pro - Check and update software installed on your computer. </a>
<!-- affiliate ads end -->
![OpenAI API key dashboard](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/introduction-to-langchain-dashboard.jpeg)

 Next, click the **Create new secret key** button to get a new API key.

![OpenAI API key page](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/introduction-to-langchain-api-key-page.jpeg)

 Enter the requested name of the API key.

![OpenAI API key naming](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/introduction-to-langchain-api-key-naming.jpeg)

 You will receive a **secret key** prompt.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=36506229&QTY=1&AFFILIATE=108875&CART=1"><video width="100%" height="" class="rounded-t-md shadow-lg relative z-20" controls="" autoplay="" loop="" muted="" playsinline="" webkit-playinginline="">
<source type="video/mp4" src="https://aidaform.com/images/videos/aidaform-welcome-site.mp4"><source type="video/webm" src="https://aidaform.com/images/videos/aidaform-welcome-site.webm"></video></a>
<!-- affiliate ads end -->
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

<!-- affiliate ads begin -->
<span id="1993650">
					<video width="720" height="300" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1993650.jpeg"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/22993-1993650">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1993650.jpeg" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:720px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fhomestyler.sjv.io%2Fc%2F5597632%2F1993650%2F22993'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1993650/22993" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![Output of developing an application using LangChain](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/introduction-to-langchain-output.jpg)

 Above is the expected output.

<!-- affiliate ads begin -->
<a href="https://shop.pcdj.com/order/checkout.php?PRODS=4698832&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/47f4b6321e9fd8e8f7326a6adc1a7c1e/products/karaoki-new-searchresultspane.jpg" border="0">PCDJ Karaoki is the complete professional karaoke software designed for KJs and karaoke venues. Karaoki includes an advanced automatic singer rotation list with singer history, key control, news ticker, next singers screen, a song book exporter and printer, a jukebox background music player and many other features designed so you can host karaoke shows faster and easier! 
 PCDJ Karaoki (WINDOWS ONLY Professional Karaoke Software - 3 Activations)</a>
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
<li><a href="https://facebook-record-videos.techidaily.com/new-2024-approved-expert-strategies-for-higher-youtube-shorts-revenue/"><u>[New] 2024 Approved  Expert Strategies for Higher YouTube Shorts Revenue</u></a></li>
<li><a href="https://screen-recording.techidaily.com/new-in-2024-complete-razer-kiyo-webcam-review/"><u>[New] In 2024, Complete Razer Kiyo Webcam Review</u></a></li>
<li><a href="https://extra-support.techidaily.com/new-leading-edge-cards-for-sharp-4k-gaming/"><u>[New] Leading Edge Cards for Sharp 4K Gaming</u></a></li>
<li><a href="https://instagram-video-files.techidaily.com/new-the-ultimate-guide-to-reverse-playbacks-on-instavids-for-2024/"><u>[New] The Ultimate Guide to Reverse Playbacks on InstaVids for 2024</u></a></li>
<li><a href="https://screen-capture.techidaily.com/updated-mastering-lenovo-perfecting-screen-capture-techniques/"><u>[Updated] Mastering Lenovo  Perfecting Screen Capture Techniques</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/10-innovative-ai-software-for-professional-email-writing/"><u>10 Innovative AI Software for Professional Email Writing</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/101-ai-tips-learning-from-9-beginner-friendly-groups/"><u>101 AI Tips: Learning From 9 Beginner-Friendly Groups</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/23-chatgpt-driven-solutions-for-crafting-business-emails/"><u>23 ChatGPT-Driven Solutions for Crafting Business Emails</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/26-inbox-perfection-free-ai-email-assistance-at-its-peak/"><u>26 Inbox Perfection: Free AI Email Assistance at Its Peak</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/28-innovative-replacements-for-openais-point-of-sale-apps/"><u>28 Innovative Replacements for OpenAI’s Point-of-Sale Apps</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/4-ai-powered-online-murder-mystery-puzzles-and-games-to-play-detective/"><u>4 AI-Powered Online Murder Mystery Puzzles and Games to Play Detective</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/5-compelling-arguments-for-enterprises-dismissing-gpt/"><u>5 Compelling Arguments for Enterprises Dismissing GPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/5-myths-about-gpt-and-the-world-of-digital-assets/"><u>5 Myths About GPT and the World of Digital Assets</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/6-best-chatgpt-extensions-for-vs-code/"><u>6 Best ChatGPT Extensions for VS Code</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/6-compelling-arguments-why-professionals-should-embrace-chatgpt/"><u>6 Compelling Arguments: Why Professionals Should Embrace ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/6-practical-ways-to-use-chatgpt-in-your-job-search/"><u>6 Practical Ways to Use ChatGPT in Your Job Search</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/8-persuasive-reasons-for-educators-to-embrace-ai/"><u>8 Persuasive Reasons for Educators to Embrace AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/8-ways-ai-chatbots-are-impacting-content-creation/"><u>8 Ways AI Chatbots Are Impacting Content Creation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/8-ways-to-use-chatgpt-for-your-business/"><u>8 Ways to Use ChatGPT for Your Business</u></a></li>
<li><a href="https://android-location-track.techidaily.com/9-best-phone-monitoring-apps-for-vivo-y17s-drfone-by-drfone-virtual-android/"><u>9 Best Phone Monitoring Apps for Vivo Y17s | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/9-chatgpt-powered-tools-to-streamline-your-email-creation/"><u>9 ChatGPT-Powered Tools to Streamline Your Email Creation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-critical-review-of-the-metaphor-describing-the-internet-as-a-giant-library-for-scholars/"><u>A Critical Review of the Metaphor Describing the Internet as a 'Giant Library' For Scholars</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-guide-to-harnessing-gpt-3s-full-capabilities-in-openai-arena/"><u>A Guide to Harnessing GPT-3's Full Capabilities in OpenAI Arena</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-new-dimension-to-hobbies-strategic-play-and-imagery-via-my-bots/"><u>A New Dimension to Hobbies: Strategic Play & Imagery via My Bots</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-timeline-to-artificial-intelligences-beginnings/"><u>A Timeline to Artificial Intelligence's Beginnings</u></a></li>
<li><a href="https://tech-revival.techidaily.com/ai-through-ages-epochs-and-early-triumphs/"><u>AI Through Ages: Epochs and Early Triumphs</u></a></li>
<li><a href="https://facebook-clips.techidaily.com/amp-up-the-sound-beat-downloads-on-fb-for-2024/"><u>Amp Up the Sound  Beat Downloads on FB for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721410096261-avoid-data-theft-expose-fraudulent-chatgpt-sites-now/"><u>Avoid Data Theft: Expose Fraudulent ChatGPT Sites Now!</u></a></li>
<li><a href="https://tech-revival.techidaily.com/can-auto-gpt-stand-alone-without-relying-on-gpt-narratives/"><u>Can Auto-GPT Stand Alone Without Relying on GPT-Narratives?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721431165441-chatgpt-at-your-fingertips-android-app-now/"><u>ChatGPT at Your Fingertips - Android App Now</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721435679680-cleared-twitter-of-checkmarks-linuss-revelations-trojan-analysis-and-ai-shortcom-writes/"><u>Cleared Twitter of Checkmarks, Linus’s Revelations, Trojan Analysis, & AI Shortcom Writes</u></a></li>
<li><a href="https://extra-information.techidaily.com/complete-google-photos-guide-for-beginners/"><u>Complete Google Photos Guide for Beginners</u></a></li>
<li><a href="https://article-helps.techidaily.com/complete-overview-the-spinning-lens-revolution/"><u>Complete Overview  The Spinning Lens Revolution</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721390956327-enhancing-your-dialogues-with-gpt-chrome-edition/"><u>Enhancing Your Dialogues with GPT, Chrome Edition</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721402584696-gpt-4-universally-accessible-6-reasons-to-persist-with-platinum-plan/"><u>GPT-4 Universally Accessible; 6 Reasons to Persist with Platinum Plan.</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721401269099-gpt-4-a-new-era-of-free-accessibility-yet-plus-maintains-6-valued-features/"><u>GPT-4: A New Era of Free Accessibility, Yet Plus Maintains 6 Valued Features.</u></a></li>
<li><a href="https://buynow-help.techidaily.com/holy-stone-rc-cartoon-race-car-review-family-friendly-fun/"><u>Holy Stone RC Cartoon Race Car Review: Family-Friendly Fun</u></a></li>
<li><a href="https://fake-location.techidaily.com/how-to-simulate-gps-movement-in-ar-games-on-tecno-camon-20-pro-5g-drfone-by-drfone-virtual-android/"><u>How to Simulate GPS Movement in AR games On Tecno Camon 20 Pro 5G? | Dr.fone</u></a></li>
<li><a href="https://android-location-track.techidaily.com/how-to-track-vivo-y77t-location-without-installing-software-drfone-by-drfone-virtual-android/"><u>How to Track Vivo Y77t Location without Installing Software? | Dr.fone</u></a></li>
<li><a href="https://android-transfer.techidaily.com/in-2024-best-3-software-to-transfer-files-tofrom-your-vivo-v30-via-a-usb-cable-drfone-by-drfone-transfer-from-android-transfer-from-android/"><u>In 2024, Best 3 Software to Transfer Files to/from Your Vivo V30 via a USB Cable | Dr.fone</u></a></li>
<li><a href="https://android-unlock.techidaily.com/in-2024-best-ways-on-how-to-unlockbypassswiperemove-samsung-fingerprint-lock-by-drfone-android/"><u>In 2024, Best Ways on How to Unlock/Bypass/Swipe/Remove Samsung Fingerprint Lock</u></a></li>
<li><a href="https://facebook-videos.techidaily.com/in-2024-signal-profileshots-guide-dimensions-file-type-minutes/"><u>In 2024, Signal Profileshots Guide  Dimensions, File Type, Minutes</u></a></li>
<li><a href="https://fox-boxes.techidaily.com/in-2024-tap-into-the-latest-gaming-and-app-splash-of-win11/"><u>In 2024, Tap Into the Latest Gaming and App Splash of Win11</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721416514954-innovative-mobile-search-bings-ai-for-everyday-use/"><u>Innovative Mobile Search - Bing’s AI for Everyday Use</u></a></li>
<li><a href="https://iphone-unlock.techidaily.com/iphone-8-asking-for-passcode-after-ios-1714-update-what-to-do-drfone-by-drfone-ios/"><u>iPhone 8 Asking for Passcode after iOS 17/14 Update, What to Do? | Dr.fone</u></a></li>
<li><a href="https://youtube-video-recordings.techidaily.com/large-display-medium-network-selection-tips/"><u>Large Display Medium Network Selection Tips</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721426226662-overcoming-gpts-text-limit-tips-and-tricks/"><u>Overcoming GPT's Text Limit – Tips & Tricks</u></a></li>
</ul></div>
