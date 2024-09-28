---
title: Seamless Communication via ChatGPT's API
date: 2024-08-29T19:42:15.449Z
updated: 2024-08-30T19:42:15.449Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Seamless Communication via ChatGPT's API
excerpt: This Article Describes Seamless Communication via ChatGPT's API
thumbnail: https://thmb.techidaily.com/ef4f7364eb178269ce5e333115e1834d8d6af4b37108b148f724431123b9f7ea.jpg
---

## Seamless Communication via ChatGPT's API

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
![OpenAI API Key Page](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2024/02/openai-api-key-page.png)

 The code used in this project is available in a [GitHub repository](https://github.com/makeuseofcode/ChatGPT-API-Sample-Code) and is free for you to use under the MIT license.

<!-- affiliate ads begin -->
<a href="https://25home.pxf.io/c/5597632/2090698/16836" target="_top" id="2090698"><img src="//a.impactradius-go.com/display-ad/16836-2090698" border="0" alt="" width="720" height="300"/></a>
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
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4537547&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/4b0a0290ad7df100b77e86839989a75e/products/vcfpro.png" border="0">Video Converter Factory Pro</a>
<!-- affiliate ads end -->
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

![A poem on programmers](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/a-poem-on-programmers.jpg)

<!-- affiliate ads begin -->
<a href="https://shop.mondly.com/affiliate.php?ACCOUNT=ATISTUDI&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.mondly.com%3FAFFILIATE%3D108875%26RESOURCE%3D%2BBusiness%2B970x90%2B"><img src="https://secure.avangate.com/images/merchant/69c418c33ec2e1a4267fa9bb77fa1428/business-970x90.gif" border="0"></a>
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

<!-- affiliate ads begin -->
<span id="1793213">
					<video width="1080" height="1620" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1793213.jpeg"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/19135-1793213">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1793213.jpeg" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:1080px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Ftinyland.pxf.io%2Fc%2F5597632%2F1793213%2F19135'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1793213/19135" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## 3\. Making ChatGPT API Requests

 The OpenAI API's GPT-3.5 Turbo, GPT-4, and GPT-4 Turbo are the same models that ChatGPT uses. These powerful models are capable of understanding and generating natural language text and code. GPT-4 Turbo can even process image inputs which opens the gates for several uses including analyzing images, parsing documents with figures, and transcribing text from images.

 Please note that the ChatGPT API is a general term that refers to OpenAI APIs that use GPT-based models, including the **gpt-3.5-turbo**, **gpt-4**, and **gpt-4-turbo** models.

 The ChatGPT API is primarily optimized for chat but it also works well for text completion tasks. Whether you want to generate code, translate languages, or draft documents, this API can handle it all.

 To get access to the GPT-4 API, you need to make a successful payment of $1 or more. Otherwise, you might get an error similar to "The model \`gpt-4\` does not exist or you do not have access to it."

<!-- affiliate ads begin -->
<a href="https://shop.pcdj.com/order/checkout.php?PRODS=4698832&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/47f4b6321e9fd8e8f7326a6adc1a7c1e/products/karaoki-new-searchresultspane.jpg" border="0">PCDJ Karaoki is the complete professional karaoke software designed for KJs and karaoke venues. Karaoki includes an advanced automatic singer rotation list with singer history, key control, news ticker, next singers screen, a song book exporter and printer, a jukebox background music player and many other features designed so you can host karaoke shows faster and easier! 
 PCDJ Karaoki (WINDOWS ONLY Professional Karaoke Software - 3 Activations)</a>
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

![Temperature parameter of ChatGPT API](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/temperature-parameter-of-chatgpt-api-3.jpg)

<!-- affiliate ads begin -->
<a href="https://shop.incomedia.eu/order/checkout.php?PRODS=39655089&QTY=1&AFFILIATE=108875&CART=1"><img src="https://incomedia.eu/files/images/affiliates/wa/01_WA_728x90.jpg" border="0"></a>
<!-- affiliate ads end -->
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

![A poem on programmers](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/a-poem-on-programmers.jpg)

<!-- affiliate ads begin -->
<a href="https://checkout.devart.com/order/checkout.php?PRODS=5023555&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/45b430710ad04765a6afd58d9d9fafca/products/dotConnect_O.png" border="0">dotConnect for Oracle is an ADO.NET data provider for Oracle with Entity Framework Support.</a>
<!-- affiliate ads end -->
<!-- affiliate ads begin -->
<a href="https://shop.systoolsgroup.com/affiliate.php?ACCOUNT=SYSTOOBY&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.systoolsgroup.com%3FAFFILIATE%3D108875%26RESOURCE%3DSysTools%2BOST%2BRecovery"><img src="https://www.systoolsgroup.com/box/ost-recovery.png" border="0"></a>
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
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=3851655&QTY=1&AFFILIATE=108875&CART=1"><img src="http://www.aiseesoft.com/avangate/30p/banner.jpg" border="0"></a>
<!-- affiliate ads end -->
## Build Next Generation Apps Using the ChatGPT API

 The ChatGPT API has opened gates for developers around the world to build innovative products with the power of AI.

 You can use this tool to develop applications like story writers, code translators, marketing copy generators, and text summarizers. Your imagination is the limit to building applications using this technology.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 With the release of its API, OpenAI has opened up the capabilities of ChatGPT to everyone. You can now seamlessly integrate ChatGPT's features into your application.

 Follow these steps to get started, whether you're looking to integrate ChatGPT into your existing application or develop new applications with it.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=2201613&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.macdvdripperpro.com/images/devices-3.png" border="0"></a>
<!-- affiliate ads end -->
## 1\. Getting an OpenAI API Key

 To start using the ChatGPT API, you need to obtain an API key.

1. Sign up or log in to the official [OpenAI](https://platform.openai.com/signup) platform.
2. Once you're logged in, click on the **API keys** tab in the left pane.
3. Next, click on the **Create new secret key** button to generate the API key.
4. You won't be able to view the API key again, so copy it and store it somewhere safe.  
![OpenAI API Key Page](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2024/02/openai-api-key-page.png)

 The code used in this project is available in a [GitHub repository](https://github.com/makeuseofcode/ChatGPT-API-Sample-Code) and is free for you to use under the MIT license.

<!-- affiliate ads begin -->
<a href="https://estore.winxdvd.com/order/checkout.php?PRODS=12653853&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/bcb41ccdc4363c6848a1d760f26c28a0/products/14_videoproc-converter-ai-box.png" border="0"></a>
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

## 3\. Making ChatGPT API Requests

 The OpenAI API's GPT-3.5 Turbo, GPT-4, and GPT-4 Turbo are the same models that ChatGPT uses. These powerful models are capable of understanding and generating natural language text and code. GPT-4 Turbo can even process image inputs which opens the gates for several uses including analyzing images, parsing documents with figures, and transcribing text from images.

 Please note that the ChatGPT API is a general term that refers to OpenAI APIs that use GPT-based models, including the **gpt-3.5-turbo**, **gpt-4**, and **gpt-4-turbo** models.

 The ChatGPT API is primarily optimized for chat but it also works well for text completion tasks. Whether you want to generate code, translate languages, or draft documents, this API can handle it all.

 To get access to the GPT-4 API, you need to make a successful payment of $1 or more. Otherwise, you might get an error similar to "The model \`gpt-4\` does not exist or you do not have access to it."

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=37100474&QTY=1&AFFILIATE=108875&CART=1"><img src="https://awario.com/images/pages/index/img-platform-ui-1280@1x.avif" border="0"></a>
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

<!-- affiliate ads begin -->
<a href="https://otszone.ots7.com/order/checkout.php?PRODS=4713321&QTY=1&AFFILIATE=108875&CART=1"><img src="https://green.ots7.com/screenshots/OtsAV/OtsAVDJ1.90-300x188.jpg" border="0">OtsAV DJ Pro</a>
<!-- affiliate ads end -->
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

<!-- affiliate ads begin -->
<a href="https://shop.systoolsgroup.com/affiliate.php?ACCOUNT=SYSTOOBY&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.systoolsgroup.com%3FAFFILIATE%3D108875%26RESOURCE%3D%2BSysTools%2BPDF%2BUnlocker"><img src="https://www.systoolsgroup.com/box/pdf-unlocker.png" border="0"></a>
<!-- affiliate ads end -->
 You can further customize the **temperature** and **max\_tokens** parameters of the model to get the output according to your requirements.

 The higher the temperature, the higher the randomness of the output, and vice-versa. If you want your responses to be more focused and deterministic, go for the lower temperature value. And if you want it to be more creative, use a higher value. The temperature value ranges between 0 and 2\.

![Temperature parameter of ChatGPT API](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/temperature-parameter-of-chatgpt-api-3.jpg)

 Like ChatGPT, the API also has a word limit. Use the **max\_tokens** parameter to limit the length of responses. Be aware that setting a lower **max\_tokens** value can cause issues as it may cut off the output mid-way.

 At the time of writing, the **gpt-3.5-turbo** model has a token limit of 4,096, while **gpt-4**'s is 8,192\. The latest **gpt-3.5-turbo-0125** and **gpt-4-turbo-preview** models have limits of 16,385 and 128,000 respectively.

 After high demand from developers, OpenAI has introduced JSON mode which instructs the model to always return a JSON object. You can enable JSON mode by setting **response\_format** to **{ "type": "json\_object" }**. Currently, this feature is only available to the latest models: gpt-3.5-turbo-0125 and gpt-4-turbo-preview.

 You can further configure the model using the other parameters provided by [OpenAI](https://platform.openai.com/docs/api-reference/chat/create).

<!-- affiliate ads begin -->
<a href="https://shop.emeditor.com/order/checkout.php?PRODS=4631722&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.emeditor.com/wp-content/uploads/2023/05/frontpage2-2048x588.webp" border="0">EmEditor Professional (Lifetime License, non-store app)</a>
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

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=194977&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.blumentals.net/scrfactory/images/screensaver-software.png" border="0">Screensaver Factory, Create stunning professional screensavers within minutes. Create screensavers for yourself, for marketing or unlimited royalty-free commercial distribution. Make screensavers from images, video and swf flash, add background music and smooth sprite and transition effects. Screensaver Factory is very easy to use, and it enables you to make self-installing screensaver files and CDs for easy setup and distribution. Screensaver Factory is the most advanced software of its kind.</a>
<!-- affiliate ads end -->
<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4600113&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.epubor.com/images/drm-removal-feature2.png" border="0">Any DRM Removal for Win：Remove DRM from Adobe, Kindle, Sony eReader, Kobo, etc, read your ebooks anywhere.</a>
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
<a href="https://coinrule.sjv.io/c/5597632/1958379/18409" target="_top" id="1958379"><img src="//a.impactradius-go.com/display-ad/18409-1958379" border="0" alt="" width="856" height="508"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1958379/18409" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
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

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4699091&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/bccefcc1b1eee9eca3ae4f5c1a281482/products/1_jutoh-logo-1200x1600.jpg" border="0">Jutoh Plus -  Jutoh is an ebook creator for Epub, Kindle and more. It's fast, runs on Windows, Mac, and Linux, comes with a cover design editor, and allows book variations to be created with alternate text, style sheets and cover designs. Jutoh Plus adds scripting so you can automate ebook import and creation operations. It also allows customisation of ebook HTML via templates and source code documents; and you can create Windows CHM and wxWidgets HTB help files. </a>
<!-- affiliate ads end -->
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
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4712430&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/c404a5adbf90e09631678b13b05d9d7a/products/dlnow_256.png" border="0">DLNow Video Downloader</a>
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

![Temperature parameter of ChatGPT API](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/temperature-parameter-of-chatgpt-api-3.jpg)

 Like ChatGPT, the API also has a word limit. Use the **max\_tokens** parameter to limit the length of responses. Be aware that setting a lower **max\_tokens** value can cause issues as it may cut off the output mid-way.

 At the time of writing, the **gpt-3.5-turbo** model has a token limit of 4,096, while **gpt-4**'s is 8,192\. The latest **gpt-3.5-turbo-0125** and **gpt-4-turbo-preview** models have limits of 16,385 and 128,000 respectively.

 After high demand from developers, OpenAI has introduced JSON mode which instructs the model to always return a JSON object. You can enable JSON mode by setting **response\_format** to **{ "type": "json\_object" }**. Currently, this feature is only available to the latest models: gpt-3.5-turbo-0125 and gpt-4-turbo-preview.

 You can further configure the model using the other parameters provided by [OpenAI](https://platform.openai.com/docs/api-reference/chat/create).

<!-- affiliate ads begin -->
<a href="https://imp.i110150.net/c/5597632/924299/11305" target="_top" id="924299"><img src="//a.impactradius-go.com/display-ad/11305-924299" border="0" alt="" width="520" height="100"/></a>
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

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2075471/7443" target="_top" id="2075471"><img src="//a.impactradius-go.com/display-ad/7443-2075471" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2075471/7443" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=37701530&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/6fe0c81e3f9438db11ebbfba6c5ce460/products/copy_cbLogo_with_text_blue.png" border="0">CalendarBudget - Monthly subscription membership to CalendarBudget via web browser or mobile app. Support included. </a>
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


