---
title: "Spearheading Development: Mastery in Using the ChatGPT API"
date: 2024-08-03T00:52:35.840Z
updated: 2024-08-04T00:52:35.840Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Spearheading Development: Mastery in Using the ChatGPT API"
excerpt: "This Article Describes Spearheading Development: Mastery in Using the ChatGPT API"
thumbnail: https://thmb.techidaily.com/f6e6b4d9497e69403999596a39a3f38ca99f274b0d3eeb6c66835e6a03fad9ac.jpg
---

## Spearheading Development: Mastery in Using the ChatGPT API

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
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=3922934&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/4b0a0290ad7df100b77e86839989a75e/products/ripperpro.png" border="0">WonderFox DVD Ripper Pro</a>
<!-- affiliate ads end -->
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
<a href="https://store.iobit.com/order/checkout.php?PRODS=4596923&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/184260348236f9554fe9375772ff966e/ascscan_468X60.png" border="0"></a>
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

<!-- affiliate ads begin -->
<a href="https://shop.copernic.com/order/checkout.php?PRODS=41033101&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.2checkout.com/images/merchant/8d30aa96e72440759f74bd2306c1fa3d/Copernic-2023-Affiliate-728x90-Elite.png" border="0"></a>
<!-- affiliate ads end -->
![ChatGPT API Roles Diagram](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/wm/2024/02/chatgpt-api-roles-diagram-1-1.jpg)

 You can further customize the **temperature** and **max\_tokens** parameters of the model to get the output according to your requirements.

 The higher the temperature, the higher the randomness of the output, and vice-versa. If you want your responses to be more focused and deterministic, go for the lower temperature value. And if you want it to be more creative, use a higher value. The temperature value ranges between 0 and 2\.

<!-- affiliate ads begin -->
<a href="https://united.elfm.net/c/5597632/748964/4704" target="_top" id="748964"><img src="//a.impactradius-go.com/display-ad/4704-748964" border="0" alt="" width="300" height="250"/></a><img height="0" width="0" src="https://united.elfm.net/i/5597632/748964/4704" style="position:absolute;visibility:hidden;" border="0" />
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
<!-- affiliate ads begin -->
<a href="https://modlily.sjv.io/c/5597632/2072819/17059" target="_top" id="2072819"><img src="//a.impactradius-go.com/display-ad/17059-2072819" border="0" alt="" width="300" height="250"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2072819/17059" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![OpenAI API Key Page](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2024/02/openai-api-key-page.png)

 The code used in this project is available in a [GitHub repository](https://github.com/makeuseofcode/ChatGPT-API-Sample-Code) and is free for you to use under the MIT license.

<!-- affiliate ads begin -->
<a href="https://godlikehost.sjv.io/c/5597632/1920054/21774" target="_top" id="1920054"><img src="//a.impactradius-go.com/display-ad/21774-1920054" border="0" alt="" width="320" height="100"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1920054/21774" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://boody-eco-wear.pxf.io/c/5597632/1567905/13846" target="_top" id="1567905"><img src="//a.impactradius-go.com/display-ad/13846-1567905" border="0" alt="" width="300" height="250"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1567905/13846" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://shop.mondly.com/affiliate.php?ACCOUNT=ATISTUDI&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.mondly.com%3FAFFILIATE%3D108875%26RESOURCE%3D%2BEducational%2B300x600%2B"><img src="https://secure.avangate.com/images/merchant/69c418c33ec2e1a4267fa9bb77fa1428/educational-300x600.gif" border="0"></a>
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
<a href="https://shop.emeditor.com/order/checkout.php?PRODS=4610657&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.emeditor.com/wp-content/uploads/2024/06/emeditor_chat_ai.png" border="0">
EmEditor is a fast, lightweight, yet extensible, easy-to-use text editor, code editor, CSV editor, and large file viewer for Windows. Both native 64-bit and 32-bit builds are available, and moreover, the 64-bit includes separate builds for SSE2 (128-bit), AVX-2 (256-bit), and AVX-512 (512-bit) instruction sets. New versions support AI-assisted writing.</a>
<!-- affiliate ads end -->
## 1\. Getting an OpenAI API Key

 To start using the ChatGPT API, you need to obtain an API key.

1. Sign up or log in to the official [OpenAI](https://platform.openai.com/signup) platform.
2. Once you're logged in, click on the **API keys** tab in the left pane.
3. Next, click on the **Create new secret key** button to generate the API key.
4. You won't be able to view the API key again, so copy it and store it somewhere safe.  
<!-- affiliate ads begin -->
<a href="https://ursime.pxf.io/c/5597632/2048963/16384" target="_top" id="2048963"><img src="//a.impactradius-go.com/display-ad/16384-2048963" border="0" alt="" width="1200" height="900"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2048963/16384" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![OpenAI API Key Page](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2024/02/openai-api-key-page.png)

 The code used in this project is available in a [GitHub repository](https://github.com/makeuseofcode/ChatGPT-API-Sample-Code) and is free for you to use under the MIT license.

<!-- affiliate ads begin -->
<a href="https://natural-cycles.sjv.io/c/5597632/2072200/17885" target="_top" id="2072200"><img src="//a.impactradius-go.com/display-ad/17885-2072200" border="0" alt="" width="728" height="90"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2072200/17885" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://parisrhonecom.sjv.io/c/5597632/1896607/21553" target="_top" id="1896607"><img src="//a.impactradius-go.com/display-ad/21553-1896607" border="0" alt="" width="750" height="422"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1896607/21553" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://shop.manycam.com/order/checkout.php?PRODS=17729331&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/8230bea7d54bcdf99cdfe85cb07313d5/mcaffbanner600x500.png" border="0"></a>
<!-- affiliate ads end -->
![Programming joke output generated via Chat Completions API](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2024/02/programming-joke-output-generated-via-chat-completions-api.jpg)

 The code demonstrates a ChatGPT API call using Python. Note that the model understood the context ("dad joke") and the type of response (Q&A form) that we were expecting, based on the prompts fed to it.

 The most significant part of the configuration is the **messages** parameter which accepts an array of message objects. Each message object contains a **role** and **content**. You can use three types of roles:

* **system** which sets up the context and behavior of the assistant.
* **user** which gives instructions to the assistant. The end user will typically provide this, but you can also provide some default user prompts in advance.
* **assistant** which can include example responses.

<!-- affiliate ads begin -->
<a href="https://zonlipartnershipprogram.pxf.io/c/5597632/1611407/17882" target="_top" id="1611407"><img src="//a.impactradius-go.com/display-ad/17882-1611407" border="0" alt="" width="300" height="485"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1611407/17882" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
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
<a href="https://turtlebeachus.sjv.io/c/5597632/1988416/23719" target="_top" id="1988416"><img src="//a.impactradius-go.com/display-ad/23719-1988416" border="0" alt="" width="600" height="600"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1988416/23719" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## 3\. Making ChatGPT API Requests

 The OpenAI API's GPT-3.5 Turbo, GPT-4, and GPT-4 Turbo are the same models that ChatGPT uses. These powerful models are capable of understanding and generating natural language text and code. GPT-4 Turbo can even process image inputs which opens the gates for several uses including analyzing images, parsing documents with figures, and transcribing text from images.

 Please note that the ChatGPT API is a general term that refers to OpenAI APIs that use GPT-based models, including the **gpt-3.5-turbo**, **gpt-4**, and **gpt-4-turbo** models.

 The ChatGPT API is primarily optimized for chat but it also works well for text completion tasks. Whether you want to generate code, translate languages, or draft documents, this API can handle it all.

 To get access to the GPT-4 API, you need to make a successful payment of $1 or more. Otherwise, you might get an error similar to "The model \`gpt-4\` does not exist or you do not have access to it."

<!-- affiliate ads begin -->
<a href="https://unicoeye.pxf.io/c/5597632/2084396/18498" target="_top" id="2084396"><img src="//a.impactradius-go.com/display-ad/18498-2084396" border="0" alt="" width="1920" height="700"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2084396/18498" style="position:absolute;visibility:hidden;" border="0" />
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

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4530091&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.pearlmountainsoft.com/n_img/product/cit_win/banScrn.jpg" border="0">CollageIt Pro</a>
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
<a href="https://checkout.mirillis.com/order/checkout.php?PRODS=4704640&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/547a5a56d43f6d40f9a6a2f76501d013/products/1_mirillis_action_boxshot_store_1x.jpg" border="0">
	Home Use license is dedicated for personal, non-commercial use only. 
	If Action! is used for commercial gain or to further any commercial purpose, 
	a Commercial Use license is required. Multi-license (volume discount) is intended for single 
 
	company, user or members of the same household. Action! - screen and game recorder</a>
<!-- affiliate ads end -->
![ChatGPT API Roles Diagram](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/wm/2024/02/chatgpt-api-roles-diagram-1-1.jpg)

 You can further customize the **temperature** and **max\_tokens** parameters of the model to get the output according to your requirements.

 The higher the temperature, the higher the randomness of the output, and vice-versa. If you want your responses to be more focused and deterministic, go for the lower temperature value. And if you want it to be more creative, use a higher value. The temperature value ranges between 0 and 2\.

<!-- affiliate ads begin -->
<a href="https://versadesk.pxf.io/c/5597632/1892107/21290" target="_top" id="1892107"><img src="//a.impactradius-go.com/display-ad/21290-1892107" border="0" alt="" width="1200" height="628"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1892107/21290" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
![Temperature parameter of ChatGPT API](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/temperature-parameter-of-chatgpt-api-3.jpg)

 Like ChatGPT, the API also has a word limit. Use the **max\_tokens** parameter to limit the length of responses. Be aware that setting a lower **max\_tokens** value can cause issues as it may cut off the output mid-way.

 At the time of writing, the **gpt-3.5-turbo** model has a token limit of 4,096, while **gpt-4**'s is 8,192\. The latest **gpt-3.5-turbo-0125** and **gpt-4-turbo-preview** models have limits of 16,385 and 128,000 respectively.

 After high demand from developers, OpenAI has introduced JSON mode which instructs the model to always return a JSON object. You can enable JSON mode by setting **response\_format** to **{ "type": "json\_object" }**. Currently, this feature is only available to the latest models: gpt-3.5-turbo-0125 and gpt-4-turbo-preview.

 You can further configure the model using the other parameters provided by [OpenAI](https://platform.openai.com/docs/api-reference/chat/create).

<!-- affiliate ads begin -->
<a href="https://electronicx.pxf.io/c/5597632/1872456/14483" target="_top" id="1872456"><img src="//a.impactradius-go.com/display-ad/14483-1872456" border="0" alt="" width="500" height="375"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1872456/14483" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://shop.mondly.com/affiliate.php?ACCOUNT=ATISTUDI&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.mondly.com%3FAFFILIATE%3D108875%26RESOURCE%3D%2BEducational%2B970x90%2B"><img src="https://secure.avangate.com/images/merchant/69c418c33ec2e1a4267fa9bb77fa1428/educational-970x90.gif" border="0"></a>
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
<a href="https://lightailing.sjv.io/c/5597632/1725213/17190" target="_top" id="1725213"><img src="//a.impactradius-go.com/display-ad/17190-1725213" border="0" alt="" width="1000" height="1000"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1725213/17190" style="position:absolute;visibility:hidden;" border="0" />
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




