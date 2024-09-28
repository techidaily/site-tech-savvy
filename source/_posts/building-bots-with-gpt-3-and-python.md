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


