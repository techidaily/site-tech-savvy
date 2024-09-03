---
title: "Uniting Messaging and AI: ChatGPT in WhatsApp Support"
date: 2024-09-02T20:37:32.977Z
updated: 2024-09-03T20:37:32.977Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Uniting Messaging and AI: ChatGPT in WhatsApp Support"
excerpt: "This Article Describes Uniting Messaging and AI: ChatGPT in WhatsApp Support"
thumbnail: https://thmb.techidaily.com/c3ecdd732aca091f9e06be3caec567f3fcd17c056bf2dd14982465e8c7b5b6a1.jpg
---

## Uniting Messaging and AI: ChatGPT in WhatsApp Support

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

## Setting Up a WhatsApp Business Account

 To integrate ChatGPT with WhatsApp, you must set up a WhatsApp Business account. Note that [WhatsApp Business is different from regular WhatsApp](https://www.makeuseof.com/whatsapp-vs-whatsapp-business/). This account will allow you to access the [WhatsApp Business API](https://business.whatsapp.com/developers/developer-hub), which you will integrate with the ChatGPT API.

 The full source code is available in a [GitHub repository](https://github.com/makeuseofcode/WhatsApp-ChatGPT-integration).

 You can use a third-party service like Kommunicate, a WhatsApp chatbot, or a Python script to integrate ChatGPT with WhatsApp. This tutorial’s focus will be on integrating ChatGPT using a Python script. It will then give you an overview of integration using a WhatsApp chatbot.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4718728&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/ce9a6fb2becc2d235e62b125e9260102/products/vMixCallScreenshot1-large.jpg" border="0"> vMix Basic HD - Software based live production. vMix Basic HD includes 4 inputs, 3 cameras, streaming, recording, playlist. 
This bundle includes Studio 200 for vMix from Virtualsetworks, HTTP Matrix 1.0 automation scheduler, and 4 introductory training videos from the Udemy vMix Basic to Amazing course. </a>
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
<a href="https://shop.copernic.com/order/checkout.php?PRODS=41033091&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.2checkout.com/images/merchant/8d30aa96e72440759f74bd2306c1fa3d/Copernic-2023-Affiliate-728x90-Advanced.png" border="0"></a>
<!-- affiliate ads end -->
## Using WhatsApp Chatbot to Integrate WhatsApp With ChatGPT API

 Another way to integrate ChatGPT into WhatsApp messages is by using a WhatsApp chatbot.

 Once you register your WhatsApp Business API, use a chat builder like OpenDialog to create a flow for the chat. You will then test your chatbot and add it to your mobile phone.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=38729081&QTY=1&AFFILIATE=108875&CART=1"><img src="https://website-prod.cache.wpscdn.com/img/wps-writer-free-word-processor-1x.3d9c80d.png" border="0">
WPS Office Premium ( File Recovery, Photo Scanning, Convert PDF)--Yearly</a>
<!-- affiliate ads end -->
### Integrate OpenAI API With Your WhatsApp Chatbot

 To integrate your WhatsApp chatbot with OpenAI models, use the API key from OpenAI.

 Integrating WhatsApp chatbots with OpenAI GPT models presents a risk of WhatsApp blocking your account on security claims.

 Though this method is easier if you already have a chatbot, you should only opt for it once you’re comfortable with the risks involved.

<!-- affiliate ads begin -->
<a href="https://boody-eco-wear.pxf.io/c/5597632/1567905/13846" target="_top" id="1567905"><img src="//a.impactradius-go.com/display-ad/13846-1567905" border="0" alt="" width="300" height="250"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1567905/13846" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
### Configuring Automated Responses

 To get better customer service, configure automated responses to provide fast and accurate responses to customer messages. These responses will personalize the customer by name and provide relevant responses to customer queries.

### Testing Your WhatsApp Chatbot

 Like all AI API systems, testing is key before you deploy your WhatsApp chatbot. This is to ensure that it works as expected. API testing tools like Postman and Curl can help to test your chatbot’s responses.

 In this case, the Django REST framework provides a browsable API to help test API requests and responses.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4726960&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/5f4f7141b65a730b4efb0e0d51f63e94/products/forexrobotronbox.gif" border="0">Forex Robotron Basic Package</a>
<!-- affiliate ads end -->
### Measuring Success and Fine-Tuning

 Once your WhatsApp chatbot is in deployment, it is crucial to measure its success and usage over time. This will help with fine-tuning it accordingly. Analytics tools like OpenDialog and Rasa can help to track metrics such as response time, retention rate, and customer satisfaction.

<!-- affiliate ads begin -->
<span id="1997795">
					<video width="250" height="250" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1997795.jpeg"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/23621-1997795">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1997795.jpeg" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:250px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fproteahair.pxf.io%2Fc%2F5597632%2F1997795%2F23621'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1997795/23621" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
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
<li><a href="https://instagram-clips.techidaily.com/new-2024-approved-boost-your-instagram-with-easily-shareable-gifs-step-by-step/"><u>[New] 2024 Approved  Boost Your Instagram with Easily Shareable GIFs (Step-by-Step)</u></a></li>
<li><a href="https://facebook-video-recording.techidaily.com/new-2024-approved-horizontal-vs-vertical-best-for-fb-videos/"><u>[New] 2024 Approved  Horizontal Vs. Vertical  Best for FB Videos?</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/new-2024-approved-unmasked-instagram-stories-pcandroidios-exploration-tips/"><u>[New] 2024 Approved  Unmasked Instagram Stories  PC/Android/iOS Exploration Tips</u></a></li>
<li><a href="https://screen-activity-recording.techidaily.com/new-boost-engagement-using-obs-for-youtube-and-twitch-audiences/"><u>[New] Boost Engagement Using OBS for YouTube & Twitch Audiences</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-expeditious-windows-file-audit-tactics/"><u>[New] Expeditious Windows File Audit Tactics</u></a></li>
<li><a href="https://extra-lessons.techidaily.com/new-how-to-create-time-travel-teleportation-effects/"><u>[New] How to Create Time Travel Teleportation Effects</u></a></li>
<li><a href="https://some-guidance.techidaily.com/new-superior-visual-experience-ranking-the-best-12-html5-players/"><u>[New] Superior Visual Experience  Ranking the Best 12 HTML5 Players</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/updated-high-fidelity-graphics-on-4k-an-in-depth-look-at-proart-monitors/"><u>[Updated] High-Fidelity Graphics on 4K  An In-Depth Look at ProArt Monitors</u></a></li>
<li><a href="https://youtube-stream.techidaily.com/2024-approved-uncover-the-leaders-1-6-in-global-short-video-clips/"><u>2024 Approved  Uncover the Leaders  #1-#6 in Global Short Video Clips</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-and-the-future-of-professional-development/"><u>AI & the Future of Professional Development</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/androidios-accessibility-with-chatgpt/"><u>Android/iOS Accessibility with ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/biz-revolution-simplified-incoritsion-of-whisper-and-gptapis/"><u>Biz Revolution Simplified: Incoritsion of Whisper & GPTAPIs</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-steps-for-soothing-the-soul/"><u>ChatGPT Steps for Soothing the Soul</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-the-ai-you-can-chit-chat-with/"><u>ChatGPT: The AI You Can Chit-Chat With</u></a></li>
<li><a href="https://techidaily.com/complete-tutorial-for-realme-11-5g-hard-reset-drfone-by-drfone-reset-android-reset-android/"><u>Complete Tutorial for Realme 11 5G Hard Reset | Dr.fone</u></a></li>
<li><a href="https://win-amazing.techidaily.com/download-latest-nvidia-graphics-drivers-compatible-with-windows-11-7-and-8/"><u>Download Latest NVIDIA Graphics Drivers Compatible with Windows 11, 7 & 8</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/elevate-spreadsheet-skills-with-chatgpts-insight/"><u>Elevate Spreadsheet Skills with ChatGPT's Insight</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/eliminating-chatgpts-memory-retention-feature/"><u>Eliminating ChatGPT’s Memory Retention Feature</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/enabling-autodoc-chatgpts-role-in-office-productivity/"><u>Enabling AutoDoc: ChatGPT's Role in Office Productivity</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/enhancing-pc-interaction-with-nvidias-ai-assistant/"><u>Enhancing PC Interaction with Nvidia’s AI Assistant</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/expert-advice-dodging-chatgpt-written-errors/"><u>Expert Advice: Dodging ChatGPT' Written Errors</u></a></li>
<li><a href="https://instagram-clips.techidaily.com/expert-strategies-to-master-the-instagram-query-tag/"><u>Expert Strategies to Master the Instagram Query Tag</u></a></li>
<li><a href="https://ai-topics.techidaily.com/exploring-ai-face-generators-for-2024/"><u>Exploring AI Face Generators for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/exploring-the-dynamics-of-shared-links-in-chatgpt/"><u>Exploring the Dynamics of Shared Links in ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/from-kitchen-clips-to-high-tech-how-ai-influences-paperclip-problem-solving/"><u>From Kitchen Clips to High-Tech: How AI Influences Paperclip Problem Solving</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/gpt-powered-gameplay-the-dandd-advantage-guide/"><u>GPT-Powered Gameplay: The D&D Advantage Guide</u></a></li>
<li><a href="https://android-transfer.techidaily.com/how-to-transfer-data-from-oneplus-ace-2-to-any-ios-devices-drfone-by-drfone-transfer-from-android-transfer-from-android/"><u>How to Transfer Data from OnePlus Ace 2 to Any iOS Devices | Dr.fone</u></a></li>
<li><a href="https://screen-recording.techidaily.com/in-2024-best-screen-capture-alternatives-for-the-cost-conscious-user/"><u>In 2024, Best Screen Capture Alternatives for the Cost-Conscious User</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/in-2024-from-raw-footage-to-instagram-gold-top-10-editor-shortlists/"><u>In 2024, From Raw Footage to Instagram Gold - Top 10 Editor Shortlists</u></a></li>
<li><a href="https://easy-unlock-android.techidaily.com/in-2024-how-to-show-wi-fi-password-on-poco-m6-pro-5g-by-drfone-android/"><u>In 2024, How to Show Wi-Fi Password on Poco M6 Pro 5G</u></a></li>
<li><a href="https://screen-sharing-recording.techidaily.com/in-2024-the-ultimate-guide-to-video-capture-obs-versus-bandicam/"><u>In 2024, The Ultimate Guide to Video Capture  OBS versus Bandicam</u></a></li>
<li><a href="https://discover-brilliant.techidaily.com/leverage-cookiebot-power-for-advanced-seo-optimization-techniques/"><u>Leverage Cookiebot Power for Advanced SEO Optimization Techniques</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/maintain-silence-on-secrets-not-with-gpt-assistance/"><u>Maintain Silence on Secrets, Not with GPT Assistance</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/maximizing-excel-potential-via-three-chatgpt-techniques/"><u>Maximizing Excel Potential via Three ChatGPT Techniques</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/quick-and-quality-aid-crafting-top-7-web-based-assistance-tools/"><u>Quick and Quality Aid Crafting: Top 7 Web-Based Assistance Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/redesigning-careers-with-the-power-of-generative-ai/"><u>Redesigning Careers with the Power of Generative AI</u></a></li>
<li><a href="https://extra-lessons.techidaily.com/reviewing-ion-air-pro-3-capturing-life-in-high-definition/"><u>Reviewing ION Air Pro 3 - Capturing Life in High Definition</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revolutionizing-presentations-7-leading-ai-innovators/"><u>Revolutionizing Presentations: 7 Leading AI Innovators</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/separating-fact-from-fiction-in-ai-health-suggestions/"><u>Separating Fact From Fiction in AI Health Suggestions</u></a></li>
<li><a href="https://data-safeguard.techidaily.com/simple-steps-for-recovering-removed-content-from-an-idevice-using-stellar-tech/"><u>Simple Steps for Recovering Removed Content From an iDevice Using Stellar Tech</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/smart-resume-writing-leverage-ai-inspire-employers/"><u>Smart Résumé Writing: Leverage AI, Inspire Employers</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/steps-to-handle-maxed-out-windows-chatgpt/"><u>Steps to Handle Maxed-Out Windows ChatGPT</u></a></li>
<li><a href="https://screen-sharing-recording.techidaily.com/swift-and-simple-method-for-screenshots-on-ios-devices/"><u>Swift and Simple Method for Screenshots on IOS Devices</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-artificers-pitfall-spotting-pretend-projections-by-algorithms/"><u>The Artificer's Pitfall: Spotting Pretend Projections by Algorithms</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-comparative-analysis-of-online-bot-intelligence/"><u>The Comparative Analysis of Online Bot Intelligence</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-game-changing-reasons-mastery-of-chatgpt-in-your-career/"><u>The Game-Changing Reasons: Mastery of ChatGPT in Your Career</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-plain-truth-about-virtual-conversations-dispelling-ai-bot-fables/"><u>The Plain Truth About Virtual Conversations - Dispelling AI Bot Fables</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/tracing-sentimental-codes-in-artificayer-emotion-interaction/"><u>Tracing Sentimental Codes in Artificayer-Emotion Interaction</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unlocking-verse-potential-with-intelligent-ai-assistance/"><u>Unlocking Verse Potential with Intelligent AI Assistance</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-gptbotinasmuch-as-it-challenges-copyright-norms/"><u>Unveiling GPTBot'inasmuch As It Challenges Copyright Norms</u></a></li>
<li><a href="https://smart-video-creator.techidaily.com/updated-in-2024-online-video-combination-made-easy-top-5-free-tools/"><u>Updated In 2024, Online Video Combination Made Easy Top 5 Free Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/web-services-revolutionized-by-chatgpt-technology/"><u>Web Services Revolutionized by ChatGPT Technology</u></a></li>
<li><a href="https://review-topics.techidaily.com/why-your-whatsapp-live-location-is-not-updating-and-how-to-fix-on-your-vivo-y100i-power-5g-drfone-by-drfone-virtual-android/"><u>Why Your WhatsApp Live Location is Not Updating and How to Fix on your Vivo Y100i Power 5G | Dr.fone</u></a></li>
</ul></div>
