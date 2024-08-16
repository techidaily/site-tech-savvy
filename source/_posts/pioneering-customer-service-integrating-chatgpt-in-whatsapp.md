---
title: "Pioneering Customer Service: Integrating ChatGPT in WhatsApp"
date: 2024-08-15T02:44:29.056Z
updated: 2024-08-16T02:44:29.056Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Pioneering Customer Service: Integrating ChatGPT in WhatsApp"
excerpt: "This Article Describes Pioneering Customer Service: Integrating ChatGPT in WhatsApp"
thumbnail: https://thmb.techidaily.com/855361452192f3b7b7e7e407da45b95275a5f560d0d0de9b64cf3676aeaaee8b.jpg
---

## Pioneering Customer Service: Integrating ChatGPT in WhatsApp

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
<a href="https://store.massmailsoftware.com/order/checkout.php?PRODS=1095219&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/dc87c13749315c7217cdc4ac692e704c/banera_for_partners-20_%281%29.jpg" border="0"></a>
<!-- affiliate ads end -->
## Setting Up a WhatsApp Business Account

 To integrate ChatGPT with WhatsApp, you must set up a WhatsApp Business account. Note that [WhatsApp Business is different from regular WhatsApp](https://www.makeuseof.com/whatsapp-vs-whatsapp-business/). This account will allow you to access the [WhatsApp Business API](https://business.whatsapp.com/developers/developer-hub), which you will integrate with the ChatGPT API.

 The full source code is available in a [GitHub repository](https://github.com/makeuseofcode/WhatsApp-ChatGPT-integration).

 You can use a third-party service like Kommunicate, a WhatsApp chatbot, or a Python script to integrate ChatGPT with WhatsApp. This tutorial’s focus will be on integrating ChatGPT using a Python script. It will then give you an overview of integration using a WhatsApp chatbot.

<!-- affiliate ads begin -->
<a href="https://united.elfm.net/c/5597632/517826/4704" target="_top" id="517826"><img src="//a.impactradius-go.com/display-ad/4704-517826" border="0" alt="" width="728" height="90"/></a><img height="0" width="0" src="https://united.elfm.net/i/5597632/517826/4704" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://twopages.pxf.io/c/5597632/2016067/18544" target="_top" id="2016067"><img src="//a.impactradius-go.com/display-ad/18544-2016067" border="0" alt="" width="1020" height="380"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2016067/18544" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://sentrypc.7eer.net/c/5597632/398457/3022" target="_top" id="398457"><img src="//a.impactradius-go.com/display-ad/3022-398457" border="0" alt="www.sentrypc.com" width="980" height="120"/></a><img height="0" width="0" src="https://sentrypc.7eer.net/i/5597632/398457/3022" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Using WhatsApp Chatbot to Integrate WhatsApp With ChatGPT API

 Another way to integrate ChatGPT into WhatsApp messages is by using a WhatsApp chatbot.

 Once you register your WhatsApp Business API, use a chat builder like OpenDialog to create a flow for the chat. You will then test your chatbot and add it to your mobile phone.

### Integrate OpenAI API With Your WhatsApp Chatbot

 To integrate your WhatsApp chatbot with OpenAI models, use the API key from OpenAI.

 Integrating WhatsApp chatbots with OpenAI GPT models presents a risk of WhatsApp blocking your account on security claims.

 Though this method is easier if you already have a chatbot, you should only opt for it once you’re comfortable with the risks involved.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=35038891&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.dupinout.com/wp-content/uploads/2021/12/DupInOut-New-Duplicate-Scan-Tab.png" border="0"></a>
<!-- affiliate ads end -->
### Configuring Automated Responses

 To get better customer service, configure automated responses to provide fast and accurate responses to customer messages. These responses will personalize the customer by name and provide relevant responses to customer queries.

### Testing Your WhatsApp Chatbot

 Like all AI API systems, testing is key before you deploy your WhatsApp chatbot. This is to ensure that it works as expected. API testing tools like Postman and Curl can help to test your chatbot’s responses.

 In this case, the Django REST framework provides a browsable API to help test API requests and responses.

<!-- affiliate ads begin -->
<a href="https://store.nero.com/order/checkout.php?PRODS=42296855&QTY=1&AFFILIATE=108875&CART=1"><img src="http://cdnwww.nero.com/nero-com-wAssets/img/banners/2023/recode/Nero_Recode_Screen_2.png" border="0"></a>
<!-- affiliate ads end -->
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
<li><a href="https://facebook-record-videos.techidaily.com/updated-2024-approved-earning-by-critiquing-goodies-a-youtube-guide/"><u>[Updated] 2024 Approved  Earning by Critiquing Goodies  A YouTube Guide</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/updated-in-2024-streamlining-screenshot-tasks-in-minutes/"><u>[Updated] In 2024, Streamlining Screenshot Tasks in Minutes</u></a></li>
<li><a href="https://facebook-video-files.techidaily.com/updated-in-2024-techniques-for-effortless-facebook-video-posting-pcandroid/"><u>[Updated] In 2024, Techniques for Effortless Facebook Video Posting, PC/Android</u></a></li>
<li><a href="https://extra-skills.techidaily.com/updated-integrated-activity-evaluation-guide/"><u>[Updated] Integrated Activity Evaluation Guide</u></a></li>
<li><a href="https://screen-recording.techidaily.com/updated-plain-screen-recorder-windows-10-edition/"><u>[Updated] Plain Screen Recorder - Windows 10 Edition</u></a></li>
<li><a href="https://fox-hovers.techidaily.com/updated-superior-audio-modification-software-with-enchanting-features-for-2024/"><u>[Updated] Superior Audio Modification Software with Enchanting Features for 2024</u></a></li>
<li><a href="https://fox-direct.techidaily.com/2024-approved-the-ultimate-powerdirector-24-review-a-comprehensive-dive/"><u>2024 Approved  The Ultimate PowerDirector '24 Review  A Comprehensive Dive</u></a></li>
<li><a href="https://some-tips.techidaily.com/2024-approved-thriving-livestreams-strategies-for-beginners-with-low-followers/"><u>2024 Approved  Thriving Livestreams  Strategies for Beginners with Low Followers</u></a></li>
<li><a href="https://android-frp.techidaily.com/about-htc-u23-pro-frp-bypass-by-drfone-android/"><u>About HTC U23 Pro FRP Bypass</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-evaluation-reimagined-moving-past-the-turing-scale/"><u>AI Evaluation Reimagined: Moving Past the Turing Scale</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ais-impact-on-intellectual-quests/"><u>AI's Impact on Intellectual Quests</u></a></li>
<li><a href="https://tech-renaissance.techidaily.com/are-you-experiencing-psn-issues-or-is-the-service-actually-down-today/"><u>Are You Experiencing PSN Issues or Is the Service Actually Down Today?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/auditory-instructions-for-effective-chatgpt-commanding/"><u>Auditory Instructions for Effective ChatGPT Commanding</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/avoiding-content-duplication-in-language-bots/"><u>Avoiding Content Duplication in Language Bots</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpts-innovative-approaches-to-your-wellness-plan/"><u>ChatGPT’s Innovative Approaches to Your Wellness Plan</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chilling-out-cool-down-the-dough-just-right/"><u>Chilling Out: Cool Down the Dough Just Right</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/critical-analysis-of-chatgpt-unveiling-the-8-main-issues/"><u>Critical Analysis of ChatGPT: Unveiling the 8 Main Issues</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/digital-identity-creation-no-number-needed-for-services/"><u>Digital Identity Creation: No Number Needed for Services</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/discovering-ais-potential-four-fee-less-approaches/"><u>Discovering AI's Potential: Four Fee-Less Approaches</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/exploring-gpt-as-a-writing-checker/"><u>Exploring GPT as a Writing Checker</u></a></li>
<li><a href="https://techidaily.com/guide-on-how-to-erase-apple-iphone-13-pro-max-data-completely-drfone-by-drfone-ios-full-data-eraser-ios-full-data-eraser/"><u>Guide on How To Erase Apple iPhone 13 Pro Max Data Completely | Dr.fone</u></a></li>
<li><a href="https://unlock-android.techidaily.com/how-to-track-imei-number-of-honor-x7b-through-google-earth-by-drfone-android/"><u>How To Track IMEI Number Of Honor X7b Through Google Earth?</u></a></li>
<li><a href="https://blog-min.techidaily.com/how-to-transfer-data-from-iphone-11-pro-max-to-other-iphone-11-devices-drfone-by-drfone-transfer-data-from-ios-transfer-data-from-ios/"><u>How To Transfer Data From iPhone 11 Pro Max To Other iPhone 11 devices? | Dr.fone</u></a></li>
<li><a href="https://youtube-help.techidaily.com/in-2024-illuminated-insights-visualizing-youtubes-17-data-story/"><u>In 2024, Illuminated Insights! Visualizing YouTube's '17 Data Story</u></a></li>
<li><a href="https://extra-guidance.techidaily.com/in-2024-proven-steps-to-convert-webp-to-high-quality-jpeg/"><u>In 2024, Proven Steps to Convert WebP to High-Quality JPEG</u></a></li>
<li><a href="https://eaxpv-info.techidaily.com/piecing-together-attention-grabbing-channel-snippets-for-2024/"><u>Piecing Together Attention-Grabbing Channel Snippets for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/replicating-human-like-dialogue-with-ai/"><u>Replicating Human-Like Dialogue with AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revamping-ai-interactions-googles-gemini-vs-chatgpts-performance/"><u>Revamping AI Interactions – Google’s Gemini Vs. ChatGPT's Performance</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/sam-altman-steps-aside-does-it-change-gpt-landscape/"><u>Sam Altman Steps Aside; Does It Change GPT Landscape?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/simplifying-complexity-openais-ai-evolution-gpt-14/"><u>Simplifying Complexity: OpenAI's AI Evolution (GPT-1–4)</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-allure-of-ai-conversations-exploring-bot-usage/"><u>The Allure of AI Conversations: Exploring Bot Usage</u></a></li>
<li><a href="https://some-approaches.techidaily.com/the-documentarians-guide-to-captivating-audience-for-2024/"><u>The Documentarian's Guide to Captivating Audience for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-future-of-flirting-gpt-powered-dating/"><u>The Future of Flirting: GPT-Powered Dating</u></a></li>
<li><a href="https://android-location-track.techidaily.com/top-5-car-locator-apps-for-oneplus-12r-drfone-by-drfone-virtual-android/"><u>Top 5 Car Locator Apps for OnePlus 12R | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/vanguard-technologies-this-years-most-promising-ai-chips-and-processors/"><u>Vanguard Technologies: This Year's Most Promising AI Chips and Processors</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/when-machines-mentored-humanity-the-dawn-of-ai/"><u>When Machines Mentored Humanity: The Dawn of AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/wild-encounters-tamed-by-ai-dialogue-support/"><u>Wild Encounters Tamed by AI Dialogue Support</u></a></li>
</ul></div>
