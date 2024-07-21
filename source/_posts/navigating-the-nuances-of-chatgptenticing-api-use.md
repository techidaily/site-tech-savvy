---
title: Navigating the Nuances of ChatGPT'enticing API Use
date: 2024-07-20T06:23:03.933Z
updated: 2024-07-21T06:23:03.933Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Navigating the Nuances of ChatGPT'enticing API Use
excerpt: This Article Describes Navigating the Nuances of ChatGPT'enticing API Use
thumbnail: https://thmb.techidaily.com/0c1d83719ebb98dea5d90c27c0b6408d258894840f31fa00d9902a55d5e2ce32.jpg
---

## Navigating the Nuances of ChatGPT'enticing API Use

<!-- affiliate ads begin -->
<a href="https://versadesk.pxf.io/c/5597632/1892107/21290" target="_top" id="1892107"><img src="//a.impactradius-go.com/display-ad/21290-1892107" border="0" alt="" width="1200" height="628"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1892107/21290" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
### Key Takeaways

* OpenAI has released the ChatGPT API, allowing developers to integrate ChatGPT's capabilities into their applications.
* To get started, you’ll need an OpenAI API key and a development environment with the official libraries.
* You can use the ChatGPT API for both chat completion and text completion tasks, opening up possibilities for various applications.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 With the release of its API, OpenAI has opened up the capabilities of ChatGPT to everyone. You can now seamlessly integrate ChatGPT's features into your application.

 Follow these steps to get started, whether you're looking to integrate ChatGPT into your existing application or develop new applications with it.

## 1\. Getting an OpenAI API Key

 To start using the ChatGPT API, you need to obtain an API key.

1. Sign up or log in to the official [OpenAI](https://platform.openai.com/signup) platform.
2. Once you're logged in, click on the **API keys** tab in the left pane.
3. Next, click on the **Create new secret key** button to generate the API key.
4. You won't be able to view the API key again, so copy it and store it somewhere safe.  
<!-- affiliate ads begin -->
<a href="https://imp.i110150.net/c/5597632/924299/11305" target="_top" id="924299"><img src="//a.impactradius-go.com/display-ad/11305-924299" border="0" alt="" width="520" height="100"/></a>
<!-- affiliate ads end -->
![OpenAI API Key Page](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2024/02/openai-api-key-page.png)

 The code used in this project is available in a [GitHub repository](https://github.com/makeuseofcode/ChatGPT-API-Sample-Code) and is free for you to use under the MIT license.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=45152835&QTY=1&AFFILIATE=108875&CART=1"><img src="https://download.terabyteunlimited.com/banners/ad_800x450_d.jpg" border="0"></a>
<!-- affiliate ads end -->
## 2\. Setting Up the Development Environment

 You can use the API endpoint directly or take advantage of the **openai** Python/JavaScript library to start building ChatGPT API-powered applications. This guide uses Python and the [openai-python](https://github.com/openai/openai-python) library.

 To get started:

1. [Create a Python virtual environment](https://www.makeuseof.com/create-manage-python-virtual-environments/)
2. Install the openai and **python-dotenv** libraries via pip:  
`pip install openai python-dotenv`
3. [Create a **.env** file](https://www.makeuseof.com/dotenv-file-read-data-python-nodejs-golang/) in the root of your project directory to store your API key securely.
4. Next, in the same file, set the **OPENAI\_API\_KEY** variable with the key value that you copied earlier:  
`OPENAI_API_KEY="YOUR_API_KEY"`

 Make sure you do not accidentally share your API key via version control. [Add a .gitignore file](https://www.makeuseof.com/what-is-a-gitignore-file-and-how-can-you-make-one/) to your project’s root directory and add ".env" to it to ignore the dotenv file.

<!-- affiliate ads begin -->
<a href="https://ukaidot.sjv.io/c/5597632/1793233/19578" target="_top" id="1793233"><img src="//a.impactradius-go.com/display-ad/19578-1793233" border="0" alt="" width="1200" height="1200"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1793233/19578" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## 3\. Making ChatGPT API Requests

 The OpenAI API's GPT-3.5 Turbo, GPT-4, and GPT-4 Turbo are the same models that ChatGPT uses. These powerful models are capable of understanding and generating natural language text and code. GPT-4 Turbo can even process image inputs which opens the gates for several uses including analyzing images, parsing documents with figures, and transcribing text from images.

 Please note that the ChatGPT API is a general term that refers to OpenAI APIs that use GPT-based models, including the **gpt-3.5-turbo**, **gpt-4**, and **gpt-4-turbo** models.

 The ChatGPT API is primarily optimized for chat but it also works well for text completion tasks. Whether you want to generate code, translate languages, or draft documents, this API can handle it all.

 To get access to the GPT-4 API, you need to make a successful payment of $1 or more. Otherwise, you might get an error similar to "The model \`gpt-4\` does not exist or you do not have access to it."

<!-- affiliate ads begin -->
<a href="https://twopages.pxf.io/c/5597632/1873313/18544" target="_top" id="1873313"><img src="//a.impactradius-go.com/display-ad/18544-1873313" border="0" alt="" width="1080" height="1263"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1873313/18544" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
### Using the API for Chat Completion

 You need to configure the chat model to get it ready for an API call. Here’s an example:

`from openai import OpenAI  
from dotenv import load_dotenv  
  
load_dotenv()  
client = OpenAI()  
  
response = client.chat.completions.create(  
  model = "gpt-3.5-turbo-0125",  
  temperature = 0.8,  
  max_tokens = 3000,  
  response_format={ "type": "json_object" },  
  messages = [  
    {"role": "system", "content": "You are a funny comedian who tells dad jokes. The output should be in JSON format."},  
    {"role": "user", "content": "Write a dad joke related to numbers."},  
    {"role": "assistant", "content": "Q: How do you make 7 even? A: Take away the s."},  
    {"role": "user", "content": "Write one related to programmers."}  
  ]  
)`

 The ChatGPT API sends a response in the following format:

![ChatGPT API output response format](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2024/02/chatgpt-api-output-response-format.jpg)

 You can extract the content from the response, as a JSON string, with this code:

`print(response.choices [0].message.content)`

 Running this code produces the following output:

<!-- affiliate ads begin -->
<a href="https://aidotcom.pxf.io/c/5597632/2086436/19576" target="_top" id="2086436"><img src="//a.impactradius-go.com/display-ad/19576-2086436" border="0" alt="" width="1500" height="400"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2086436/19576" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![Programming joke output generated via Chat Completions API](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2024/02/programming-joke-output-generated-via-chat-completions-api.jpg)

 The code demonstrates a ChatGPT API call using Python. Note that the model understood the context ("dad joke") and the type of response (Q&A form) that we were expecting, based on the prompts fed to it.

 The most significant part of the configuration is the **messages** parameter which accepts an array of message objects. Each message object contains a **role** and **content**. You can use three types of roles:

* **system** which sets up the context and behavior of the assistant.
* **user** which gives instructions to the assistant. The end user will typically provide this, but you can also provide some default user prompts in advance.
* **assistant** which can include example responses.

![ChatGPT API Roles Diagram](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/wm/2024/02/chatgpt-api-roles-diagram-1-1.jpg)

 You can further customize the **temperature** and **max\_tokens** parameters of the model to get the output according to your requirements.

 The higher the temperature, the higher the randomness of the output, and vice-versa. If you want your responses to be more focused and deterministic, go for the lower temperature value. And if you want it to be more creative, use a higher value. The temperature value ranges between 0 and 2\.

![Temperature parameter of ChatGPT API](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/temperature-parameter-of-chatgpt-api-3.jpg)

 Like ChatGPT, the API also has a word limit. Use the **max\_tokens** parameter to limit the length of responses. Be aware that setting a lower **max\_tokens** value can cause issues as it may cut off the output mid-way.

 At the time of writing, the **gpt-3.5-turbo** model has a token limit of 4,096, while **gpt-4**'s is 8,192\. The latest **gpt-3.5-turbo-0125** and **gpt-4-turbo-preview** models have limits of 16,385 and 128,000 respectively.

 After high demand from developers, OpenAI has introduced JSON mode which instructs the model to always return a JSON object. You can enable JSON mode by setting **response\_format** to **{ "type": "json\_object" }**. Currently, this feature is only available to the latest models: gpt-3.5-turbo-0125 and gpt-4-turbo-preview.

 You can further configure the model using the other parameters provided by [OpenAI](https://platform.openai.com/docs/api-reference/chat/create).

<!-- affiliate ads begin -->
<a href="https://shop.pcdj.com/order/checkout.php?PRODS=4698827&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/47f4b6321e9fd8e8f7326a6adc1a7c1e/products/dex3REpage-newmainscreenshot.png" border="0">DEX 3 RE is Easy-To-Use DJ Mixing Software for MAC and Windows Designed for Today's Versatile DJ. 

 Mix from your own library of music, iTunes or use the Pulselocker subsciprtion service for in-app access to over 44 million songs. Use with over 85 supported DJ controllers or mix with a keyboard and mouse.  

 DEX 3 RE is everything you need without the clutter - the perfect 2-deck mixing software solution for mobile DJs or hard-core hobbiests.  
 PCDJ DEX 3 RE (DJ Software for Win & MAC - Product Activation For 3 Machines)</a>
<!-- affiliate ads end -->
### Using the ChatGPT API for Text Completion

 In addition to multi-turn conversation tasks, the Chat Completions API (ChatGPT API) does a good job with text completion. The following example demonstrates how you can configure the ChatGPT API for text completion:

`  
from openai import OpenAI  
from dotenv import load_dotenv  
  
load_dotenv()  
client = OpenAI()  
  
response = client.chat.completions.create(  
  model = "gpt-3.5-turbo",  
  temperature = 0.8,  
  max_tokens = 3000,  
  messages = [  
    {"role": "system", "content": "You are a poet who creates poems that evoke emotions."},  
    {"role": "user", "content": "Write a short poem for programmers."}  
  ]  
)  
  
print(response.choices [0].message.content)`

 You don't even need to provide the system role and its content. Providing just the user prompt will do the work for you.

`messages = [  
  {"role": "user", "content": "Write a short poem for programmers."}  
]`

 Running the above code will generate a poem for programmers, for example:

![A poem on programmers](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/a-poem-on-programmers.jpg)

## ChatGPT API Pricing

 The ChatGPT API pricing is based on the "price per 1,000 tokens" model. For chat completion requests, the cost is calculated based on the number of input tokens plus the number of output tokens returned by the API. In layman's terms, tokens are equivalent to pieces of words, where 1,000 tokens are approximately equal to 750 words.

| **Model**                 | **Input**           | **Output**          |
| ------------------------- | ------------------- | ------------------- |
| gpt-4-0125-preview        | $0.01 / 1K tokens   | $0.03 / 1K tokens   |
| gpt-4-1106-preview        | $0.01 / 1K tokens   | $0.03 / 1K tokens   |
| gpt-4-1106-vision-preview | $0.01 / 1K tokens   | $0.03 / 1K tokens   |
| gpt-4                     | $0.03 / 1K tokens   | $0.06 / 1K tokens   |
| gpt-4-32k                 | $0.06 / 1K tokens   | $0.12 / 1K tokens   |
| gpt-3.5-turbo-0125        | $0.0005 / 1K tokens | $0.0015 / 1K tokens |
| gpt-3.5-turbo-instruct    | $0.0015 / 1K tokens | $0.0020 / 1K tokens |

 Note that the pricing may change over time with improvements in the model.

## Build Next Generation Apps Using the ChatGPT API

 The ChatGPT API has opened gates for developers around the world to build innovative products with the power of AI.

 You can use this tool to develop applications like story writers, code translators, marketing copy generators, and text summarizers. Your imagination is the limit to building applications using this technology.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 With the release of its API, OpenAI has opened up the capabilities of ChatGPT to everyone. You can now seamlessly integrate ChatGPT's features into your application.

 Follow these steps to get started, whether you're looking to integrate ChatGPT into your existing application or develop new applications with it.

## 1\. Getting an OpenAI API Key

 To start using the ChatGPT API, you need to obtain an API key.

1. Sign up or log in to the official [OpenAI](https://platform.openai.com/signup) platform.
2. Once you're logged in, click on the **API keys** tab in the left pane.
3. Next, click on the **Create new secret key** button to generate the API key.
4. You won't be able to view the API key again, so copy it and store it somewhere safe.  
![OpenAI API Key Page](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2024/02/openai-api-key-page.png)

 The code used in this project is available in a [GitHub repository](https://github.com/makeuseofcode/ChatGPT-API-Sample-Code) and is free for you to use under the MIT license.

## 2\. Setting Up the Development Environment

 You can use the API endpoint directly or take advantage of the **openai** Python/JavaScript library to start building ChatGPT API-powered applications. This guide uses Python and the [openai-python](https://github.com/openai/openai-python) library.

 To get started:

1. [Create a Python virtual environment](https://www.makeuseof.com/create-manage-python-virtual-environments/)
2. Install the openai and **python-dotenv** libraries via pip:  
`pip install openai python-dotenv`
3. [Create a **.env** file](https://www.makeuseof.com/dotenv-file-read-data-python-nodejs-golang/) in the root of your project directory to store your API key securely.
4. Next, in the same file, set the **OPENAI\_API\_KEY** variable with the key value that you copied earlier:  
`OPENAI_API_KEY="YOUR_API_KEY"`

 Make sure you do not accidentally share your API key via version control. [Add a .gitignore file](https://www.makeuseof.com/what-is-a-gitignore-file-and-how-can-you-make-one/) to your project’s root directory and add ".env" to it to ignore the dotenv file.

## 3\. Making ChatGPT API Requests

 The OpenAI API's GPT-3.5 Turbo, GPT-4, and GPT-4 Turbo are the same models that ChatGPT uses. These powerful models are capable of understanding and generating natural language text and code. GPT-4 Turbo can even process image inputs which opens the gates for several uses including analyzing images, parsing documents with figures, and transcribing text from images.

 Please note that the ChatGPT API is a general term that refers to OpenAI APIs that use GPT-based models, including the **gpt-3.5-turbo**, **gpt-4**, and **gpt-4-turbo** models.

 The ChatGPT API is primarily optimized for chat but it also works well for text completion tasks. Whether you want to generate code, translate languages, or draft documents, this API can handle it all.

 To get access to the GPT-4 API, you need to make a successful payment of $1 or more. Otherwise, you might get an error similar to "The model \`gpt-4\` does not exist or you do not have access to it."

### Using the API for Chat Completion

 You need to configure the chat model to get it ready for an API call. Here’s an example:

`from openai import OpenAI  
from dotenv import load_dotenv  
  
load_dotenv()  
client = OpenAI()  
  
response = client.chat.completions.create(  
  model = "gpt-3.5-turbo-0125",  
  temperature = 0.8,  
  max_tokens = 3000,  
  response_format={ "type": "json_object" },  
  messages = [  
    {"role": "system", "content": "You are a funny comedian who tells dad jokes. The output should be in JSON format."},  
    {"role": "user", "content": "Write a dad joke related to numbers."},  
    {"role": "assistant", "content": "Q: How do you make 7 even? A: Take away the s."},  
    {"role": "user", "content": "Write one related to programmers."}  
  ]  
)`

 The ChatGPT API sends a response in the following format:

<!-- affiliate ads begin -->
<a href="https://store.bitdefender.com/affiliate.php?ACCOUNT=BITLATIN&AFFILIATE=108875&PATH=http%3A%2F%2Fwww.bitdefender.com%2Fbusiness%3FAFFILIATE%3D108875%26RESOURCE%3D30%2525%2BOff%2Ball%2BGravityZone%2BProducts"><img src="https://www.bitdefender.com/content/dam/bitdefender/business/campaign/1200X628.png" border="0"></a>
<!-- affiliate ads end -->
![ChatGPT API output response format](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2024/02/chatgpt-api-output-response-format.jpg)

 You can extract the content from the response, as a JSON string, with this code:

`print(response.choices [0].message.content)`

 Running this code produces the following output:

![Programming joke output generated via Chat Completions API](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2024/02/programming-joke-output-generated-via-chat-completions-api.jpg)

 The code demonstrates a ChatGPT API call using Python. Note that the model understood the context ("dad joke") and the type of response (Q&A form) that we were expecting, based on the prompts fed to it.

 The most significant part of the configuration is the **messages** parameter which accepts an array of message objects. Each message object contains a **role** and **content**. You can use three types of roles:

* **system** which sets up the context and behavior of the assistant.
* **user** which gives instructions to the assistant. The end user will typically provide this, but you can also provide some default user prompts in advance.
* **assistant** which can include example responses.

![ChatGPT API Roles Diagram](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/wm/2024/02/chatgpt-api-roles-diagram-1-1.jpg)

 You can further customize the **temperature** and **max\_tokens** parameters of the model to get the output according to your requirements.

 The higher the temperature, the higher the randomness of the output, and vice-versa. If you want your responses to be more focused and deterministic, go for the lower temperature value. And if you want it to be more creative, use a higher value. The temperature value ranges between 0 and 2\.

<!-- affiliate ads begin -->
<a href="https://twopages.pxf.io/c/5597632/2016067/18544" target="_top" id="2016067"><img src="//a.impactradius-go.com/display-ad/18544-2016067" border="0" alt="" width="1020" height="380"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2016067/18544" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![Temperature parameter of ChatGPT API](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/temperature-parameter-of-chatgpt-api-3.jpg)

 Like ChatGPT, the API also has a word limit. Use the **max\_tokens** parameter to limit the length of responses. Be aware that setting a lower **max\_tokens** value can cause issues as it may cut off the output mid-way.

 At the time of writing, the **gpt-3.5-turbo** model has a token limit of 4,096, while **gpt-4**'s is 8,192\. The latest **gpt-3.5-turbo-0125** and **gpt-4-turbo-preview** models have limits of 16,385 and 128,000 respectively.

 After high demand from developers, OpenAI has introduced JSON mode which instructs the model to always return a JSON object. You can enable JSON mode by setting **response\_format** to **{ "type": "json\_object" }**. Currently, this feature is only available to the latest models: gpt-3.5-turbo-0125 and gpt-4-turbo-preview.

 You can further configure the model using the other parameters provided by [OpenAI](https://platform.openai.com/docs/api-reference/chat/create).

<!-- affiliate ads begin -->
<a href="https://estore.winxdvd.com/order/checkout.php?PRODS=1412049&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.winxdvd.com/affiliate/new-banner/pt-200x200.jpg" border="0"></a>
<!-- affiliate ads end -->
### Using the ChatGPT API for Text Completion

 In addition to multi-turn conversation tasks, the Chat Completions API (ChatGPT API) does a good job with text completion. The following example demonstrates how you can configure the ChatGPT API for text completion:

`  
from openai import OpenAI  
from dotenv import load_dotenv  
  
load_dotenv()  
client = OpenAI()  
  
response = client.chat.completions.create(  
  model = "gpt-3.5-turbo",  
  temperature = 0.8,  
  max_tokens = 3000,  
  messages = [  
    {"role": "system", "content": "You are a poet who creates poems that evoke emotions."},  
    {"role": "user", "content": "Write a short poem for programmers."}  
  ]  
)  
  
print(response.choices [0].message.content)`

 You don't even need to provide the system role and its content. Providing just the user prompt will do the work for you.

`messages = [  
  {"role": "user", "content": "Write a short poem for programmers."}  
]`

 Running the above code will generate a poem for programmers, for example:

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2068416/7443" target="_top" id="2068416"><img src="//a.impactradius-go.com/display-ad/7443-2068416" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2068416/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![A poem on programmers](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/a-poem-on-programmers.jpg)

<!-- affiliate ads begin -->
<a href="https://godlikehost.sjv.io/c/5597632/1920054/21774" target="_top" id="1920054"><img src="//a.impactradius-go.com/display-ad/21774-1920054" border="0" alt="" width="320" height="100"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1920054/21774" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## ChatGPT API Pricing

 The ChatGPT API pricing is based on the "price per 1,000 tokens" model. For chat completion requests, the cost is calculated based on the number of input tokens plus the number of output tokens returned by the API. In layman's terms, tokens are equivalent to pieces of words, where 1,000 tokens are approximately equal to 750 words.

| **Model**                 | **Input**           | **Output**          |
| ------------------------- | ------------------- | ------------------- |
| gpt-4-0125-preview        | $0.01 / 1K tokens   | $0.03 / 1K tokens   |
| gpt-4-1106-preview        | $0.01 / 1K tokens   | $0.03 / 1K tokens   |
| gpt-4-1106-vision-preview | $0.01 / 1K tokens   | $0.03 / 1K tokens   |
| gpt-4                     | $0.03 / 1K tokens   | $0.06 / 1K tokens   |
| gpt-4-32k                 | $0.06 / 1K tokens   | $0.12 / 1K tokens   |
| gpt-3.5-turbo-0125        | $0.0005 / 1K tokens | $0.0015 / 1K tokens |
| gpt-3.5-turbo-instruct    | $0.0015 / 1K tokens | $0.0020 / 1K tokens |

 Note that the pricing may change over time with improvements in the model.

## Build Next Generation Apps Using the ChatGPT API

 The ChatGPT API has opened gates for developers around the world to build innovative products with the power of AI.

 You can use this tool to develop applications like story writers, code translators, marketing copy generators, and text summarizers. Your imagination is the limit to building applications using this technology.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 With the release of its API, OpenAI has opened up the capabilities of ChatGPT to everyone. You can now seamlessly integrate ChatGPT's features into your application.

 Follow these steps to get started, whether you're looking to integrate ChatGPT into your existing application or develop new applications with it.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4742929&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/e09fdffe648a30658a9657bbed7b2388/products/boxshot(2).png" border="0">Kanto Player Professional</a>
<!-- affiliate ads end -->
## 1\. Getting an OpenAI API Key

 To start using the ChatGPT API, you need to obtain an API key.

1. Sign up or log in to the official [OpenAI](https://platform.openai.com/signup) platform.
2. Once you're logged in, click on the **API keys** tab in the left pane.
3. Next, click on the **Create new secret key** button to generate the API key.
4. You won't be able to view the API key again, so copy it and store it somewhere safe.  
![OpenAI API Key Page](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2024/02/openai-api-key-page.png)

 The code used in this project is available in a [GitHub repository](https://github.com/makeuseofcode/ChatGPT-API-Sample-Code) and is free for you to use under the MIT license.

## 2\. Setting Up the Development Environment

 You can use the API endpoint directly or take advantage of the **openai** Python/JavaScript library to start building ChatGPT API-powered applications. This guide uses Python and the [openai-python](https://github.com/openai/openai-python) library.

 To get started:

1. [Create a Python virtual environment](https://www.makeuseof.com/create-manage-python-virtual-environments/)
2. Install the openai and **python-dotenv** libraries via pip:  
`pip install openai python-dotenv`
3. [Create a **.env** file](https://www.makeuseof.com/dotenv-file-read-data-python-nodejs-golang/) in the root of your project directory to store your API key securely.
4. Next, in the same file, set the **OPENAI\_API\_KEY** variable with the key value that you copied earlier:  
`OPENAI_API_KEY="YOUR_API_KEY"`

 Make sure you do not accidentally share your API key via version control. [Add a .gitignore file](https://www.makeuseof.com/what-is-a-gitignore-file-and-how-can-you-make-one/) to your project’s root directory and add ".env" to it to ignore the dotenv file.

## 3\. Making ChatGPT API Requests

 The OpenAI API's GPT-3.5 Turbo, GPT-4, and GPT-4 Turbo are the same models that ChatGPT uses. These powerful models are capable of understanding and generating natural language text and code. GPT-4 Turbo can even process image inputs which opens the gates for several uses including analyzing images, parsing documents with figures, and transcribing text from images.

 Please note that the ChatGPT API is a general term that refers to OpenAI APIs that use GPT-based models, including the **gpt-3.5-turbo**, **gpt-4**, and **gpt-4-turbo** models.

 The ChatGPT API is primarily optimized for chat but it also works well for text completion tasks. Whether you want to generate code, translate languages, or draft documents, this API can handle it all.

 To get access to the GPT-4 API, you need to make a successful payment of $1 or more. Otherwise, you might get an error similar to "The model \`gpt-4\` does not exist or you do not have access to it."

### Using the API for Chat Completion

 You need to configure the chat model to get it ready for an API call. Here’s an example:

`from openai import OpenAI  
from dotenv import load_dotenv  
  
load_dotenv()  
client = OpenAI()  
  
response = client.chat.completions.create(  
  model = "gpt-3.5-turbo-0125",  
  temperature = 0.8,  
  max_tokens = 3000,  
  response_format={ "type": "json_object" },  
  messages = [  
    {"role": "system", "content": "You are a funny comedian who tells dad jokes. The output should be in JSON format."},  
    {"role": "user", "content": "Write a dad joke related to numbers."},  
    {"role": "assistant", "content": "Q: How do you make 7 even? A: Take away the s."},  
    {"role": "user", "content": "Write one related to programmers."}  
  ]  
)`

 The ChatGPT API sends a response in the following format:

<!-- affiliate ads begin -->
<a href="https://shop.emeditor.com/order/checkout.php?PRODS=4610657&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.emeditor.com/wp-content/uploads/2024/06/emeditor_chat_ai.png" border="0">
EmEditor is a fast, lightweight, yet extensible, easy-to-use text editor, code editor, CSV editor, and large file viewer for Windows. Both native 64-bit and 32-bit builds are available, and moreover, the 64-bit includes separate builds for SSE2 (128-bit), AVX-2 (256-bit), and AVX-512 (512-bit) instruction sets. New versions support AI-assisted writing.</a>
<!-- affiliate ads end -->
![ChatGPT API output response format](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2024/02/chatgpt-api-output-response-format.jpg)

 You can extract the content from the response, as a JSON string, with this code:

`print(response.choices [0].message.content)`

 Running this code produces the following output:

![Programming joke output generated via Chat Completions API](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2024/02/programming-joke-output-generated-via-chat-completions-api.jpg)

 The code demonstrates a ChatGPT API call using Python. Note that the model understood the context ("dad joke") and the type of response (Q&A form) that we were expecting, based on the prompts fed to it.

 The most significant part of the configuration is the **messages** parameter which accepts an array of message objects. Each message object contains a **role** and **content**. You can use three types of roles:

* **system** which sets up the context and behavior of the assistant.
* **user** which gives instructions to the assistant. The end user will typically provide this, but you can also provide some default user prompts in advance.
* **assistant** which can include example responses.

<!-- affiliate ads begin -->
<a href="https://shop.mondly.com/affiliate.php?ACCOUNT=ATISTUDI&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.mondly.com%3FAFFILIATE%3D108875%26RESOURCE%3D%2BEducational%2B300x600%2B"><img src="https://secure.avangate.com/images/merchant/69c418c33ec2e1a4267fa9bb77fa1428/educational-300x600.gif" border="0"></a>
<!-- affiliate ads end -->
![ChatGPT API Roles Diagram](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/wm/2024/02/chatgpt-api-roles-diagram-1-1.jpg)

 You can further customize the **temperature** and **max\_tokens** parameters of the model to get the output according to your requirements.

 The higher the temperature, the higher the randomness of the output, and vice-versa. If you want your responses to be more focused and deterministic, go for the lower temperature value. And if you want it to be more creative, use a higher value. The temperature value ranges between 0 and 2\.

![Temperature parameter of ChatGPT API](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/temperature-parameter-of-chatgpt-api-3.jpg)

 Like ChatGPT, the API also has a word limit. Use the **max\_tokens** parameter to limit the length of responses. Be aware that setting a lower **max\_tokens** value can cause issues as it may cut off the output mid-way.

 At the time of writing, the **gpt-3.5-turbo** model has a token limit of 4,096, while **gpt-4**'s is 8,192\. The latest **gpt-3.5-turbo-0125** and **gpt-4-turbo-preview** models have limits of 16,385 and 128,000 respectively.

 After high demand from developers, OpenAI has introduced JSON mode which instructs the model to always return a JSON object. You can enable JSON mode by setting **response\_format** to **{ "type": "json\_object" }**. Currently, this feature is only available to the latest models: gpt-3.5-turbo-0125 and gpt-4-turbo-preview.

 You can further configure the model using the other parameters provided by [OpenAI](https://platform.openai.com/docs/api-reference/chat/create).

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=33729450&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/7f687767ccf20fcea1c9dc4a5adc2326/Digisigner_banner_728_x_90_color_version.png" border="0"></a>
<!-- affiliate ads end -->
### Using the ChatGPT API for Text Completion

 In addition to multi-turn conversation tasks, the Chat Completions API (ChatGPT API) does a good job with text completion. The following example demonstrates how you can configure the ChatGPT API for text completion:

`  
from openai import OpenAI  
from dotenv import load_dotenv  
  
load_dotenv()  
client = OpenAI()  
  
response = client.chat.completions.create(  
  model = "gpt-3.5-turbo",  
  temperature = 0.8,  
  max_tokens = 3000,  
  messages = [  
    {"role": "system", "content": "You are a poet who creates poems that evoke emotions."},  
    {"role": "user", "content": "Write a short poem for programmers."}  
  ]  
)  
  
print(response.choices [0].message.content)`

 You don't even need to provide the system role and its content. Providing just the user prompt will do the work for you.

`messages = [  
  {"role": "user", "content": "Write a short poem for programmers."}  
]`

 Running the above code will generate a poem for programmers, for example:

<!-- affiliate ads begin -->
<a href="https://shop.mondly.com/affiliate.php?ACCOUNT=ATISTUDI&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.mondly.com%3FAFFILIATE%3D108875%26RESOURCE%3D%2BGeneral%2B970x90%2B"><img src="https://secure.avangate.com/images/merchant/69c418c33ec2e1a4267fa9bb77fa1428/general-970x90.gif" border="0"></a>
<!-- affiliate ads end -->
![A poem on programmers](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/a-poem-on-programmers.jpg)

## ChatGPT API Pricing

 The ChatGPT API pricing is based on the "price per 1,000 tokens" model. For chat completion requests, the cost is calculated based on the number of input tokens plus the number of output tokens returned by the API. In layman's terms, tokens are equivalent to pieces of words, where 1,000 tokens are approximately equal to 750 words.

| **Model**                 | **Input**           | **Output**          |
| ------------------------- | ------------------- | ------------------- |
| gpt-4-0125-preview        | $0.01 / 1K tokens   | $0.03 / 1K tokens   |
| gpt-4-1106-preview        | $0.01 / 1K tokens   | $0.03 / 1K tokens   |
| gpt-4-1106-vision-preview | $0.01 / 1K tokens   | $0.03 / 1K tokens   |
| gpt-4                     | $0.03 / 1K tokens   | $0.06 / 1K tokens   |
| gpt-4-32k                 | $0.06 / 1K tokens   | $0.12 / 1K tokens   |
| gpt-3.5-turbo-0125        | $0.0005 / 1K tokens | $0.0015 / 1K tokens |
| gpt-3.5-turbo-instruct    | $0.0015 / 1K tokens | $0.0020 / 1K tokens |

 Note that the pricing may change over time with improvements in the model.

## Build Next Generation Apps Using the ChatGPT API

 The ChatGPT API has opened gates for developers around the world to build innovative products with the power of AI.

 You can use this tool to develop applications like story writers, code translators, marketing copy generators, and text summarizers. Your imagination is the limit to building applications using this technology.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 With the release of its API, OpenAI has opened up the capabilities of ChatGPT to everyone. You can now seamlessly integrate ChatGPT's features into your application.

 Follow these steps to get started, whether you're looking to integrate ChatGPT into your existing application or develop new applications with it.

## 1\. Getting an OpenAI API Key

 To start using the ChatGPT API, you need to obtain an API key.

1. Sign up or log in to the official [OpenAI](https://platform.openai.com/signup) platform.
2. Once you're logged in, click on the **API keys** tab in the left pane.
3. Next, click on the **Create new secret key** button to generate the API key.
4. You won't be able to view the API key again, so copy it and store it somewhere safe.  
![OpenAI API Key Page](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2024/02/openai-api-key-page.png)

 The code used in this project is available in a [GitHub repository](https://github.com/makeuseofcode/ChatGPT-API-Sample-Code) and is free for you to use under the MIT license.

## 2\. Setting Up the Development Environment

 You can use the API endpoint directly or take advantage of the **openai** Python/JavaScript library to start building ChatGPT API-powered applications. This guide uses Python and the [openai-python](https://github.com/openai/openai-python) library.

 To get started:

1. [Create a Python virtual environment](https://www.makeuseof.com/create-manage-python-virtual-environments/)
2. Install the openai and **python-dotenv** libraries via pip:  
`pip install openai python-dotenv`
3. [Create a **.env** file](https://www.makeuseof.com/dotenv-file-read-data-python-nodejs-golang/) in the root of your project directory to store your API key securely.
4. Next, in the same file, set the **OPENAI\_API\_KEY** variable with the key value that you copied earlier:  
`OPENAI_API_KEY="YOUR_API_KEY"`

 Make sure you do not accidentally share your API key via version control. [Add a .gitignore file](https://www.makeuseof.com/what-is-a-gitignore-file-and-how-can-you-make-one/) to your project’s root directory and add ".env" to it to ignore the dotenv file.

## 3\. Making ChatGPT API Requests

 The OpenAI API's GPT-3.5 Turbo, GPT-4, and GPT-4 Turbo are the same models that ChatGPT uses. These powerful models are capable of understanding and generating natural language text and code. GPT-4 Turbo can even process image inputs which opens the gates for several uses including analyzing images, parsing documents with figures, and transcribing text from images.

 Please note that the ChatGPT API is a general term that refers to OpenAI APIs that use GPT-based models, including the **gpt-3.5-turbo**, **gpt-4**, and **gpt-4-turbo** models.

 The ChatGPT API is primarily optimized for chat but it also works well for text completion tasks. Whether you want to generate code, translate languages, or draft documents, this API can handle it all.

 To get access to the GPT-4 API, you need to make a successful payment of $1 or more. Otherwise, you might get an error similar to "The model \`gpt-4\` does not exist or you do not have access to it."

<!-- affiliate ads begin -->
<a href="https://printrendy.pxf.io/c/5597632/1453719/17020" target="_top" id="1453719"><img src="//a.impactradius-go.com/display-ad/17020-1453719" border="0" alt="" width="300" height="250"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1453719/17020" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
### Using the API for Chat Completion

 You need to configure the chat model to get it ready for an API call. Here’s an example:

`from openai import OpenAI  
from dotenv import load_dotenv  
  
load_dotenv()  
client = OpenAI()  
  
response = client.chat.completions.create(  
  model = "gpt-3.5-turbo-0125",  
  temperature = 0.8,  
  max_tokens = 3000,  
  response_format={ "type": "json_object" },  
  messages = [  
    {"role": "system", "content": "You are a funny comedian who tells dad jokes. The output should be in JSON format."},  
    {"role": "user", "content": "Write a dad joke related to numbers."},  
    {"role": "assistant", "content": "Q: How do you make 7 even? A: Take away the s."},  
    {"role": "user", "content": "Write one related to programmers."}  
  ]  
)`

 The ChatGPT API sends a response in the following format:

![ChatGPT API output response format](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2024/02/chatgpt-api-output-response-format.jpg)

 You can extract the content from the response, as a JSON string, with this code:

`print(response.choices [0].message.content)`

 Running this code produces the following output:

![Programming joke output generated via Chat Completions API](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2024/02/programming-joke-output-generated-via-chat-completions-api.jpg)

 The code demonstrates a ChatGPT API call using Python. Note that the model understood the context ("dad joke") and the type of response (Q&A form) that we were expecting, based on the prompts fed to it.

 The most significant part of the configuration is the **messages** parameter which accepts an array of message objects. Each message object contains a **role** and **content**. You can use three types of roles:

* **system** which sets up the context and behavior of the assistant.
* **user** which gives instructions to the assistant. The end user will typically provide this, but you can also provide some default user prompts in advance.
* **assistant** which can include example responses.

![ChatGPT API Roles Diagram](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/wm/2024/02/chatgpt-api-roles-diagram-1-1.jpg)

 You can further customize the **temperature** and **max\_tokens** parameters of the model to get the output according to your requirements.

 The higher the temperature, the higher the randomness of the output, and vice-versa. If you want your responses to be more focused and deterministic, go for the lower temperature value. And if you want it to be more creative, use a higher value. The temperature value ranges between 0 and 2\.

<!-- affiliate ads begin -->
<a href="https://shop.mondly.com/affiliate.php?ACCOUNT=ATISTUDI&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.mondly.com%3FAFFILIATE%3D108875%26RESOURCE%3D%2BBusiness%2B970x90%2B"><img src="https://secure.avangate.com/images/merchant/69c418c33ec2e1a4267fa9bb77fa1428/business-970x90.gif" border="0"></a>
<!-- affiliate ads end -->
![Temperature parameter of ChatGPT API](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/temperature-parameter-of-chatgpt-api-3.jpg)

 Like ChatGPT, the API also has a word limit. Use the **max\_tokens** parameter to limit the length of responses. Be aware that setting a lower **max\_tokens** value can cause issues as it may cut off the output mid-way.

 At the time of writing, the **gpt-3.5-turbo** model has a token limit of 4,096, while **gpt-4**'s is 8,192\. The latest **gpt-3.5-turbo-0125** and **gpt-4-turbo-preview** models have limits of 16,385 and 128,000 respectively.

 After high demand from developers, OpenAI has introduced JSON mode which instructs the model to always return a JSON object. You can enable JSON mode by setting **response\_format** to **{ "type": "json\_object" }**. Currently, this feature is only available to the latest models: gpt-3.5-turbo-0125 and gpt-4-turbo-preview.

 You can further configure the model using the other parameters provided by [OpenAI](https://platform.openai.com/docs/api-reference/chat/create).

### Using the ChatGPT API for Text Completion

 In addition to multi-turn conversation tasks, the Chat Completions API (ChatGPT API) does a good job with text completion. The following example demonstrates how you can configure the ChatGPT API for text completion:

`  
from openai import OpenAI  
from dotenv import load_dotenv  
  
load_dotenv()  
client = OpenAI()  
  
response = client.chat.completions.create(  
  model = "gpt-3.5-turbo",  
  temperature = 0.8,  
  max_tokens = 3000,  
  messages = [  
    {"role": "system", "content": "You are a poet who creates poems that evoke emotions."},  
    {"role": "user", "content": "Write a short poem for programmers."}  
  ]  
)  
  
print(response.choices [0].message.content)`

 You don't even need to provide the system role and its content. Providing just the user prompt will do the work for you.

`messages = [  
  {"role": "user", "content": "Write a short poem for programmers."}  
]`

 Running the above code will generate a poem for programmers, for example:

<!-- affiliate ads begin -->
<a href="https://printrendy.pxf.io/c/5597632/1453720/17020" target="_top" id="1453720"><img src="//a.impactradius-go.com/display-ad/17020-1453720" border="0" alt="" width="300" height="250"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1453720/17020" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![A poem on programmers](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/a-poem-on-programmers.jpg)

<!-- affiliate ads begin -->
<a href="https://boody-eco-wear.pxf.io/c/5597632/1572622/13846" target="_top" id="1572622"><img src="//a.impactradius-go.com/display-ad/13846-1572622" border="0" alt="" width="1000" height="1298"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1572622/13846" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## ChatGPT API Pricing

 The ChatGPT API pricing is based on the "price per 1,000 tokens" model. For chat completion requests, the cost is calculated based on the number of input tokens plus the number of output tokens returned by the API. In layman's terms, tokens are equivalent to pieces of words, where 1,000 tokens are approximately equal to 750 words.

| **Model**                 | **Input**           | **Output**          |
| ------------------------- | ------------------- | ------------------- |
| gpt-4-0125-preview        | $0.01 / 1K tokens   | $0.03 / 1K tokens   |
| gpt-4-1106-preview        | $0.01 / 1K tokens   | $0.03 / 1K tokens   |
| gpt-4-1106-vision-preview | $0.01 / 1K tokens   | $0.03 / 1K tokens   |
| gpt-4                     | $0.03 / 1K tokens   | $0.06 / 1K tokens   |
| gpt-4-32k                 | $0.06 / 1K tokens   | $0.12 / 1K tokens   |
| gpt-3.5-turbo-0125        | $0.0005 / 1K tokens | $0.0015 / 1K tokens |
| gpt-3.5-turbo-instruct    | $0.0015 / 1K tokens | $0.0020 / 1K tokens |

 Note that the pricing may change over time with improvements in the model.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4620778&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/07dd4d5a72f5740ef0f035f201951476/300__250banner.jpg" border="0"></a>
<!-- affiliate ads end -->
## Build Next Generation Apps Using the ChatGPT API

 The ChatGPT API has opened gates for developers around the world to build innovative products with the power of AI.

 You can use this tool to develop applications like story writers, code translators, marketing copy generators, and text summarizers. Your imagination is the limit to building applications using this technology.

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
<li><a href="https://youtube-sure.techidaily.com/024-approved-highest-quality-screen-time-movie-hits-list/"><u>[New] 2024 Approved  Highest-Quality Screen Time  Movie Hits List</u></a></li>
<li><a href="https://facebook-video-content.techidaily.com/new-2024-approved-maximize-your-impact-strategic-approaches-to-facebook-bios/"><u>[New] 2024 Approved  Maximize Your Impact  Strategic Approaches to Facebook Bios</u></a></li>
<li><a href="https://snapchat-videos.techidaily.com/new-immediate-recovery-of-lost-snapshots/"><u>[New] Immediate Recovery of Lost Snapshots</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/updated-fl-studios-approach-to-cautious-sound-dimming/"><u>[Updated] FL Studio's Approach to Cautious Sound Dimming</u></a></li>
<li><a href="https://on-screen-recording.techidaily.com/updated-in-2024-pro-streamers-list-5-innovative-webcams-for-gamers/"><u>[Updated] In 2024, Pro Streamer's List  5 Innovative Webcams for Gamers</u></a></li>
<li><a href="https://some-approaches.techidaily.com/updated-inside-insights-proclaiming-rights-to-free-clip-art-legally/"><u>[Updated] Inside Insights  Proclaiming Rights to Free Clip Art Legally</u></a></li>
<li><a href="https://fox-boxes.techidaily.com/updated-pixelperfect-image-transformations-for-2024/"><u>[Updated] PixelPerfect Image Transformations for 2024</u></a></li>
<li><a href="https://fox-access.techidaily.com/2024-approved-formulating-fascinating-film-moments/"><u>2024 Approved  Formulating Fascinating Film Moments</u></a></li>
<li><a href="https://some-tips.techidaily.com/2024-approved-strategic-steps-for-incorporating-srt-files-into-googleplus-campaigns/"><u>2024 Approved  Strategic Steps for Incorporating SRT Files Into Google+ Campaigns</u></a></li>
<li><a href="https://fox-blue.techidaily.com/2024-approved-syncing-sound-and-visuals-a-movie-maker-technique/"><u>2024 Approved  Syncing Sound and Visuals  A Movie Maker Technique</u></a></li>
<li><a href="https://howto.techidaily.com/8-ultimate-fixes-for-google-play-your-xiaomi-civi-3-disney-100th-anniversary-edition-isnt-compatible-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>8 Ultimate Fixes for Google Play Your Xiaomi Civi 3 Disney 100th Anniversary Edition Isnt Compatible | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/a-journey-through-openais-gpt-generations/"><u>A Journey Through OpenAI’s GPT Generations</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-oversight-how-and-by-whom/"><u>AI Oversight: How & By Whom?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-driven-approaches-to-streamline-domestic-life/"><u>AI-Driven Approaches to Streamline Domestic Life</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/authenticity-alert-separating-real-from-fake-bincrypt-tokens/"><u>Authenticity Alert: Separating Real From Fake BinCrypt Tokens</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/auto-gpts-effectiveness-independent-or-not/"><u>Auto-GPT's Effectiveness: Independent or Not?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/barricade-website-from-robotic-data-collectors/"><u>Barricade Website From Robotic Data Collectors</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/becoming-an-expert-at-obs-studio-android-focus/"><u>Becoming an Expert at OBS Studio  Android Focus</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/beyond-bots-separating-truth-from-ai-mythology/"><u>Beyond Bots: Separating Truth From AI Mythology</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpts-impact-on-modern-day-job-seekers/"><u>ChatGPT's Impact on Modern-Day Job Seekers</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/crafting-your-path-to-fitness-ai-assisted-strategy/"><u>Crafting Your Path to Fitness: AI-Assisted Strategy</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/creative-catalysts-da-vincis-triumph-in-image-generation-ai/"><u>Creative Catalysts: Da Vinci’s Triumph in Image Generation AI</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/easy-steps-to-recover-deleted-videos-from-huawei-nova-y91-by-fonelab-android-recover-video/"><u>Easy steps to recover deleted videos from Huawei Nova Y91</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/elevating-ai-writing-making-chatgpt-write-like-you/"><u>Elevating AI Writing: Making ChatGPT Write Like You</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/enhanced-ai-conversations-with-siri-and-chatgpt-on-iphone/"><u>Enhanced AI Conversations with Siri and ChatGPT on iPhone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/exploring-career-trajectories-in-ai-driven-responsiveness-design/"><u>Exploring Career Trajectories in AI-Driven Responsiveness Design</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/fallacious-chrome-extension-steals-facebook-sign-in-info/"><u>Fallacious Chrome Extension: Steals FACEBOOK Sign-In Info</u></a></li>
<li><a href="https://facebook-video-content.techidaily.com/fb-video-extractor-for-pc-mobile-and-mac-for-2024/"><u>FB Video Extractor for PC, Mobile & Mac for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1721405554846-free-gpt-4-for-everyone-nonetheless-select-plus-membership-continues-to-provide-unique-services/"><u>Free GPT-4 for Everyone; Nonetheless, Select Plus Membership Continues to Provide Unique Services.</u></a></li>
<li><a href="https://youtube-stream.techidaily.com/free-high-quality-youtube-banner-samples-inside-for-2024/"><u>Free High-Quality YouTube Banner Samples Inside for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-onlyoffice-docspace-uses-chatgpt-to-improve-your-productivity/"><u>How ONLYOFFICE DocSpace Uses ChatGPT to Improve Your Productivity</u></a></li>
<li><a href="https://extra-resources.techidaily.com/how-to-make-reels-on-instagram/"><u>How to Make Reels on Instagram</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/in-2024-how-itel-a60-mirror-screen-to-pc-drfone-by-drfone-android/"><u>In 2024, How Itel A60 Mirror Screen to PC? | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/leap-into-advanced-chatgpt-top-9-essential-plugins-here/"><u>Leap Into Advanced ChatGPT – Top 9 Essential Plugins Here</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/leveraging-ai-for-compelling-youtube-thumbnails/"><u>Leveraging AI for Compelling YouTube Thumbnails</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/machine-talk-deciphering-the-gpt-bing-divide/"><u>Machine Talk: Deciphering the GPT-Bing Divide</u></a></li>
<li><a href="https://extra-skills.techidaily.com/mastering-time-stamps-on-youtube-videos-for-2024/"><u>Mastering Time Stamps on YouTube Videos for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/maximizing-chatgpts-potential-in-academia/"><u>Maximizing ChatGPT's Potential in Academia</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/maximizing-creativity-with-chatgpts-advanced-image-recognition/"><u>Maximizing Creativity with ChatGPT's Advanced Image Recognition</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/missed-malware-alert-say-no-to-google-bard-download/"><u>Missed Malware Alert: Say No to Google Bard Download</u></a></li>
<li><a href="https://animation-videos.techidaily.com/new-ways-on-how-to-get-started-in-stop-motion-claymation/"><u>New Ways on How to Get Started in Stop Motion Claymation</u></a></li>
<li><a href="https://graphic-issues.techidaily.com/removing-network-errors-in-multiplayer-civ-5/"><u>Removing Network Errors in Multiplayer CIV 5</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revolutionizing-communication-post-chatgpt-era/"><u>Revolutionizing Communication: Post-ChatGPT Era</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/sparkling-ai-chat-mastering-chatgpts-10-enhancements/"><u>Sparkling AI Chat: Mastering ChatGPT's 10 Enhancements</u></a></li>
<li><a href="https://facebook-video-recording.techidaily.com/strategies-to-successfully-broadcast-facespace-lives-on-tv-for-2024/"><u>Strategies to Successfully Broadcast Facespace Lives on TV for 2024</u></a></li>
<li><a href="https://audio-editing.techidaily.com/the-swift-method-for-rescaling-audio-playback-rates-for-2024/"><u>The Swift Method for Rescaling Audio Playback Rates for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-ultimate-7-extensions-for-supercharged-ai-conversations/"><u>The Ultimate 7 Extensions for Supercharged AI Conversations</u></a></li>
<li><a href="https://screen-mirror.techidaily.com/top-10-airplay-apps-in-realme-c55-for-streaming-drfone-by-drfone-android/"><u>Top 10 AirPlay Apps in Realme C55 for Streaming | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/understanding-and-correcting-6-typical-gpt-malfunctions/"><u>Understanding & Correcting 6 Typical GPT Malfunctions</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unlocking-the-potential-of-gpt-4-collectively/"><u>Unlocking the Potential of GPT-4 Collectively</u></a></li>
<li><a href="https://ai-video-editing.techidaily.com/1713964398363-updated-looking-for-the-simple-steps-to-add-a-filter-to-your-video-in-premiere-pro-here-are-the-complete-steps-along-with-the-list-of-free-premiere-filter-p/"><u>Updated Looking for the Simple Steps to Add a Filter to Your Video in Premiere Pro? Here Are the Complete Steps Along with the List of Free Premiere Filter Presets to Use for 2024</u></a></li>
</ul></div>
