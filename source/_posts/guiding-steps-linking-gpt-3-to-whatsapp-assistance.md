---
title: "Guiding Steps: Linking GPT-3 to WhatsApp Assistance"
date: 2024-08-15T02:40:41.013Z
updated: 2024-08-16T02:40:41.013Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Guiding Steps: Linking GPT-3 to WhatsApp Assistance"
excerpt: "This Article Describes Guiding Steps: Linking GPT-3 to WhatsApp Assistance"
thumbnail: https://thmb.techidaily.com/2546a6e6db1c838a1a7b59103067ea8f9dccc09f3a86cd4ad8b0c7371cd0f3e3.jpg
---

## Guiding Steps: Linking GPT-3 to WhatsApp Assistance

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
<a href="https://store.nero.com/order/checkout.php?PRODS=4729507&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.nero.com/nero-com-wAssets/img/banners/2023/TIU/Nero_TuneItUp_Screen_2.webp" border="0">/a>
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
<!-- affiliate ads begin -->
<a href="https://aspironcom.sjv.io/c/5597632/1941789/21554" target="_top" id="1941789"><img src="//a.impactradius-go.com/display-ad/21554-1941789" border="0" alt="" width="650" height="800"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1941789/21554" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 Move to your WhatsApp mobile app and navigate to **Settings > QR code > Scan code** to add a new linked device and scan the popped QR code on your terminal.

 After logging in, the application will start listening to incoming messages. If someone sends a message, the received message will make a GET request to API with the message as a query parameter and send the response back to the sender on WhatsApp.

 Expected output:

![Output of integrating chatgpt and WhatsApp](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/integrating-whatsapp-and-chatgpt-api-output.jpg)

## Using WhatsApp Chatbot to Integrate WhatsApp With ChatGPT API

 Another way to integrate ChatGPT into WhatsApp messages is by using a WhatsApp chatbot.

 Once you register your WhatsApp Business API, use a chat builder like OpenDialog to create a flow for the chat. You will then test your chatbot and add it to your mobile phone.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4940317&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/333ac5d90817d69113471fbb6e531bee/sps-partnership-728x90eng.png" border="0"></a>
<!-- affiliate ads end -->
### Integrate OpenAI API With Your WhatsApp Chatbot

 To integrate your WhatsApp chatbot with OpenAI models, use the API key from OpenAI.

 Integrating WhatsApp chatbots with OpenAI GPT models presents a risk of WhatsApp blocking your account on security claims.

 Though this method is easier if you already have a chatbot, you should only opt for it once you’re comfortable with the risks involved.

<!-- affiliate ads begin -->
<a href="https://shop.systoolsgroup.com/affiliate.php?ACCOUNT=SYSTOOBY&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.systoolsgroup.com%3FAFFILIATE%3D108875%26RESOURCE%3D%2BSysTools%2BOutlook%2BRecovery"><img src="https://www.systoolsgroup.com/box/outlook-recovery.png" border="0"></a>
<!-- affiliate ads end -->
### Configuring Automated Responses

 To get better customer service, configure automated responses to provide fast and accurate responses to customer messages. These responses will personalize the customer by name and provide relevant responses to customer queries.

<!-- affiliate ads begin -->
<a href="https://funwhole.sjv.io/c/5597632/1702887/17189" target="_top" id="1702887"><img src="//a.impactradius-go.com/display-ad/17189-1702887" border="0" alt="" width="1000" height="1000"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1702887/17189" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
### Testing Your WhatsApp Chatbot

 Like all AI API systems, testing is key before you deploy your WhatsApp chatbot. This is to ensure that it works as expected. API testing tools like Postman and Curl can help to test your chatbot’s responses.

 In this case, the Django REST framework provides a browsable API to help test API requests and responses.

<!-- affiliate ads begin -->
<a href="https://store.movavi.com/affiliate.php?ACCOUNT=MOVAVI&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.movavi.com%3FAFFILIATE%3D108875%26RESOURCE%3DMovavi%2BVideo%2BEditor%2Bbox"><img src="https://mcusercontent.com/0885a03ded3d480dca9287f12/images/6d3207fd-9f15-4c21-f0ad-59c68e6a7e2a.png" border="0"></a>
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
<li><a href="https://facebook-record-videos.techidaily.com/new-2024-approved-comprehensive-guide-to-downloading-standardized-youtube-images/"><u>[New] 2024 Approved  Comprehensive Guide to Downloading Standardized YouTube Images</u></a></li>
<li><a href="https://extra-lessons.techidaily.com/new-ace-the-art-of-altering-and-amplifying-vhs-photos-on-computers/"><u>[New] Ace the Art of Altering and Amplifying VHS Photos on Computers</u></a></li>
<li><a href="https://extra-information.techidaily.com/new-appreciative-adjacencies-templates-for-any-spend-plan/"><u>[New] Appreciative Adjacencies  Templates for Any Spend Plan</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/new-direct-route-uploading-from-youtube-to-dailymotion-for-2024/"><u>[New] Direct Route  Uploading From YouTube to Dailymotion for 2024</u></a></li>
<li><a href="https://vp-tips.techidaily.com/new-in-2024-home-cinema-mastery-top-10-hd-players-list/"><u>[New] In 2024, Home Cinema Mastery  Top 10 HD Players' List</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/updated-2024-approved-the-rotation-riddle-decoding-the-secrets-of-video-swapping-on-social-media/"><u>[Updated] 2024 Approved  The Rotation Riddle  Decoding the Secrets of Video Swapping on Social Media</u></a></li>
<li><a href="https://twitter-videos.techidaily.com/updated-efficiently-tackling-twitter-archive-data-analysis/"><u>[Updated] Efficiently Tackling Twitter Archive Data Analysis</u></a></li>
<li><a href="https://screen-sharing-recording.techidaily.com/updated-in-2024-from-casual-gamer-to-pro-elevating-your-minecraft-recordings-with-a-mac/"><u>[Updated] In 2024, From Casual Gamer to Pro  Elevating Your Minecraft Recordings with a Mac</u></a></li>
<li><a href="https://instagram-video-files.techidaily.com/updated-mastering-identity-verification-a-deep-dive-into-ig-selfies/"><u>[Updated] Mastering Identity Verification  A Deep Dive Into IG Selfies</u></a></li>
<li><a href="https://buynow-info.techidaily.com/a-connoisseurs-choice-explore-the-best-websites-hosting-film-preview-clips/"><u>A Connoisseur's Choice: Explore the Best Websites Hosting Film Preview Clips</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/are-gpt-enhanced-jobs-the-next-big-income-boost/"><u>Are GPT-Enhanced Jobs the Next Big Income Boost?</u></a></li>
<li><a href="https://fox-glue.techidaily.com/become-an-expert-tutorial-for-making-gifs-into-desirable-whatsapp-and-telegram-stickers/"><u>Become an Expert  Tutorial for Making GIFs Into Desirable WhatsApp & Telegram Stickers</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/breaking-down-claude-2-features-unveiled/"><u>Breaking Down Claude 2: Features Unveiled</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/compare-and-conquer-why-ios-chatgpt-wins-over-web/"><u>Compare & Conquer: Why iOS ChatGPT Wins Over Web</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/content-enhancement-through-smart-ai-technology/"><u>Content Enhancement Through Smart AI Technology</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/diving-into-digital-dialogue-googles-groundbreayer-palm-2/"><u>Diving Into Digital Dialogue: Google's Groundbreayer, PaLM 2</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/does-ai-like-chatgpt-have-wordcharacter-count-boundaries/"><u>Does AI, Like ChatGPT, Have Word/Character Count Boundaries?</u></a></li>
<li><a href="https://windows11.techidaily.com/eliminating-error-0x80072efd-a-windows-store-solution/"><u>Eliminating Error 0X80072EFD: A Windows Store Solution</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/from-digital-dialogue-to-printed-poetry-collections/"><u>From Digital Dialogue to Printed Poetry Collections</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/gamifying-language-text-based-quests-via-chatgpt/"><u>Gamifying Language: Text-Based Quests via ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/googles-gemini-navigating-through-its-artificial-intelligence-landscape/"><u>Google’s Gemini: Navigating Through Its Artificial Intelligence Landscape</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-correct-chatgpt-live-dialogue-problems/"><u>How To Correct ChatGPT Live Dialogue Problems</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/in-2024-15-best-strongest-pokemon-to-use-in-pokemon-go-pvp-leagues-for-htc-u23-drfone-by-drfone-virtual-android/"><u>In 2024, 15 Best Strongest Pokémon To Use in Pokémon GO PvP Leagues For HTC U23 | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/innovative-excel-solutions-achieved-via-chatgpt-use-cases/"><u>Innovative Excel Solutions Achieved via ChatGPT Use Cases</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-chatgpt-plugin-integration/"><u>Mastering ChatGPT Plugin Integration</u></a></li>
<li><a href="https://tech-recovery.techidaily.com/mastering-the-art-of-protecting-emails-tips-for-achieving-safelisting-on-google/"><u>Mastering the Art of Protecting Emails: Tips for Achieving Safelisting on Google</u></a></li>
<li><a href="https://youtube-help.techidaily.com/mastering-youtube-revenue-a-complete-playbook-for-2024/"><u>Mastering Youtube Revenue   A Complete Playbook for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/musks-mystery-the-future-of-gpt-revealed/"><u>Musk's Mystery: The Future of GPT Revealed?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/navigating-chatgpt-for-kids-five-child-friendly-practices/"><u>Navigating ChatGPT for Kids: Five Child-Friendly Practices</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/new-era-of-conversation-chatgpt-on-ios/"><u>New Era of Conversation: ChatGPT on iOS</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/paramount-considerations-in-utilizing-artificial-intelligence-for-emotional-support-via-chatgpt/"><u>Paramount Considerations in Utilizing Artificial Intelligence for Emotional Support via ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/pathway-to-peak-performance-chatgpts-wellbe-point-of-view/"><u>Pathway to Peak Performance: ChatGPT's Wellbe Point of View</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/politeness-in-the-age-of-ai-engaging-with-gpt-alexa-and-more/"><u>Politeness in the Age of AI: Engaging with GPT, Alexa & More</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revolutionizing-creation-ten-advances-by-ai/"><u>Revolutionizing Creation: Ten Advances by AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revolutionizing-health-care-with-chatgpts-top-9-tactics/"><u>Revolutionizing Health Care with ChatGPT’s Top 9 Tactics</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/seek-these-six-no-cost-ai-options-similar-to-sora/"><u>Seek These Six No-Cost AI Options Similar to Sora</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/simplify-complexity-transformative-techniques-for-3d-printing-with-chatgpt/"><u>Simplify Complexity: Transformative Techniques for 3D Printing with ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/strategies-for-employing-chatgpt-in-study-papers/"><u>Strategies for Employing ChatGPT in Study Papers</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/strategies-for-exporting-data-from-your-ai-conversations/"><u>Strategies for Exporting Data From Your AI Conversations</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/streamlined-academic-success-through-gpt-assisted-notes/"><u>Streamlined Academic Success Through GPT-Assisted Notes</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/tailored-transformation-crafting-a-personalized-chatgpt/"><u>Tailored Transformation: Crafting a Personalized ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/tailoring-ai-communication-implementing-gpt-creation/"><u>Tailoring AI Communication: Implementing GPT Creation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-chat-comparison-coin-how-gpt-stacks-up-against-bingbot/"><u>The Chat Comparison Coin: How GPT Stacks Up Against BingBot</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-quest-for-excellence-between-gemini-max-and-enhanced-chatgpt/"><u>The Quest for Excellence: Between Gemini Max & Enhanced ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-truth-behind-grok-ai-insights-from-musk-on-its-purpose-and-price/"><u>The Truth Behind Grok AI - Insights From Musk on Its Purpose & Price</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-ultimate-list-of-ai-powered-chrome-extensions-for-better-task-management/"><u>The Ultimate List of AI-Powered Chrome Extensions for Better Task Management</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-unreliable-shield-of-artificative-intelligence/"><u>The Unreliable Shield of Artificative Intelligence</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/top-5-voice-commands-for-mastering-chatgpt/"><u>Top 5 Voice Commands for Mastering ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unraveling-chatgpt-premiums-worth/"><u>Unraveling ChatGPT Premium's Worth</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-the-shortcomings-of-ai-powered-message-bots/"><u>Unveiling the Shortcomings of AI-Powered Message Bots</u></a></li>
<li><a href="https://win-dash.techidaily.com/upgrade-your-sound-quality-today-free-downloads-of-audigy-fx-driver-software/"><u>Upgrade Your Sound Quality Today – Free Downloads of Audigy FX Driver Software</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/where-is-the-best-place-to-catch-dratini-on-oneplus-ace-3-drfone-by-drfone-virtual-android/"><u>Where Is the Best Place to Catch Dratini On OnePlus Ace 3 | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/why-distrust-in-artificial-intelligence-isnt-extreme/"><u>Why Distrust in Artificial Intelligence Isn't Extreme</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/why-not-rely-on-chatgpt-for-complete-text-synopses/"><u>Why Not Rely on ChatGPT for Complete Text Synopses?</u></a></li>
</ul></div>
