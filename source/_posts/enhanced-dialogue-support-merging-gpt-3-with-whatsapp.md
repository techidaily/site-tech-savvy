---
title: "Enhanced Dialogue Support: Merging GPT-3 with WhatsApp"
date: 2024-08-15T02:39:04.090Z
updated: 2024-08-16T02:39:04.090Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Enhanced Dialogue Support: Merging GPT-3 with WhatsApp"
excerpt: "This Article Describes Enhanced Dialogue Support: Merging GPT-3 with WhatsApp"
thumbnail: https://thmb.techidaily.com/6a8b7b3cdb25a03e07ba1819bb3940ce3cb079bf3680cebd2f9e48a956c136d3.jpg
---

## Enhanced Dialogue Support: Merging GPT-3 with WhatsApp

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
<a href="https://store.iobit.com/order/checkout.php?PRODS=1468905&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/184260348236f9554fe9375772ff966e/ascscan_728x90.png" border="0"></a>
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
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4721564&QTY=1&AFFILIATE=108875&CART=1">Power Tools add-on for Google Sheets, 12-month subscription</a>
<!-- affiliate ads end -->

 Move to your WhatsApp mobile app and navigate to **Settings > QR code > Scan code** to add a new linked device and scan the popped QR code on your terminal.

 After logging in, the application will start listening to incoming messages. If someone sends a message, the received message will make a GET request to API with the message as a query parameter and send the response back to the sender on WhatsApp.

 Expected output:

![Output of integrating chatgpt and WhatsApp](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/integrating-whatsapp-and-chatgpt-api-output.jpg)
<!-- affiliate ads begin -->
<a href="https://store.nero.com/order/checkout.php?PRODS=42296855&QTY=1&AFFILIATE=108875&CART=1"><img src="http://cdnwww.nero.com/nero-com-wAssets/img/banners/2023/recode/Nero_Recode_Screen_2.png" border="0"></a>
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
<a href="https://store.massmailsoftware.com/order/checkout.php?PRODS=1300375&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/dc87c13749315c7217cdc4ac692e704c/banera_for_partners-15_%281%29.jpg" border="0"></a>
<!-- affiliate ads end -->
### Testing Your WhatsApp Chatbot

 Like all AI API systems, testing is key before you deploy your WhatsApp chatbot. This is to ensure that it works as expected. API testing tools like Postman and Curl can help to test your chatbot’s responses.

 In this case, the Django REST framework provides a browsable API to help test API requests and responses.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2087267/19272" target="_top" id="2087267"><img src="//a.impactradius-go.com/display-ad/19272-2087267" border="0" alt="" width="728" height="90"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2087267/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
### Measuring Success and Fine-Tuning

 Once your WhatsApp chatbot is in deployment, it is crucial to measure its success and usage over time. This will help with fine-tuning it accordingly. Analytics tools like OpenDialog and Rasa can help to track metrics such as response time, retention rate, and customer satisfaction.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4712430&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/c404a5adbf90e09631678b13b05d9d7a/products/dlnow_256.png" border="0">DLNow Video Downloader</a>
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
<li><a href="https://youtube-docs.techidaily.com/024-approved-top-ten-lady-gamers-on-youtube-rising/"><u>[New] 2024 Approved  Top Ten Lady Gamers on YouTube Rising</u></a></li>
<li><a href="https://snapchat-videos.techidaily.com/new-elevating-your-selfies-the-art-of-drawing-with-filters-for-2024/"><u>[New] Elevating Your Selfies  The Art of Drawing with Filters for 2024</u></a></li>
<li><a href="https://facebook-videos.techidaily.com/new-in-2024-finding-the-right-angle-for-your-fb-videos/"><u>[New] In 2024, Finding the Right Angle for Your FB Videos</u></a></li>
<li><a href="https://eaxpv-info.techidaily.com/new-in-2024-harness-the-power-of-keywords-top-selection-software-unveiled/"><u>[New] In 2024, Harness the Power of Keywords  Top Selection Software Unveiled</u></a></li>
<li><a href="https://digital-screen-recording.techidaily.com/new-in-2024-strategies-to-maintain-synchronization-between-cameras-and-streaming-software/"><u>[New] In 2024, Strategies to Maintain Synchronization Between Cameras and Streaming Software</u></a></li>
<li><a href="https://screen-activity-recording.techidaily.com/2024-approved-soundscape-archives-collect-and-evaluate-recordings/"><u>2024 Approved  Soundscape Archives  Collect & Evaluate Recordings</u></a></li>
<li><a href="https://extra-lessons.techidaily.com/a-step-by-step-manual-for-stunning-slow-motion-with-gopro-hero-10-for-2024/"><u>A Step-by-Step Manual for Stunning Slow Motion with GoPro Hero 10 for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-and-job-evolution-the-next-big-shift/"><u>AI and Job Evolution: The Next Big Shift</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/are-gpt-enhanced-jobs-the-next-big-income-boost/"><u>Are GPT-Enhanced Jobs the Next Big Income Boost?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/character-depth-explored-top-11-chatgpt-inquiry-models/"><u>Character Depth Explored: Top 11 ChatGPT Inquiry Models</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/coding-elegance-with-python-and-gpt-3-synergy/"><u>Coding Elegance with Python & GPT-3 Synergy</u></a></li>
<li><a href="https://techidaily.com/complete-tutorial-for-xiaomi-redmi-note-12t-pro-hard-reset-drfone-by-drfone-reset-android-reset-android/"><u>Complete Tutorial for Xiaomi Redmi Note 12T Pro Hard Reset | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/content-enhancement-through-smart-ai-technology/"><u>Content Enhancement Through Smart AI Technology</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/deciphering-chatgpt-unleashing-the-power-of-ai-generation/"><u>Deciphering ChatGPT: Unleashing the Power of AI Generation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/dissecting-linguistics-tech-nlp-vs-ml/"><u>Dissecting Linguistics Tech: NLP vs ML</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/diving-into-digital-dialogue-googles-groundbreayer-palm-2/"><u>Diving Into Digital Dialogue: Google's Groundbreayer, PaLM 2</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/empowering-conversations-mastering-chatgpt-on-iphone-via-siri/"><u>Empowering Conversations: Mastering ChatGPT on iPhone via Siri</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/enhance-user-experience-by-leveraging-chatgpts-4-elements/"><u>Enhance User Experience by Leveraging ChatGPT's 4 Elements</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/essential-list-of-leading-artificial-intelligence-note-taking-apps/"><u>Essential List of Leading Artificial Intelligence Note-Taking Apps</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/examining-ai-for-perfected-cocktail-recipes/"><u>Examining AI for Perfected Cocktail Recipes</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/from-concept-to-creation-building-apps-with-chatgpts-insight/"><u>From Concept to Creation: Building Apps with ChatGPT's Insight</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/from-simple-ai-to-sophisticated-gpt-4/"><u>From Simple AI to Sophisticated GPT-4</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/googles-gemini-navigating-through-its-artificial-intelligence-landscape/"><u>Google’s Gemini: Navigating Through Its Artificial Intelligence Landscape</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/has-openai-fallen-behind-gpt/"><u>Has OpenAI Fallen Behind GPT?</u></a></li>
<li><a href="https://fake-location.techidaily.com/how-to-find-ispoofer-pro-activation-key-on-vivo-x100-pro-drfone-by-drfone-virtual-android/"><u>How to Find iSpoofer Pro Activation Key On Vivo X100 Pro? | Dr.fone</u></a></li>
<li><a href="https://fox-access.techidaily.com/how-to-smoothly-manipulate-video-speed-in-snapchat-for-2024/"><u>How to Smoothly Manipulate Video Speed in Snapchat for 2024</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/how-to-unlock-sim-card-on-lava-blaze-pro-5g-online-without-jailbreak-by-drfone-android/"><u>How to Unlock SIM Card on Lava Blaze Pro 5G online without jailbreak</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/in-2024-the-best-android-sim-unlock-code-generators-unlock-your-huawei-nova-y91-phone-hassle-free-by-drfone-android/"><u>In 2024, The Best Android SIM Unlock Code Generators Unlock Your Huawei Nova Y91 Phone Hassle-Free</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-safe-use-of-deep-learning-algos/"><u>Mastering Safe Use of Deep Learning Algos</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/modern-ai-metrics-beyond-the-historical-turing-index/"><u>Modern AI Metrics: Beyond the Historical Turing Index</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/paramount-considerations-in-utilizing-artificial-intelligence-for-emotional-support-via-chatgpt/"><u>Paramount Considerations in Utilizing Artificial Intelligence for Emotional Support via ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/pathway-to-peak-performance-chatgpts-wellbe-point-of-view/"><u>Pathway to Peak Performance: ChatGPT's Wellbe Point of View</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/perfect-your-verbal-direction-mastering-gpt-with-5-voice-based-strategies/"><u>Perfect Your Verbal Direction: Mastering GPT with 5 Voice-Based Strategies</u></a></li>
<li><a href="https://data-wizards.techidaily.com/phoenix-assistance-stellars-server-sos-help/"><u>Phoenix Assistance: Stellar's Server SOS Help</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/politeness-in-the-age-of-ai-engaging-with-gpt-alexa-and-more/"><u>Politeness in the Age of AI: Engaging with GPT, Alexa & More</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/prompting-proficiency-leading-ai-training-modules/"><u>Prompting Proficiency: Leading AI Training Modules</u></a></li>
<li><a href="https://buynow-marvelous.techidaily.com/q30-soundcore-life-comprehensive-affordable-headphone-insight/"><u>Q30 Soundcore Life: Comprehensive Affordable Headphone Insight</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/rethink-ai-six-reasons-to-approach-with-skepticism/"><u>Rethink AI: Six Reasons to Approach with Skepticism</u></a></li>
<li><a href="https://facebook-video-share.techidaily.com/revolutionizing-channel-presence-the-secret-of-higher-subscriber-numbers-for-2024/"><u>Revolutionizing Channel Presence  The Secret of Higher Subscriber Numbers for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revolutionizing-health-care-with-chatgpts-top-9-tactics/"><u>Revolutionizing Health Care with ChatGPT’s Top 9 Tactics</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/streamlined-academic-success-through-gpt-assisted-notes/"><u>Streamlined Academic Success Through GPT-Assisted Notes</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/three-simple-steps-for-free-gpt-4-usage/"><u>Three Simple Steps for Free GPT-4 Usage</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/top-5-voice-commands-for-mastering-chatgpt/"><u>Top 5 Voice Commands for Mastering ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/top-7-hidden-traps-of-ai-text-synthesis/"><u>Top 7 Hidden Traps of AI Text Synthesis</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unleashing-paperclip-potential-through-ai-interaction-and-analysis/"><u>Unleashing Paperclip Potential Through AI Interaction and Analysis</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unleashing-the-best-ai-gpt-showdown-with-microsoft-and-google-bard/"><u>Unleashing the Best AI: GPT Showdown with Microsoft and Google Bard</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/why-distrust-in-artificial-intelligence-isnt-extreme/"><u>Why Distrust in Artificial Intelligence Isn't Extreme</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/why-not-rely-on-chatgpt-for-complete-text-synopses/"><u>Why Not Rely on ChatGPT for Complete Text Synopses?</u></a></li>
</ul></div>
