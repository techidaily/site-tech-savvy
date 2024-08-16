---
title: "Mastering Conversational Support: Merging GPT with WhatsApp"
date: 2024-08-15T02:40:30.422Z
updated: 2024-08-16T02:40:30.422Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Mastering Conversational Support: Merging GPT with WhatsApp"
excerpt: "This Article Describes Mastering Conversational Support: Merging GPT with WhatsApp"
thumbnail: https://thmb.techidaily.com/1d7a3c5b577ddb7940a6a2457c0bee5c40f1807e21452ed2f6065cb51e5a9f16.jpg
---

## Mastering Conversational Support: Merging GPT with WhatsApp

 Today’s businesses embrace messaging apps like WhatsApp to communicate with customers. This results in a surge in the automation of business customer interactions using chatbots.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 Such a chatbot is ChatGPT, a large language model by OpenAI that you can integrate with WhatsApp to automate customer interactions by providing fast and accurate responses to customer queries.

## Understanding and Accessing the ChatGPT API

 Before integrating with WhatsApp, it is essential to get a [basic understanding of ChatGPT and ChatGPT API](https://www.makeuseof.com/chatgpt-api-complete-guide/). ChatGPT is a [generative large language model](https://www.makeuseof.com/what-is-generative-ai/) that receives text-based queries and returns human-like responses. OpenAI provides a simple API interface for developers to access and use ChatGPT’s GPT-3.5 and GPT-4 models.

 To access ChatGPT API keys, you need to navigate to the [OpenAI API](https://platform.openai.com/) platform. After signing in, click on the profile icon. Then, click on the **View API keys** option.

![OpenAI API homepage](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/integrating-whatsapp-and-chatgpt-api-homepage.jpg)

 Next, click the **Create new secret key** button to create a new API key.

![OpenAI API keys creation](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/integrating-whatsapp-and-chatgpt-api-key.jpg)

 Enter the requested details, i.e., the **name** of the key.

![OpenAI API key naming](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/integrating-whatsapp-and-chatgpt-api-key-name.jpeg)

 A secret key will prompt.

![OpenAI API key generated](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/integrating-whatsapp-and-chatgpt-api-key-prompt.jpeg)

 Copy and store the key in a secure place for future use.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4620780&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/07dd4d5a72f5740ef0f035f201951476/728__90banner.jpg" border="0"></a>
<!-- affiliate ads end -->
## Setting Up a WhatsApp Business Account

 To integrate ChatGPT with WhatsApp, you must set up a WhatsApp Business account. Note that [WhatsApp Business is different from regular WhatsApp](https://www.makeuseof.com/whatsapp-vs-whatsapp-business/). This account will allow you to access the [WhatsApp Business API](https://business.whatsapp.com/developers/developer-hub), which you will integrate with the ChatGPT API.

 The full source code is available in a [GitHub repository](https://github.com/makeuseofcode/WhatsApp-ChatGPT-integration).

 You can use a third-party service like Kommunicate, a WhatsApp chatbot, or a Python script to integrate ChatGPT with WhatsApp. This tutorial’s focus will be on integrating ChatGPT using a Python script. It will then give you an overview of integration using a WhatsApp chatbot.

<!-- affiliate ads begin -->
<a href="https://ukaidot.sjv.io/c/5597632/1793237/19578" target="_top" id="1793237"><img src="//a.impactradius-go.com/display-ad/19578-1793237" border="0" alt="" width="1200" height="1200"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1793237/19578" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Using Python Script to Integrate WhatsApp With ChatGPT API

 Before you start the development, create a virtual environment for your application using **Pipenv** as follows:

`pipenv install django djangorestframework openai  
`

 This command will install the **django**, **djangorestframework**, and **openai** packages.

 Then, create a new Django project.

`django-admin startproject whatsapp  
`

 Navigate to the created **whatsapp** directory and create a Django app named **gpt**:

`py manage.py startapp gpt  
`

 In the **whatsapp/settings.py** file, add the new app, **gpt** on the installed apps list as follows:

`INSTALLED_APPS = [  
   'django.contrib.admin',  
   'django.contrib.auth',  
   'django.contrib.contenttypes',  
   'django.contrib.sessions',  
   'django.contrib.messages',  
   'django.contrib.staticfiles',  
   'rest_framework',  
   'gpt',
]`

 In your **whatsapp/urls.py** file, add the **gpt** app URL. This will redirect to the URLs you will create on the **gpt** app:

`from django.contrib import admin  
from django.urls import path, include  
  
urlpatterns = [  
   ...  
   path('api/', include('gpt.urls')), # gpt app URL  
]`

 On the **gpt/views.py** file, add the following block of code to create ChatGPT API view:

`from rest_framework.response import Response  
import openai  
from rest_framework.views import APIView  
  
class OpenAIGPTView(APIView):  
  
   def get(self, request):  
       input = request.GET.get('q')  
       openai.api_key = "ENTER_OPENAI_API_KEY"  
       completion = openai.ChatCompletion.create(  
       model="gpt-3.5-turbo",
       messages=[{"role": "user", "content": input}]  
       )  
       answer = completion ['choices'][0]['message']['content']  
       return Response(answer)`

 The view [sets up an API endpoint](https://www.makeuseof.com/how-apis-work-and-how-to-use-them/) that expects a GET request with a query parameter **q** comprising the user input. It then uses OpenAI’s **gpt-3.5-turbo** model to generate a response based on the provided input and returns the response as the API’s output.

 Next, create a **urls.py** file and register the API view by adding the following lines of code:

`from django.urls import path  
from .views import *  
  
urlpatterns = [  
   path('chat', OpenAIGPTView.as_view()),  
]`

 Run the **migrate** and **runserver** commands as follows:

`python manage.py migrate  
python manage.py runserver`

 Test the **/api/chat** endpoint by sending a GET request to **<http://localhost:8000/api/chat?q=Hello>**.

 Expected output:

![API endpoint test](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/integrating-whatsapp-and-chatgpt-api-endpoint.jpeg)
<!-- affiliate ads begin -->
<a href="https://ursime.pxf.io/c/5597632/2048963/16384" target="_top" id="2048963"><img src="//a.impactradius-go.com/display-ad/16384-2048963" border="0" alt="" width="1200" height="900"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2048963/16384" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Next, install [Go](https://go.dev/doc/install) if it is not already installed on your machine.

 Clone the **Whatsmeow** client using the command below:

`git clone https://github.com/Huskynarr/whatsapp-gpt.git  
`

 Navigate to the repository, **whatsapp-gpt**, and on the file, **main.go** update this line:

`url := "http://localhost:5001/chat?q=" + urlEncoded  
`

 to:

`url := "http://127.0.0.1:8000/api/chat?q=" + urlEncode  
`

 Save the changes and run the file:

`go run main.go`

 The application will prompt you with a QR code to log in to your WhatsApp account.

 Expected output:

![Application QR code prompt](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/integrating-whatsapp-and-chatgpt-api-key-qr-code.jpeg)
<!-- affiliate ads begin -->
<a href="https://turtlebeacheu.sjv.io/c/5597632/1996818/23722" target="_top" id="1996818"><img src="//a.impactradius-go.com/display-ad/23722-1996818" border="0" alt="" width="600" height="600"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1996818/23722" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Move to your WhatsApp mobile app and navigate to **Settings > QR code > Scan code** to add a new linked device and scan the popped QR code on your terminal.

 After logging in, the application will start listening to incoming messages. If someone sends a message, the received message will make a GET request to API with the message as a query parameter and send the response back to the sender on WhatsApp.

 Expected output:

![Output of integrating chatgpt and WhatsApp](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/integrating-whatsapp-and-chatgpt-api-output.jpg)

## Using WhatsApp Chatbot to Integrate WhatsApp With ChatGPT API

 Another way to integrate ChatGPT into WhatsApp messages is by using a WhatsApp chatbot.

 Once you register your WhatsApp Business API, use a chat builder like OpenDialog to create a flow for the chat. You will then test your chatbot and add it to your mobile phone.

<!-- affiliate ads begin -->
<a href="https://shop.copernic.com/order/checkout.php?PRODS=41033095&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.2checkout.com/images/merchant/8d30aa96e72440759f74bd2306c1fa3d/Copernic-2023-Affiliate-728x90-Advanced-3YR.png" border="0"></a>
<!-- affiliate ads end -->
### Integrate OpenAI API With Your WhatsApp Chatbot

 To integrate your WhatsApp chatbot with OpenAI models, use the API key from OpenAI.

 Integrating WhatsApp chatbots with OpenAI GPT models presents a risk of WhatsApp blocking your account on security claims.

 Though this method is easier if you already have a chatbot, you should only opt for it once you’re comfortable with the risks involved.

<!-- affiliate ads begin -->
<a href="https://shop.emeditor.com/order/checkout.php?PRODS=4631722&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.emeditor.com/wp-content/uploads/2023/05/frontpage2-2048x588.webp" border="0">EmEditor Professional (Lifetime License, non-store app)</a>
<!-- affiliate ads end -->
### Configuring Automated Responses

 To get better customer service, configure automated responses to provide fast and accurate responses to customer messages. These responses will personalize the customer by name and provide relevant responses to customer queries.

### Testing Your WhatsApp Chatbot

 Like all AI API systems, testing is key before you deploy your WhatsApp chatbot. This is to ensure that it works as expected. API testing tools like Postman and Curl can help to test your chatbot’s responses.

 In this case, the Django REST framework provides a browsable API to help test API requests and responses.

### Measuring Success and Fine-Tuning

 Once your WhatsApp chatbot is in deployment, it is crucial to measure its success and usage over time. This will help with fine-tuning it accordingly. Analytics tools like OpenDialog and Rasa can help to track metrics such as response time, retention rate, and customer satisfaction.

## Streamline Customer Support on WhatsApp With ChatGPT Integration

 OpenAI’s GPT-3.5 or GPT-4 models can handle large volumes of inquiries, provide instant responses, and use advanced language processing, making it a better solution for customer service interactions. By integrating ChatGPT with WhatsApp, you can save time, improve customer satisfaction, and streamline communication. Several other large language models could also improve your chatbot’s performance.

**SCROLL TO CONTINUE WITH CONTENT**

 Such a chatbot is ChatGPT, a large language model by OpenAI that you can integrate with WhatsApp to automate customer interactions by providing fast and accurate responses to customer queries.

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
<li><a href="https://some-techniques.techidaily.com/updated-font-fusion-merging-style-and-content-in-after-effects/"><u>[Updated] Font Fusion  Merging Style & Content in After Effects</u></a></li>
<li><a href="https://some-techniques.techidaily.com/updated-how-to-add-filters-and-music-on-windows-11-photos-app/"><u>[Updated] How to Add Filters and Music on Windows 11 Photos App</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/2024-approved-revamped-interview-inquiries-to-spark-podcast-fans-curiosity/"><u>2024 Approved  Revamped Interview Inquiries to Spark Podcast Fans' Curiosity</u></a></li>
<li><a href="https://digital-screen-recording.techidaily.com/2024-approved-seamlessly-saving-your-screen-premium-choices-on-pc-and-mac/"><u>2024 Approved  Seamlessly Saving Your Screen  Premium Choices on PC & Mac</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-powered-productivity-6-essential-chatgpt-tools-for-remote-jobs/"><u>AI-Powered Productivity: 6 Essential ChatGPT Tools for Remote Jobs</u></a></li>
<li><a href="https://buynow-info.techidaily.com/akaso-ek7000-ultimate-4k-action-cam-at-affordable-prices/"><u>AKASO EK7000 Ultimate 4K Action Cam at Affordable Prices</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/artificinas-and-labor-the-converging-pathways/"><u>Artificinas and Labor: The Converging Pathways</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/beyond-boundaries-next-gen-ai-discussions/"><u>Beyond Boundaries: Next Gen AI Discussions</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/building-bots-with-gpt-3-and-python/"><u>Building Bots with GPT-3 & Python</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-and-numbers-navigating-data-with-ai-expertise/"><u>ChatGPT & Numbers: Navigating Data with AI Expertise</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpts-comedic-crafting-are-we-witness-to-witty-works/"><u>ChatGPT's Comedic Crafting: Are We Witness to Witty Works?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/dialogue-revolution-giving-chatgpt-a-human-touch/"><u>Dialogue Revolution: Giving ChatGPT a Human Touch</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/elevating-work-routines-with-gpt-3-strategies/"><u>Elevating Work Routines with GPT-3 Strategies</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/epiphany-talking-to-chatgpt-made-simple/"><u>Epiphany: Talking to ChatGPT Made Simple</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/exploiting-chatgpts-link-to-wolframalpha-in-3-ways/"><u>Exploiting ChatGPT's Link to WolframAlpha in 3 Ways</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/explosive-popularity-unveiling-5-powerful-motivators-for-chatgpt/"><u>Explosive Popularity: Unveiling 5 Powerful Motivators for ChatGPT</u></a></li>
<li><a href="https://extra-information.techidaily.com/flip-to-fun-immediate-collage-making-tricks/"><u>Flip to Fun  Immediate Collage Making Tricks</u></a></li>
<li><a href="https://techidaily.com/how-to-reset-vivo-t2x-5g-without-losing-data-drfone-by-drfone-reset-android-reset-android/"><u>How to Reset Vivo T2x 5G without Losing Data | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/innovative-integrations-leveraging-chatgpts-api-power/"><u>Innovative Integrations: Leveraging ChatGPT's API Power</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/inside-claude-2-operations-and-applications/"><u>Inside Claude 2: Operations and Applications</u></a></li>
<li><a href="https://win11.techidaily.com/mastering-window-customization-for-a-macos-feel-in-windows/"><u>Mastering Window Customization for a macOS Feel in Windows</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/power-up-your-design-process-large-scale-techniques-in-canva-plus-gpt/"><u>Power Up Your Design Process: Large Scale Techniques in Canva + GPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/sifting-through-virtual-realities-identifying-inauthentic-ai-responses/"><u>Sifting Through Virtual Realities: Identifying Inauthentic AI Responses</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/silent-content-slips-ai-detectors-at-risk/"><u>Silent Content Slips: AI Detectors at Risk</u></a></li>
<li><a href="https://fix-guide.techidaily.com/simple-solutions-to-fix-android-systemui-has-stopped-error-for-asus-rog-phone-8-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>Simple Solutions to Fix Android SystemUI Has Stopped Error For Asus ROG Phone 8 | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/sleuth-through-cyberspace-discover-4-immersive-ai-game-challenges/"><u>Sleuth Through Cyberspace: Discover 4 Immersive AI Game Challenges</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/smartphone-deals-and-digital-safety-unveiled/"><u>Smartphone Deals & Digital Safety Unveiled</u></a></li>
<li><a href="https://mondly-stories.techidaily.com/spanish-for-the-curious-childs-mind/"><u>Spanish for the Curious Child's Mind</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/steering-ai-ethics-why-openais-ceo-calls-for-oversight/"><u>Steering AI Ethics: Why OpenAI's CEO Calls for Oversight</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/suddenly-no-more-chatgpt-in-italy-the-banned-reason/"><u>Suddenly No More ChatGPT in Italy: The Banned Reason</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/transform-your-job-applications-write-cover-letters-via-chatai/"><u>Transform Your Job Applications: Write Cover Letters via ChatAI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unraveling-the-dangers-of-fraudgpt-cybersecurity-protocols/"><u>Unraveling the Dangers of FraudGPT: Cybersecurity Protocols</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveil-converse-with-chatgpt-instantly/"><u>Unveil: Converse With ChatGPT Instantly</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/why-websites-ban-gptbot-navigating-ai-and-copyright-laws/"><u>Why Websites Ban GPTBot - Navigating AI and Copyright Laws</u></a></li>
</ul></div>
