---
title: "Streamlining Support Interaction: AI & WhatsApp Integration Guide"
date: 2024-08-29T19:46:00.841Z
updated: 2024-08-30T19:46:00.841Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Streamlining Support Interaction: AI & WhatsApp Integration Guide"
excerpt: "This Article Describes Streamlining Support Interaction: AI & WhatsApp Integration Guide"
thumbnail: https://thmb.techidaily.com/2a48b2247fe4fccf62c26b321b73686dd63d342e88315635def6454749492ddb.jpg
---

## Streamlining Support Interaction: AI & WhatsApp Integration Guide

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
<a href="https://laganoo.pxf.io/c/5597632/1657399/16446" target="_top" id="1657399"><img src="//a.impactradius-go.com/display-ad/16446-1657399" border="0" alt="" width="728" height="90"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1657399/16446" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://shop.pcdj.com/order/checkout.php?PRODS=4698998&QTY=1&AFFILIATE=108875&CART=1"> <img src="https://secure.avangate.com/images/merchant/47f4b6321e9fd8e8f7326a6adc1a7c1e/products/MacBook_Pro_lyrx-withsinger-tv.png" border="0">LYRX is an easy-to-use karaoke software with the professional features karaoke hosts need to perform with precision. LYRX is karaoke show hosting software that supports all standard karaoke file types as well as HD video formats, and it’s truly fun to use. 
LYRX Karaoke Software MAC/WINDOWS (Includes Activation For 3 Machines)</a>
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
<a href="https://shop.manycam.com/order/checkout.php?PRODS=17729331&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/8230bea7d54bcdf99cdfe85cb07313d5/mcaffbanner600x500.png" border="0"></a>
<!-- affiliate ads end -->
## Using WhatsApp Chatbot to Integrate WhatsApp With ChatGPT API

 Another way to integrate ChatGPT into WhatsApp messages is by using a WhatsApp chatbot.

 Once you register your WhatsApp Business API, use a chat builder like OpenDialog to create a flow for the chat. You will then test your chatbot and add it to your mobile phone.

<!-- affiliate ads begin -->
<a href="https://turtlebeachus.sjv.io/c/5597632/1988416/23719" target="_top" id="1988416"><img src="//a.impactradius-go.com/display-ad/23719-1988416" border="0" alt="" width="600" height="600"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1988416/23719" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
### Integrate OpenAI API With Your WhatsApp Chatbot

 To integrate your WhatsApp chatbot with OpenAI models, use the API key from OpenAI.

 Integrating WhatsApp chatbots with OpenAI GPT models presents a risk of WhatsApp blocking your account on security claims.

 Though this method is easier if you already have a chatbot, you should only opt for it once you’re comfortable with the risks involved.

### Configuring Automated Responses

 To get better customer service, configure automated responses to provide fast and accurate responses to customer messages. These responses will personalize the customer by name and provide relevant responses to customer queries.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4559731&QTY=1&AFFILIATE=108875&CART=1"><img src="http://www.neowise.com/images/nd-ss-w200.jpg" border="0">NeoDownloader - Fast and fully automatic image/video/music downloader. </a>
<!-- affiliate ads end -->
### Testing Your WhatsApp Chatbot

 Like all AI API systems, testing is key before you deploy your WhatsApp chatbot. This is to ensure that it works as expected. API testing tools like Postman and Curl can help to test your chatbot’s responses.

 In this case, the Django REST framework provides a browsable API to help test API requests and responses.

### Measuring Success and Fine-Tuning

 Once your WhatsApp chatbot is in deployment, it is crucial to measure its success and usage over time. This will help with fine-tuning it accordingly. Analytics tools like OpenDialog and Rasa can help to track metrics such as response time, retention rate, and customer satisfaction.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4699091&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/bccefcc1b1eee9eca3ae4f5c1a281482/products/1_jutoh-logo-1200x1600.jpg" border="0">Jutoh Plus -  Jutoh is an ebook creator for Epub, Kindle and more. It's fast, runs on Windows, Mac, and Linux, comes with a cover design editor, and allows book variations to be created with alternate text, style sheets and cover designs. Jutoh Plus adds scripting so you can automate ebook import and creation operations. It also allows customisation of ebook HTML via templates and source code documents; and you can create Windows CHM and wxWidgets HTB help files. </a>
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
<li><a href="https://vp-tips.techidaily.com/new-2024-approved-from-basic-to-advanced-your-guide-to-system-advancements/"><u>[New] 2024 Approved  From Basic to Advanced  Your Guide to System Advancements</u></a></li>
<li><a href="https://instagram-clips.techidaily.com/new-bridging-platforms-for-broad-sharing-instagram-and-facebook-for-2024/"><u>[New] Bridging Platforms for Broad Sharing  Instagram & Facebook for 2024</u></a></li>
<li><a href="https://facebook-clips.techidaily.com/new-in-2024-transforming-facebook-watchlists-implementing-autoplay-for-youtube-content/"><u>[New] In 2024, Transforming Facebook Watchlists  Implementing Autoplay for YouTube Content</u></a></li>
<li><a href="https://youtube-webster.techidaily.com/ed-2024-approved-becoming-a-pro-at-using-a-tripod-for-clear-high-quality-vlogs/"><u>[Updated] 2024 Approved  Becoming a Pro at Using a Tripod for Clear, High-Quality Vlogs</u></a></li>
<li><a href="https://youtube-webster.techidaily.com/ed-in-2024-budget-friendly-designs-for-youtube-content-creators/"><u>[Updated] In 2024, Budget-Friendly Designs for YouTube Content Creators</u></a></li>
<li><a href="https://article-tips.techidaily.com/2024-approved-free-movie-talent-release-declaration/"><u>2024 Approved  Free Movie Talent Release Declaration</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/abbyy-expands-asian-footprint-with-new-office-launch-in-hong-kong/"><u>ABBYY Expands Asian Footprint with New Office Launch in Hong Kong</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-investigators-unite-explore-4-online-whodunit-adventures/"><u>AI Investigators Unite: Explore 4 Online Whodunit Adventures</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-showdown-gpt-plus-versus-perplexity/"><u>AI Showdown: GPT Plus Versus Perplexity</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/bert-vs-gpt-a-deep-dive-into-modern-nlp-models/"><u>BERT V/S GPT: A Deep Dive Into Modern NLP Models</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/character-complexity-made-simple-by-chatgpts-nine-methods/"><u>Character Complexity Made Simple by ChatGPT’s Nine Methods</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-integration-for-seamless-smart-living-controls/"><u>ChatGPT Integration for Seamless Smart Living Controls</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-understanding-shared-links-and-their-functionality/"><u>ChatGPT: Understanding Shared Links & Their Functionality</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/claim-the-future-how-claude-redefines-data-insights-and-solutions/"><u>Claim the Future: How Claude Redefines Data Insights and Solutions</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/crafting-sites-easily-with-gpts-4-essential-aids/"><u>Crafting Sites Easily with GPT's 4 Essential Aids</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/demystifying-gemini-googles-latest-ai-research-venture/"><u>Demystifying Gemini: Google’s Latest AI Research Venture</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/elevate-interactive-exchanges-chatgpt-meets-mac/"><u>Elevate Interactive Exchanges: ChatGPT Meets Mac</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/enhanced-audience-engagement-through-intelligent-conversational-agents/"><u>Enhanced Audience Engagement Through Intelligent Conversational Agents</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/enhanced-user-experience-with-cookiebots-powerful-tracking-solutions/"><u>Enhanced User Experience with Cookiebot's Powerful Tracking Solutions</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/enhancing-marketing-pace-for-carlsberg-beers-quick-market-entry-tactics/"><u>Enhancing Marketing Pace for Carlsberg Beers - Quick Market Entry Tactics</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/enhancing-online-marketing-roi-through-advanced-cookiebot-ad-tech-tools/"><u>Enhancing Online Marketing ROI Through Advanced Cookiebot Ad Tech Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ensuring-the-legacy-of-classics-how-abbyy-brought-tolstoy-into-the-digital-age/"><u>Ensuring the Legacy of Classics: How ABBYY Brought Tolstoy Into the Digital Age</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/fostering-long-lasting-communication-with-gpt/"><u>Fostering Long-Lasting Communication with GPT</u></a></li>
<li><a href="https://techidaily.com/guide-successfully-navigating-the-windows-11-boot-settings-menu/"><u>Guide: Successfully Navigating the Windows 11 Boot Settings Menu</u></a></li>
<li><a href="https://location-social.techidaily.com/how-to-changeadd-location-filters-on-snapchat-for-your-samsung-galaxy-xcover-6-pro-tactical-edition-drfone-by-drfone-virtual-android/"><u>How to Change/Add Location Filters on Snapchat For your Samsung Galaxy XCover 6 Pro Tactical Edition | Dr.fone</u></a></li>
<li><a href="https://games-able.techidaily.com/how-to-play-the-nyc-connection-game-like-a-pro-8-steps/"><u>How to Play the NYC Connection Game Like a Pro (8 Steps)</u></a></li>
<li><a href="https://easy-unlock-android.techidaily.com/in-2024-how-to-unlock-oppo-reno-10-pro-5g-phone-pattern-lock-without-factory-reset-by-drfone-android/"><u>In 2024, How to Unlock Oppo Reno 10 Pro 5G Phone Pattern Lock without Factory Reset</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ios-users-check-this-out-chatgpt-app/"><u>IOS Users, Check This Out: ChatGPT App!</u></a></li>
<li><a href="https://extra-lessons.techidaily.com/laugh-loops-unlocked-zero-cost-humor-hub/"><u>Laugh Loops Unlocked  Zero-Cost Humor Hub</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/microsoft-redefines-search-ai-in-bing/"><u>Microsoft Redefines Search: AI in Bing</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/navigating-the-crowd-how-abbyy-stands-out-in-todays-loud-market/"><u>Navigating the Crowd: How ABBYY Stands Out in Today's Loud Market</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/no-more-lines-crossed-exit-chatgpts-reach/"><u>No More Lines Crossed? Exit ChatGPT's Reach</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/openai-denies-decline-in-chatgpts-intelligence/"><u>OpenAI Denies Decline in ChatGPT's Intelligence</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/optimized-with-advanced-traffic-analysis-via-ai-driven-cookie-tracking/"><u>Optimized with Advanced Traffic Analysis via AI-Driven Cookie Tracking</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revolutionary-dialogue-engine-anticipated-traits-of-gpt-5/"><u>Revolutionary Dialogue Engine: Anticipated Traits of GPT-5</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revolutionize-your-site-advanced-analytics-and-personalization-using-the-cookiebot-engine/"><u>Revolutionize Your Site: Advanced Analytics & Personalization Using the Cookiebot Engine</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/skepticism-in-self-care-questioning-ai-guidance/"><u>Skepticism in Self-Care: Questioning AI Guidance</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/surfez-sur-la-vague-de-changement-limpact-accelerateur-des-crises-sur-les-relations-bancaires/"><u>Surfez Sur La Vague De Changement - L'Impact Accélérateur Des Crises Sur Les Relations Bancaires</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/tackling-peak-limit-problem-with-chatgpt-win/"><u>Tackling Peak Limit Problem with ChatGPT (Win)</u></a></li>
<li><a href="https://win-solutions.techidaily.com/the-definitive-guide-to-dominating-roller-champions-crossplay-strategies-for-the-modern-gamer/"><u>The Definitive Guide to Dominating Roller Champions: Crossplay Strategies for the Modern Gamer</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-future-of-business-8-key-ways-to-harness-chatgpt/"><u>The Future of Business: 8 Key Ways to Harness ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-human-element-in-comprehensive-document-synopses/"><u>The Human Element in Comprehensive Document Synopses</u></a></li>
<li><a href="https://vimeo-videos.techidaily.com/the-ultimate-checklist-for-movie-maker-videos-on-vimeo-for-2024/"><u>The Ultimate Checklist for Movie Maker Videos on Vimeo for 2024</u></a></li>
<li><a href="https://facebook-video-share.techidaily.com/unleashing-brand-potential-with-free-youtube-marketing-templates-for-2024/"><u>Unleashing Brand Potential with FREE YouTube Marketing Templates for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unpacking-gpt-models-from-one-to-four/"><u>Unpacking GPT Models From One to Four</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-the-power-of-conversational-computing-rtx-bot/"><u>Unveiling the Power of Conversational Computing: RTX Bot</u></a></li>
<li><a href="https://ai-voice-clone.techidaily.com/updated-in-2024-google-translate-video-a-complete-guide-to-translate-video-with-google/"><u>Updated In 2024, Google Translate Video A Complete Guide To Translate Video With Google</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/what-is-llama-2-and-how-can-you-use-it/"><u>What Is Llama 2 and How Can You Use It?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/winchatgpt-hoax-exposed-the-facts-unfolded/"><u>WinChatGPT Hoax Exposed - The Facts Unfolded</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/world-leaders-in-tech-discussing-tomorrows-intelligence-systems/"><u>World Leaders in Tech Discussing Tomorrow's Intelligence Systems</u></a></li>
</ul></div>
