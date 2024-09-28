---
title: "Interactive AI: Blending Python and GPT-3"
date: 2024-08-10T02:10:10.291Z
updated: 2024-08-11T02:10:10.291Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Interactive AI: Blending Python and GPT-3"
excerpt: "This Article Describes Interactive AI: Blending Python and GPT-3"
thumbnail: https://thmb.techidaily.com/35506a9c5eeb39965a6739f4255f2a7fd3073f2c89e35224944b9c79ce0abec8.jpg
---

## Interactive AI: Blending Python and GPT-3

 An AI storm has swept across the world. The release of OpenAI's ChatGPT has sent developers and curious users into a frenzy. OpenAI has gathered a whopping 100 million active users within two months of its launch and people have already started building applications using it.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 CopyAI uses it to generate copywriting content for websites, blogs, advertisements, emails, and social media. Lex uses GPT-3 to answer research questions, Algolia for semantic search, and Replier to create branded replies to customer reviews. Here's how you can use OpenAI's GPT-3 model with Python to get started on building your AI-powered application.

<!-- affiliate ads begin -->
<a href="https://shop.systoolsgroup.com/affiliate.php?ACCOUNT=SYSTOOBY&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.systoolsgroup.com%3FAFFILIATE%3D108875%26RESOURCE%3D%2BSysTools%2BPDF%2BUnlocker"><img src="https://www.systoolsgroup.com/box/pdf-unlocker.png" border="0"></a>
<!-- affiliate ads end -->
## What Is GPT-3?

[OpenAI's GPT-3](https://www.makeuseof.com/how-to-use-gpt-3-openai-playground/) is the third-generation Generative Pre-trained Transformer. It is a Machine Learning model with over 175 billion parameters, almost the entire internet. This gives it immense capabilities to answer a wide range of questions and perform tasks that would otherwise take a lot of manual effort.

 Open AI has developed a Python module that contains pre-defined compatible classes to interact with its APIs. To install it on your system, open a terminal and run:

`pip install openai`

 If you're wondering what GPT-3 is capable of, then you can explore some of the [creative uses for GPT-3 in OpenAI Playground](https://www.makeuseof.com/creative-uses-for-gpt-3-openai-playground/).

<!-- affiliate ads begin -->
<a href="https://store.absolute.com/order/checkout.php?PRODS=4601998&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/ef70e26a0b5da778eda3f48014d087cd/728x90_larger-shield.jpg" border="0"></a>
<!-- affiliate ads end -->
## Generating the API Key

 To use GPT-3 with Python you need to generate an API key. To view your API key, follow these steps:

1. Sign up for an account on the [OpenAI page](https://platform.openai.com/overview). Select the account type as **Personal**.
2. Click on your profile and select the **View API Keys** button.  
<!-- affiliate ads begin -->
<a href="https://store.movavi.com/affiliate.php?ACCOUNT=MOVAVI&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.movavi.com%3FAFFILIATE%3D108875%26RESOURCE%3DMovavi%2BVideo%2BEditor%2Bbox"><img src="https://mcusercontent.com/0885a03ded3d480dca9287f12/images/6d3207fd-9f15-4c21-f0ad-59c68e6a7e2a.png" border="0"></a>
<!-- affiliate ads end -->
![View API Key of OpenAI website](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/02/view-api-key-of-openai-website-1.jpg)
3. Click on **Create new secret key** to generate your API key.  
<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4537546&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/4b0a0290ad7df100b77e86839989a75e/products/7_copy_2_2_hdpro.png" border="0">HD Video Converter Factory Pro</a>
<!-- affiliate ads end -->
![Create Secret API Screen of OpenAI website](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/02/create-secret-api-screen-of-openai-website.jpg)
4. Copy your API key and keep it in a secure location as you won't be able to view it again.

 OpenAI's GPT-3 API charges you based on the number of tokens (words) you use to interact with it. Luckily, OpenAI provides $18 of credit for free for the first three months, so you can explore it and experiment according to your needs.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4699091&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/bccefcc1b1eee9eca3ae4f5c1a281482/products/1_jutoh-logo-1200x1600.jpg" border="0">Jutoh Plus -  Jutoh is an ebook creator for Epub, Kindle and more. It's fast, runs on Windows, Mac, and Linux, comes with a cover design editor, and allows book variations to be created with alternate text, style sheets and cover designs. Jutoh Plus adds scripting so you can automate ebook import and creation operations. It also allows customisation of ebook HTML via templates and source code documents; and you can create Windows CHM and wxWidgets HTB help files. </a>
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

## The Output of Your GPT-3-Enabled Python Program

 When you run the program, it will ask you to enter a question. On entering the prompt, "Write a poem in 5 lines about how Iron Man is the greatest superhero of all time," the program produced the following impressive output:

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2087394/7443" target="_top" id="2087394"><img src="//a.impactradius-go.com/display-ad/7443-2087394" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2087394/7443" style="position:absolute;visibility:hidden;" border="0" />
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


