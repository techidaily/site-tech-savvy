---
title: "Transforming Replies with AI: Merging GPT-3 and WhatsApp Help"
date: 2025-01-08T17:26:21.312Z
updated: 2025-01-12T18:19:42.669Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Transforming Replies with AI: Merging GPT-3 and WhatsApp Help"
excerpt: "This Article Describes Transforming Replies with AI: Merging GPT-3 and WhatsApp Help"
thumbnail: https://thmb.techidaily.com/7e53aeacfe9180f7bf103bd851c0952fea27590b967ba6821cf8991af471fa5a.jpg
---

## Transforming Replies with AI: Merging GPT-3 and WhatsApp Help

 Today’s businesses embrace messaging apps like WhatsApp to communicate with customers. This results in a surge in the automation of business customer interactions using chatbots.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 Such a chatbot is ChatGPT, a large language model by OpenAI that you can integrate with WhatsApp to automate customer interactions by providing fast and accurate responses to customer queries.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/q4-YQ9Wjtfg?si=6afn1fydg_Wb9B8z" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/fo4lNZ84x9Q?si=WdcYPZp-9VJnZEnC" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Copy and store the key in a secure place for future use.

## Setting Up a WhatsApp Business Account

 To integrate ChatGPT with WhatsApp, you must set up a WhatsApp Business account. Note that [WhatsApp Business is different from regular WhatsApp](https://www.makeuseof.com/whatsapp-vs-whatsapp-business/). This account will allow you to access the [WhatsApp Business API](https://business.whatsapp.com/developers/developer-hub), which you will integrate with the ChatGPT API.

 The full source code is available in a [GitHub repository](https://github.com/makeuseofcode/WhatsApp-ChatGPT-integration).

 You can use a third-party service like Kommunicate, a WhatsApp chatbot, or a Python script to integrate ChatGPT with WhatsApp. This tutorial’s focus will be on integrating ChatGPT using a Python script. It will then give you an overview of integration using a WhatsApp chatbot.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/NTQGoOOiJzs?si=zbZwflEfXgBY3qbs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/xIP8ktrmOdg?si=zRnjbGzM6PDx2jCq" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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

 Move to your WhatsApp mobile app and navigate to **Settings > QR code > Scan code** to add a new linked device and scan the popped QR code on your terminal.

 After logging in, the application will start listening to incoming messages. If someone sends a message, the received message will make a GET request to API with the message as a query parameter and send the response back to the sender on WhatsApp.

 Expected output:

![Output of integrating chatgpt and WhatsApp](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/integrating-whatsapp-and-chatgpt-api-output.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/3hS27nZVi9Y?si=_Zqj_l4a4XkPqT2S" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## Using WhatsApp Chatbot to Integrate WhatsApp With ChatGPT API

 Another way to integrate ChatGPT into WhatsApp messages is by using a WhatsApp chatbot.

 Once you register your WhatsApp Business API, use a chat builder like OpenDialog to create a flow for the chat. You will then test your chatbot and add it to your mobile phone.

### Integrate OpenAI API With Your WhatsApp Chatbot

 To integrate your WhatsApp chatbot with OpenAI models, use the API key from OpenAI.

 Integrating WhatsApp chatbots with OpenAI GPT models presents a risk of WhatsApp blocking your account on security claims.

 Though this method is easier if you already have a chatbot, you should only opt for it once you’re comfortable with the risks involved.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/QPAKth3O_5c?si=M69YSY0Mk_gsdU0Q" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://article-files.techidaily.com/new-2024-approved-exclusive-insiders-list-of-20-storage-services-unlimited-upload/"><u>[New] 2024 Approved Exclusive Insider's List of 20 Storage Services, Unlimited Upload</u></a></li>
<li><a href="https://facebook-clips.techidaily.com/new-in-2024-crafting-connections-the-art-and-science-of-personalized-facebook-profiles/"><u>[New] In 2024, Crafting Connections The Art and Science of Personalized Facebook Profiles</u></a></li>
<li><a href="https://twitter-videos.techidaily.com/new-winning-approach-to-saving-twitters-humor-for-2024/"><u>[New] Winning Approach to Saving Twitter's Humor for 2024</u></a></li>
<li><a href="https://youtube-clips.techidaily.com/updated-charting-the-course-from-scale-to-submillions-in-youtube/"><u>[Updated] Charting the Course From Scale to Submillions in Youtube</u></a></li>
<li><a href="https://extra-skills.techidaily.com/updated-mastering-the-art-of-import-in-windows-10-photo-space/"><u>[Updated] Mastering the Art of Import in Windows 10 Photo Space</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/apples-revolutionary-ai-powered-m3-macbook-air-review-how-its-changing-computing-for-all-featured-in-zdnet/"><u>Apple's Revolutionary AI-Powered M3 MacBook Air Review | How It's Changing Computing for All, Featured in ZDNet.</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/comparing-google-pixel-watch-and-apple-watch-series-9-is-it-worth-upgrading-expert-insights-from-zdnet/"><u>Comparing Google Pixel Watch and Apple Watch Series 9 – Is It Worth Upgrading? Expert Insights From ZDNet</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/comprehensive-guide-to-leading-ai-notetakers/"><u>Comprehensive Guide to Leading AI Notetakers</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/dialogue-engine-differences-10-highlights-of-ai-discrepanrances/"><u>Dialogue Engine Differences: 10 Highlights of AI Discrepanrances</u></a></li>
<li><a href="https://extra-lessons.techidaily.com/digital-diaspora-mixing-music-and-memory-images/"><u>Digital Diaspora Mixing Music and Memory Images</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/elevate-your-iphone-experience-must-have-anker-charger-additions-coming-soon-zdnet/"><u>Elevate Your iPhone Experience: Must-Have Anker Charger Additions Coming Soon - ZDNet</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/eu-levies-2b-penalty-on-apple-for-monopolistic-practices-in-app-store-business-insight-from-zdnet/"><u>EU Levies $2B Penalty on Apple for Monopolistic Practices in App Store Business - Insight From ZDNet</u></a></li>
<li><a href="https://fake-location.techidaily.com/fixing-foneazy-mockgo-not-working-on-oneplus-11-5g-drfone-by-drfone-virtual-android/"><u>Fixing Foneazy MockGo Not Working On OnePlus 11 5G | Dr.fone</u></a></li>
<li><a href="https://techno-recovery.techidaily.com/meta-vs-apple-in-the-vr-arena-exploring-metas-secret-tech-advantage-with-zdnets-in-depth-analysis/"><u>Meta Vs. Apple in the VR Arena: Exploring Meta's Secret Tech Advantage with ZDNet's In-Depth Analysis</u></a></li>
<li><a href="https://buynow-tips.techidaily.com/monoprices-economical-masterpiece-a-detailed-review-of-its-pro-artist-features-without-breaking-the-bank/"><u>Monoprice's Economical Masterpiece: A Detailed Review of Its Pro Artist Features Without Breaking the Bank</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/redefining-cinematic-exploration-via-vr-for-2024/"><u>Redefining Cinematic Exploration via VR for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/top-3-key-oversights-with-ml-algorithms/"><u>Top 3 Key Oversights with ML Algorithms</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/top-budget-friendly-tablets-comprehensive-reviews-by-tech-experts-zdnet/"><u>Top Budget-Friendly Tablets : Comprehensive Reviews by Tech Experts | ZDNet</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/uncover-the-truth-how-to-determine-if-someones-using-an-airtag-to-locate-you/"><u>Uncover the Truth: How to Determine If Someone's Using an AirTag to Locate You</u></a></li>
</ul></div>

