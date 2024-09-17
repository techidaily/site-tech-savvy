---
title: "Uniting Customer Care: ChatGPT Meets WhatsApp"
date: 2024-09-14T16:28:58.066Z
updated: 2024-09-17T16:16:18.378Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Uniting Customer Care: ChatGPT Meets WhatsApp"
excerpt: "This Article Describes Uniting Customer Care: ChatGPT Meets WhatsApp"
thumbnail: https://thmb.techidaily.com/c95c5b89385ea5c16d5bf29142574c7f6fa915aba69d6f94485f47171ff348f2.jpg
---

## Uniting Customer Care: ChatGPT Meets WhatsApp

 Today’s businesses embrace messaging apps like WhatsApp to communicate with customers. This results in a surge in the automation of business customer interactions using chatbots.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 Such a chatbot is ChatGPT, a large language model by OpenAI that you can integrate with WhatsApp to automate customer interactions by providing fast and accurate responses to customer queries.

>  Disclaimer: This post includes affiliate links
>
>  If you click on a link and make a purchase, I may receive a commission at no extra cost to you.
>

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

## Setting Up a WhatsApp Business Account

 To integrate ChatGPT with WhatsApp, you must set up a WhatsApp Business account. Note that [WhatsApp Business is different from regular WhatsApp](https://www.makeuseof.com/whatsapp-vs-whatsapp-business/). This account will allow you to access the [WhatsApp Business API](https://business.whatsapp.com/developers/developer-hub), which you will integrate with the ChatGPT API.

 The full source code is available in a [GitHub repository](https://github.com/makeuseofcode/WhatsApp-ChatGPT-integration).

 You can use a third-party service like Kommunicate, a WhatsApp chatbot, or a Python script to integrate ChatGPT with WhatsApp. This tutorial’s focus will be on integrating ChatGPT using a Python script. It will then give you an overview of integration using a WhatsApp chatbot.

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
<a href="https://aligracehair.sjv.io/c/5597632/2135361/19272" target="_top" id="2135361">
  <img src="//a.impactradius-go.com/display-ad/19272-2135361" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135361/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

## Using WhatsApp Chatbot to Integrate WhatsApp With ChatGPT API

 Another way to integrate ChatGPT into WhatsApp messages is by using a WhatsApp chatbot.

 Once you register your WhatsApp Business API, use a chat builder like OpenDialog to create a flow for the chat. You will then test your chatbot and add it to your mobile phone.

### Integrate OpenAI API With Your WhatsApp Chatbot

 To integrate your WhatsApp chatbot with OpenAI models, use the API key from OpenAI.

 Integrating WhatsApp chatbots with OpenAI GPT models presents a risk of WhatsApp blocking your account on security claims.

 Though this method is easier if you already have a chatbot, you should only opt for it once you’re comfortable with the risks involved.

### Configuring Automated Responses

 To get better customer service, configure automated responses to provide fast and accurate responses to customer messages. These responses will personalize the customer by name and provide relevant responses to customer queries.

<!-- affiliate ads begin -->
<span id="1975555">
					<video width="128" height="480" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1975555.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/22993-1975555">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1975555.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:80px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fhomestyler.sjv.io%2Fc%2F5597632%2F1975555%2F22993'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1975555/22993" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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
<li><a href="https://video-screen-grab.techidaily.com/updated-2024-approved-examining-splitcam-top-video-recorder/"><u>[Updated] 2024 Approved Examining SplitCam Top Video Recorder?</u></a></li>
<li><a href="https://video-screen-grab.techidaily.com/updated-2024-approved-the-complete-users-manual-to-zoom-meeting-recordings/"><u>[Updated] 2024 Approved The Complete User's Manual to Zoom Meeting Recordings</u></a></li>
<li><a href="https://video-screen-grab.techidaily.com/updated-freecam-x-live-streaming-software-reviewed-for-2024/"><u>[Updated] FreeCam X Live Streaming Software Reviewed for 2024</u></a></li>
<li><a href="https://howto.techidaily.com/app-wont-open-on-your-asus-rog-phone-7-ultimate-here-are-all-fixes-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>App Wont Open on Your Asus ROG Phone 7 Ultimate? Here Are All Fixes | Dr.fone</u></a></li>
<li><a href="https://fake-location.techidaily.com/how-to-fix-my-asus-rog-phone-7-ultimate-location-is-wrong-drfone-by-drfone-virtual-android/"><u>How to Fix My Asus ROG Phone 7 Ultimate Location Is Wrong | Dr.fone</u></a></li>
<li><a href="https://iphone-transfer.techidaily.com/in-2024-5-tutorials-on-how-to-transfer-photos-from-apple-iphone-15-plus-to-new-iphone-drfone-by-drfone-transfer-from-ios/"><u>In 2024, 5 Tutorials on How to Transfer Photos From Apple iPhone 15 Plus to New iPhone | Dr.fone</u></a></li>
<li><a href="https://change-location.techidaily.com/in-2024-detailed-guide-of-ispoofer-for-pogo-installation-on-samsung-galaxy-s24-ultra-drfone-by-drfone-virtual-android/"><u>In 2024, Detailed guide of ispoofer for pogo installation On Samsung Galaxy S24 Ultra | Dr.fone</u></a></li>
<li><a href="https://youtube-tips.techidaily.com/izing-your-videos-impact-with-perfect-post-times-for-2024/"><u>Maximizing Your Videos' Impact with Perfect Post Times for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/simple-guide-to-converting-your-dvds-into-avi-files-with-no-hassle/"><u>Simple Guide to Converting Your DVDs Into AVI Files with No Hassle</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/simple-guide-change-wmv-videos-into-mp4-mov-and-mp3-formats-with-one-click/"><u>Simple Guide: Change WMV Videos Into MP4, Mov & MP3 Formats with One-Click</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/slice-the-baguette-lengthwise-but-not-all-the-way-through-leave-about-an-inch-of-bread-intact-at-one-end-to-hold-it-together/"><u>Slice the Baguette Lengthwise, but Not All the Way Through – Leave About an Inch of Bread Intact at One End to Hold It Together.</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/step-by-step-guide-maintaining-high-definition-clarity-while-uploading-your-videos-on-youtube/"><u>Step-by-Step Guide: Maintaining High Definition Clarity While Uploading Your Videos on YouTube</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/top-6-mp4-to-gif-conversion-tools-for-windows-users-the-ultimate-guide/"><u>Top 6 MP4 to GIF Conversion Tools for Windows Users: The Ultimate Guide</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/transforming-your-videos-from-wmv-to-avi-format-easily/"><u>Transforming Your Videos From WMV to AVI Format Easily</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/troubleshooting-the-movietv-app-in-windows-11-essential-tips-for-smooth-playback/"><u>Troubleshooting the MovieTV App in Windows 11: Essential Tips for Smooth Playback</u></a></li>
</ul></div>

