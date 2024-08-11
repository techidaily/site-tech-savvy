---
title: Building Bots with GPT-3 & Python
date: 2024-08-10T02:14:22.184Z
updated: 2024-08-11T02:14:22.184Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Building Bots with GPT-3 & Python
excerpt: This Article Describes Building Bots with GPT-3 & Python
thumbnail: https://thmb.techidaily.com/80de444cb408ef81f4728e2850b723591d8016d7f4cd61445fe263111407c51f.jpg
---

## Building Bots with GPT-3 & Python

 An AI storm has swept across the world. The release of OpenAI's ChatGPT has sent developers and curious users into a frenzy. OpenAI has gathered a whopping 100 million active users within two months of its launch and people have already started building applications using it.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 CopyAI uses it to generate copywriting content for websites, blogs, advertisements, emails, and social media. Lex uses GPT-3 to answer research questions, Algolia for semantic search, and Replier to create branded replies to customer reviews. Here's how you can use OpenAI's GPT-3 model with Python to get started on building your AI-powered application.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2068407/7443" target="_top" id="2068407"><img src="//a.impactradius-go.com/display-ad/7443-2068407" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2068407/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## What Is GPT-3?

[OpenAI's GPT-3](https://www.makeuseof.com/how-to-use-gpt-3-openai-playground/) is the third-generation Generative Pre-trained Transformer. It is a Machine Learning model with over 175 billion parameters, almost the entire internet. This gives it immense capabilities to answer a wide range of questions and perform tasks that would otherwise take a lot of manual effort.

 Open AI has developed a Python module that contains pre-defined compatible classes to interact with its APIs. To install it on your system, open a terminal and run:

`pip install openai`

 If you're wondering what GPT-3 is capable of, then you can explore some of the [creative uses for GPT-3 in OpenAI Playground](https://www.makeuseof.com/creative-uses-for-gpt-3-openai-playground/).

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=40085955&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/f702defbc67edb455949f46babab0c18/products/2_logo9.png" border="0">FX PRO (Gold Robot + Silver Robot(Basic Package))</a>
<!-- affiliate ads end -->
## Generating the API Key

 To use GPT-3 with Python you need to generate an API key. To view your API key, follow these steps:

1. Sign up for an account on the [OpenAI page](https://platform.openai.com/overview). Select the account type as **Personal**.
2. Click on your profile and select the **View API Keys** button.  
<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2087394/7443" target="_top" id="2087394"><img src="//a.impactradius-go.com/display-ad/7443-2087394" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2087394/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![View API Key of OpenAI website](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/02/view-api-key-of-openai-website-1.jpg)
3. Click on **Create new secret key** to generate your API key.  
![Create Secret API Screen of OpenAI website](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/02/create-secret-api-screen-of-openai-website.jpg)
4. Copy your API key and keep it in a secure location as you won't be able to view it again.

 OpenAI's GPT-3 API charges you based on the number of tokens (words) you use to interact with it. Luckily, OpenAI provides $18 of credit for free for the first three months, so you can explore it and experiment according to your needs.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2087264/19272" target="_top" id="2087264"><img src="//a.impactradius-go.com/display-ad/19272-2087264" border="0" alt="" width="336" height="280"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2087264/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Building a Python Program to Use the GPT-3 API

 You can find the source code of this program in its [GitHub repository](https://github.com/makeuseofcode/GPT-3-With-Python).

 Now that you have access to the API, you can build a Python program to communicate using it. Start building the program by importing the OpenAI module. Define a function, **askGPT()**,that takes **text** as an input argument. The text will contain the query you are going to ask GPT-3\. Copy the API key you generated earlier and initialize it.

`import openai  
  
def askGPT(text):  
    openai.api_key = "your_api_key"`

 Create a request by defining the following parameters:

* **engine:** The model you want to use for your request. The **Davinci** model is the most reliable, trained to data until October 2019\.
* **prompt:** Prompt is the set of words you ask as a question to generate a response from the API.
* **temperature:** Set how professional or creative your text should sound. With lower values, you will get more focused and deterministic answers. With higher values, you will get more creative answers. 0.6 is a good compromise.
* **max\_tokens:** The maximum number of words in the generated response. You can set it to a maximum of 2,048 words.

 For example, here's how you can send a request and store the response:

`response = openai.Completion.create(  
        engine = "text-davinci-003",  
        prompt = text,  
        temperature = 0.6,  
        max_tokens = 150,  
    )  
`

 Display GPT-3's response by retrieving the text parameter of the first result:

`return print(response.choices [0].text)`

 To invoke this function, define a main function and an infinite loop. Ask the user to enter a question and pass it to the **askGpt()** function.

`def main():  
    while True:  
        print('GPT: Ask me a question\n')  
        myQn = input()  
        askGPT(myQn)  
  
main()`

 Put it all together and use Artificial Intelligence to answer your questions.

<!-- affiliate ads begin -->
<a href="https://modlily.sjv.io/c/5597632/2072819/17059" target="_top" id="2072819"><img src="//a.impactradius-go.com/display-ad/17059-2072819" border="0" alt="" width="300" height="250"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2072819/17059" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## The Output of Your GPT-3-Enabled Python Program

 When you run the program, it will ask you to enter a question. On entering the prompt, "Write a poem in 5 lines about how Iron Man is the greatest superhero of all time," the program produced the following impressive output:

<!-- affiliate ads begin -->
<a href="https://bluetties.sjv.io/c/5597632/2039292/17094" target="_top" id="2039292"><img src="//a.impactradius-go.com/display-ad/17094-2039292" border="0" alt="BLUETTI NEW LAUNCH AC240" width="954" height="1020"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2039292/17094" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![Output of using GPT3 with Python](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/02/output-of-using-gpt3-with-python.jpg)

## GPT-3 Has Many Interesting Applications

 You can use GPT-3 to accomplish some pretty amazing feats. You use it as a chatbot that will give you fresh realistic answers on every prompt. You can generate poems, scripts, stories, slogans, essays, headlines, and a lot more. You can even summarize long pieces of text, generate code, converse infinitely, and get conversation based on past prompts as well.

 On the flip side, the API is cloud-hosted, paid, and needs more fine-tuning. With the release of GPT-3.5 in the market, people will expect it to be more accurate and less biased compared to previous versions.

**SCROLL TO CONTINUE WITH CONTENT**

 CopyAI uses it to generate copywriting content for websites, blogs, advertisements, emails, and social media. Lex uses GPT-3 to answer research questions, Algolia for semantic search, and Replier to create branded replies to customer reviews. Here's how you can use OpenAI's GPT-3 model with Python to get started on building your AI-powered application.

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
<li><a href="https://youtube-zero.techidaily.com/024-approved-achieve-optimum-stability-incorrances-for-tripods-in-vlog-shoots/"><u>[New] 2024 Approved  Achieve Optimum Stability  Incorrances for Tripods in Vlog Shoots</u></a></li>
<li><a href="https://fox-boxes.techidaily.com/new-from-novice-to-expert-navigating-windows-11s-movie-maker-easily/"><u>[New] From Novice to Expert  Navigating Windows 11'S Movie Maker Easily</u></a></li>
<li><a href="https://facebook-video-files.techidaily.com/new-in-2024-invisible-vids-on-social-reveal-the-top-12-techniques-to-restore-appearance-in-23/"><u>[New] In 2024, Invisible Vids on Social? Reveal the Top 12 Techniques to Restore Appearance in '23</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/updated-in-2024-simplifying-cross-platform-sharing-instagram-and-facebook-integration/"><u>[Updated] In 2024, Simplifying Cross-Platform Sharing  Instagram & Facebook Integration</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/14-chatgpt-and-summarize-inbox-ai-driven-email-assistance/"><u>14 ChatGPT & Summarize Inbox: AI-Driven Email Assistance</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/2024-approved-mastering-dynamic-range-with-iphone-cameras/"><u>2024 Approved  Mastering Dynamic Range with iPhone Cameras</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/31-maximizing-email-potential-with-chatgpt-and-inbox-summarizers/"><u>31 Maximizing Email Potential with ChatGPT & Inbox Summarizers</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/4-ways-to-let-chatgpt-read-pdfs/"><u>4 Ways to Let ChatGPT Read PDFs</u></a></li>
<li><a href="https://ios-unlock.techidaily.com/4-ways-to-unlock-apple-iphone-14-plus-to-use-usb-accessories-without-passcode-by-drfone-ios/"><u>4 Ways to Unlock Apple iPhone 14 Plus to Use USB Accessories Without Passcode</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/4-ways-to-use-chatgpt-for-time-management/"><u>4 Ways to Use ChatGPT for Time Management</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/6-ai-powered-pdf-tools-unveiled-by-gpt/"><u>6 AI Powered PDF Tools Unveiled by GPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/6-predictable-gpt-automobile-setup-snags-and-solutions/"><u>6 Predictable GPT Automobile Setup Snags & Solutions</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/7-innovative-approaches-to-refine-gpt-interaction-quality/"><u>7 Innovative Approaches to Refine GPT Interaction Quality</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/7-parameters-that-define-quality-ai-assistants/"><u>7 Parameters That Define Quality AI Assistants</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/7-strategies-for-smoother-real-time-dialogue-with-chatgpt/"><u>7 Strategies for Smoother Real-Time Dialogue with ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-beginners-primer-on-ai/"><u>A Beginner’s Primer on AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-close-look-at-ai-dialogues-nine-major-issues-in-gpt/"><u>A Close Look at AI Dialogues: Nine Major Issues in GPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-guide-to-archive-gpt-chats-effortlessly/"><u>A Guide to Archive GPT Chats Effortlessly</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-guide-to-child-centric-chatbot-use-top-5-security-tips/"><u>A Guide to Child-Centric Chatbot Use: Top 5 Security Tips</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-leaner-approach-to-user-personas-via-chatgpt-innovation/"><u>A Leaner Approach to User Personas via ChatGPT Innovation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-practical-path-to-powerful-text-generation-with-openai/"><u>A Practical Path to Powerful Text Generation with OpenAI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-quick-primer-on-langchain-llm-tech/"><u>A Quick Primer on LangChain LLM Tech</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-step-by-step-approach-to-clearing-older-gpt-discussions/"><u>A Step-by-Step Approach to Clearing Older GPT Discussions</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-world-without-boundaries-with-gpt-4/"><u>A World Without Boundaries with GPT-4</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/academia-meets-artificial-intelligence/"><u>Academia Meets Artificial Intelligence</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721431369176-chatgpt-evolved-discover-the-features-that-matter-most/"><u>ChatGPT Evolved: Discover the Features That Matter Most</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721429031447-cyber-savvy-needed-recognize-authenticity-in-tech-titles/"><u>Cyber Savvy Needed: Recognize Authenticity in Tech Titles</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721387028276-discover-talk-directly-to-chatgpt/"><u>Discover: Talk Directly to ChatGPT</u></a></li>
<li><a href="https://review-topics.techidaily.com/does-find-my-friends-work-on-xiaomi-13t-drfone-by-drfone-virtual-android/"><u>Does find my friends work on Xiaomi 13T | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721383520275-guard-your-data-from-malware-disguised-as-ai-helpers/"><u>Guard Your Data From Malware Disguised as AI Helpers!</u></a></li>
<li><a href="https://pokemon-go-android.techidaily.com/how-and-where-to-find-a-shiny-stone-pokemon-for-honor-play-8t-drfone-by-drfone-virtual-android/"><u>How and Where to Find a Shiny Stone Pokémon For Honor Play 8T? | Dr.fone</u></a></li>
<li><a href="https://android-frp.techidaily.com/in-2024-5-quick-methods-to-bypass-poco-m6-5g-frp-by-drfone-android/"><u>In 2024, 5 Quick Methods to Bypass Poco M6 5G FRP</u></a></li>
<li><a href="https://some-guidance.techidaily.com/in-2024-top-easytime-timer-solutions-at-zero-cost/"><u>In 2024, Top EasyTime Timer Solutions at Zero Cost</u></a></li>
<li><a href="https://extra-tips.techidaily.com/innovative-approaches-to-video-voiceover-integration/"><u>Innovative Approaches to Video Voiceover Integration</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721398147316-revolutionizing-ai-communication-explore-openais-tailored-store/"><u>Revolutionizing AI Communication: Explore OpenAI’s Tailored Store</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721428001769-talk-directly-with-chatgpt/"><u>Talk Directly with ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721419017133-unlock-the-full-potential-of-your-smartphone-with-bing-ai-search/"><u>Unlock the Full Potential of Your Smartphone: With Bing AI Search.</u></a></li>
</ul></div>
