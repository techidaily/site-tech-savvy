---
title: The Path to Proficiency in ChatGPT's API Utilization
date: 2024-10-31T16:51:29.512Z
updated: 2024-11-01T17:40:54.116Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes The Path to Proficiency in ChatGPT's API Utilization
excerpt: This Article Describes The Path to Proficiency in ChatGPT's API Utilization
thumbnail: https://thmb.techidaily.com/400ab6b2d84e9fcc703013e683c9e38470acb071407495f0911dc7de431c6c41.jpg
---

## The Path to Proficiency in ChatGPT's API Utilization

>  Disclaimer: This post includes affiliate links
>
>  If you click on a link and make a purchase, I may receive a commission at no extra cost to you.
>

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
<a href="https://bluettius.sjv.io/c/5597632/2148619/17108" target="_top" id="2148619">
  <img src="//a.impactradius-go.com/display-ad/17108-2148619" border="0" alt="https://techidaily.com" width="100" height="90"/>
</a>
<img height="0" width="0" src="https://bluettius.sjv.io/i/5597632/2148619/17108" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://aligracehair.sjv.io/c/5597632/2087253/19272" target="_top" id="2087253">
  <img src="//a.impactradius-go.com/display-ad/19272-2087253" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2087253/19272" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://ephamedtechinc.pxf.io/c/5597632/2137214/26400" target="_top" id="2137214">
  <img src="//a.impactradius-go.com/display-ad/26400-2137214" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://ephamedtechinc.pxf.io/i/5597632/2137214/26400" style="position:absolute;visibility:hidden;" border="0" />
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

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2087409/7443" target="_top" id="2087409">
  <img src="//a.impactradius-go.com/display-ad/7443-2087409" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2087409/7443" style="position:absolute;visibility:hidden;" border="0" />
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

<!-- affiliate ads begin -->
<a href="https://unicoeye.pxf.io/c/5597632/2134243/18498" target="_top" id="2134243">
  <img src="//a.impactradius-go.com/display-ad/18498-2134243" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://unicoeye.pxf.io/i/5597632/2134243/18498" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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
<a href="https://aligracehair.sjv.io/c/5597632/2135355/19272" target="_top" id="2135355">
  <img src="//a.impactradius-go.com/display-ad/19272-2135355" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135355/19272" style="position:absolute;visibility:hidden;" border="0" />
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

![ChatGPT API output response format](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2024/02/chatgpt-api-output-response-format.jpg)

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2135418/19272" target="_top" id="2135418">
  <img src="//a.impactradius-go.com/display-ad/19272-2135418" border="0" alt="https://techidaily.com" width="468" height="60"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135418/19272" style="position:absolute;visibility:hidden;" border="0" />
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

 You can further customize the **temperature** and **max\_tokens** parameters of the model to get the output according to your requirements.

 The higher the temperature, the higher the randomness of the output, and vice-versa. If you want your responses to be more focused and deterministic, go for the lower temperature value. And if you want it to be more creative, use a higher value. The temperature value ranges between 0 and 2\.

![Temperature parameter of ChatGPT API](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/04/temperature-parameter-of-chatgpt-api-3.jpg)

 Like ChatGPT, the API also has a word limit. Use the **max\_tokens** parameter to limit the length of responses. Be aware that setting a lower **max\_tokens** value can cause issues as it may cut off the output mid-way.

 At the time of writing, the **gpt-3.5-turbo** model has a token limit of 4,096, while **gpt-4**'s is 8,192\. The latest **gpt-3.5-turbo-0125** and **gpt-4-turbo-preview** models have limits of 16,385 and 128,000 respectively.

 After high demand from developers, OpenAI has introduced JSON mode which instructs the model to always return a JSON object. You can enable JSON mode by setting **response\_format** to **{ "type": "json\_object" }**. Currently, this feature is only available to the latest models: gpt-3.5-turbo-0125 and gpt-4-turbo-preview.

 You can further configure the model using the other parameters provided by [OpenAI](https://platform.openai.com/docs/api-reference/chat/create).

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2100537/7443" target="_top" id="2100537">
  <img src="//a.impactradius-go.com/display-ad/7443-2100537" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2100537/7443" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://instagram-videos.techidaily.com/new-2024-approved-simplify-media-handling-with-top-18-free-converters-for-windowsmacos-users/"><u>[New] 2024 Approved Simplify Media Handling With Top 18 Free Converters For Windows/macOS Users</u></a></li>
<li><a href="https://extra-tips.techidaily.com/new-breaking-down-youtube-promotion-costs/"><u>[New] Breaking Down Youtube Promotion Costs</u></a></li>
<li><a href="https://digital-screen-recording.techidaily.com/new-in-2024-snapshot-survival-guide-top-recorders-evaluated/"><u>[New] In 2024, SnapShot Survival Guide Top Recorders Evaluated</u></a></li>
<li><a href="https://youtube-web.techidaily.com/n-2024-the-counterplay-creative-ways-to-watch-youtube-in-reverse/"><u>[New] In 2024, The Counterplay Creative Ways to Watch YouTube in Reverse</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-for-devices-the-ultimate-guide-to-use/"><u>ChatGPT for Devices: The Ultimate Guide to Use</u></a></li>
<li><a href="https://fox-links.techidaily.com/gaming-meets-high-fidelity-review-of-logitech-g533/"><u>Gaming Meets High Fidelity: Review of Logitech G533</u></a></li>
<li><a href="https://blog-min.techidaily.com/how-to-transfer-apps-from-realme-v30-to-another-drfone-by-drfone-transfer-from-android-transfer-from-android/"><u>How to Transfer Apps from Realme V30 to Another | Dr.fone</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/in-2024-enhance-visibility-editing-igtv-video-texts/"><u>In 2024, Enhance Visibility Editing IGTV Video Texts</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/incorporating-chatgpt-to-boost-therapy-effectiveness/"><u>Incorporating ChatGPT to Boost Therapy Effectiveness</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/navigate-excel-complexity-using-3-strategic-chatgpt-techniques/"><u>Navigate Excel Complexity Using 3 Strategic ChatGPT Techniques</u></a></li>
<li><a href="https://techidaily.com/recover-apple-iphone-12-mini-data-from-ios-itunes-drfone-by-drfone-ios-data-recovery-ios-data-recovery/"><u>Recover Apple iPhone 12 mini Data From iOS iTunes | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/siri-to-gain-smart-enhancements-via-apple-innovation-expect-big-changes-in-the-2025-roadmap-insights/"><u>Siri to Gain Smart Enhancements via Apple Innovation; Expect Big Changes in the 2025 Roadmap – Insights</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-apple-watch-ultra-2-how-its-features-make-it-a-top-choice-for-me-now-at-100-off-expert-review/"><u>The Apple Watch Ultra 2: How Its Features Make It a Top Choice for Me, Now at $100 Off - Expert Review</u></a></li>
<li><a href="https://fox-access.techidaily.com/ultimate-choices-top-laptops-pro-video-editing-in-4k/"><u>Ultimate Choices Top Laptops Pro Video Editing in 4K</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unauthorized-advantages-of-ai-conversational-tools/"><u>Unauthorized Advantages of AI Conversational Tools</u></a></li>
</ul></div>

