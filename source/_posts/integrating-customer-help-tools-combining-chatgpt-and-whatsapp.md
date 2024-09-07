---
title: "Integrating Customer Help Tools: Combining ChatGPT & WhatsApp"
date: 2024-09-06T23:30:16.244Z
updated: 2024-09-07T23:30:16.244Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Integrating Customer Help Tools: Combining ChatGPT & WhatsApp"
excerpt: "This Article Describes Integrating Customer Help Tools: Combining ChatGPT & WhatsApp"
thumbnail: https://thmb.techidaily.com/9f1310fb04eb76846ce94c2831da468762b7226e2e1efaca7ef8fd8dc861a7cc.jpg
---

## Integrating Customer Help Tools: Combining ChatGPT & WhatsApp

 Today’s businesses embrace messaging apps like WhatsApp to communicate with customers. This results in a surge in the automation of business customer interactions using chatbots.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 Such a chatbot is ChatGPT, a large language model by OpenAI that you can integrate with WhatsApp to automate customer interactions by providing fast and accurate responses to customer queries.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2135364/19272" target="_top" id="2135364">
  <img src="//a.impactradius-go.com/display-ad/19272-2135364" border="0" alt="https://techidaily.com" width="120" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135364/19272" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://aligracehair.sjv.io/c/5597632/2135397/19272" target="_top" id="2135397">
  <img src="//a.impactradius-go.com/display-ad/19272-2135397" border="0" alt="https://techidaily.com" width="180" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135397/19272" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://ephamedtechinc.pxf.io/c/5597632/2137229/26400" target="_top" id="2137229">
  <img src="//a.impactradius-go.com/display-ad/26400-2137229" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://ephamedtechinc.pxf.io/i/5597632/2137229/26400" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
<!-- affiliate ads begin -->
<span id="1424529">
					<video width="864" height="1536" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1424529.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/16446-1424529">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1424529.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:540px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Flaganoo.pxf.io%2Fc%2F5597632%2F1424529%2F16446'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1424529/16446" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Using WhatsApp Chatbot to Integrate WhatsApp With ChatGPT API

 Another way to integrate ChatGPT into WhatsApp messages is by using a WhatsApp chatbot.

 Once you register your WhatsApp Business API, use a chat builder like OpenDialog to create a flow for the chat. You will then test your chatbot and add it to your mobile phone.

### Integrate OpenAI API With Your WhatsApp Chatbot

 To integrate your WhatsApp chatbot with OpenAI models, use the API key from OpenAI.

 Integrating WhatsApp chatbots with OpenAI GPT models presents a risk of WhatsApp blocking your account on security claims.

 Though this method is easier if you already have a chatbot, you should only opt for it once you’re comfortable with the risks involved.

<!-- affiliate ads begin -->
<a href="https://bluettius.sjv.io/c/5597632/2139115/17108" target="_top" id="2139115">
  <img src="//a.impactradius-go.com/display-ad/17108-2139115" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://bluettius.sjv.io/i/5597632/2139115/17108" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
### Configuring Automated Responses

 To get better customer service, configure automated responses to provide fast and accurate responses to customer messages. These responses will personalize the customer by name and provide relevant responses to customer queries.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2118319/7443" target="_top" id="2118319">
  <img src="//a.impactradius-go.com/display-ad/7443-2118319" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2118319/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
### Testing Your WhatsApp Chatbot

 Like all AI API systems, testing is key before you deploy your WhatsApp chatbot. This is to ensure that it works as expected. API testing tools like Postman and Curl can help to test your chatbot’s responses.

 In this case, the Django REST framework provides a browsable API to help test API requests and responses.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2118323/7443" target="_top" id="2118323">
  <img src="//a.impactradius-go.com/display-ad/7443-2118323" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2118323/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
### Measuring Success and Fine-Tuning

 Once your WhatsApp chatbot is in deployment, it is crucial to measure its success and usage over time. This will help with fine-tuning it accordingly. Analytics tools like OpenDialog and Rasa can help to track metrics such as response time, retention rate, and customer satisfaction.

<!-- affiliate ads begin -->
<span id="1982596">
					<video width="576" height="240" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1982596.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/22993-1982596">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1982596.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:360px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fhomestyler.sjv.io%2Fc%2F5597632%2F1982596%2F22993'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1982596/22993" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://youtube-sure.techidaily.com/electing-gear-for-youtube-a-filmmakers-essentials-for-2024/"><u>[New] Selecting Gear for YouTube  A Filmmaker's Essentials for 2024</u></a></li>
<li><a href="https://remote-screen-capture.techidaily.com/new-streamline-your-slide-share-experience-with-webcam/"><u>[New] Streamline Your Slide Share Experience with Webcam</u></a></li>
<li><a href="https://facebook-video-share.techidaily.com/new-youtube-comment-management-turn-it-on-or-off/"><u>[New] YouTube Comment Management  Turn It On or Off</u></a></li>
<li><a href="https://on-screen-recording.techidaily.com/2024-approved-revamping-video-meeting-banners-for-teammates/"><u>2024 Approved  Revamping Video Meeting Banners for Teammates</u></a></li>
<li><a href="https://fox-boxes.techidaily.com/2024-approved-typographic-tactics-for-advanced-ae-users/"><u>2024 Approved  Typographic Tactics for Advanced AE Users</u></a></li>
<li><a href="https://article-knowledge.techidaily.com/adventure-essentials-top-10-gopro-protectors-reviewed/"><u>Adventure Essentials - Top 10 GoPro Protectors Reviewed</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-breakthroughs-essential-updates-in-the-latest-chatgpt-version/"><u>AI Breakthroughs: Essential Updates in the Latest ChatGPT Version</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/assessing-ai-risks-chatgpt-and-malware-development/"><u>Assessing AI Risks: ChatGPT and Malware Development</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/breeze-into-adventures-compiling-top-7-free-chatgpt-itinerary-apps/"><u>Breeze Into Adventures: Compiling Top 7 Free ChatGPT Itinerary Apps</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/businesses-dilemnas-five-arguments-for-keeping-ai-out/"><u>Businesses' Dilemnas: Five Arguments for Keeping AI Out</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatbots-explained-the-tech-thats-shaping-interactive-futures/"><u>Chatbots Explained: The Tech That's Shaping Interactive Futures</u></a></li>
<li><a href="https://games-able.techidaily.com/emulate-android-games-in-linux-system/"><u>Emulate Android Games in Linux System</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/enhance-output-speed-the-ultimate-list-of-ai-pdf-tools/"><u>Enhance Output Speed: The Ultimate List of AI PDF Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/expert-tips-genuine-gpt-practices/"><u>Expert Tips: Genuine GPT Practices</u></a></li>
<li><a href="https://facebook-video-content.techidaily.com/expert-video-extractor-fb-and-firefox-enhanced-experience-for-2024/"><u>Expert Video Extractor  FB & Firefox Enhanced Experience for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/five-key-considerations-every-buyer-should-evaluate-before-acquiring-a-fitness-device/"><u>Five Key Considerations Every Buyer Should Evaluate Before Acquiring a Fitness Device</u></a></li>
<li><a href="https://fake-location.techidaily.com/in-2024-4-methods-to-turn-off-life-360-on-motorola-moto-g14-without-anyone-knowing-drfone-by-drfone-virtual-android/"><u>In 2024, 4 Methods to Turn off Life 360 On Motorola Moto G14 without Anyone Knowing | Dr.fone</u></a></li>
<li><a href="https://change-location.techidaily.com/in-2024-which-pokemon-can-evolve-with-a-moon-stone-for-samsung-galaxy-m34-drfone-by-drfone-virtual-android/"><u>In 2024, Which Pokémon can Evolve with a Moon Stone For Samsung Galaxy M34? | Dr.fone</u></a></li>
<li><a href="https://youtube-lab.techidaily.com/ing-your-youtube-comments-desktop-and-mobile-guide-for-2024/"><u>Locating Your YouTube Comments  Desktop & Mobile Guide for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/navigating-chatgpts-stream-errors-successfully/"><u>Navigating ChatGPT's Stream Errors Successfully</u></a></li>
<li><a href="https://ai-driven-video-production.techidaily.com/new-bring-your-ideas-to-life-the-top-8-animation-software-for-mac-and-windows/"><u>New Bring Your Ideas to Life The Top 8 Animation Software for Mac and Windows</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/optimizing-ai-dialogue-the-ultimate-list-of-techniques/"><u>Optimizing AI Dialogue: The Ultimate List of Techniques</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/questioning-the-reliability-of-zerogpt-and-similar-tech-tools/"><u>Questioning the Reliability of ZeroGPT & Similar Tech Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/quick-journey-queries-answered-by-ai-best-7-free-planning-tools/"><u>Quick Journey Queries Answered by AI: Best 7 Free Planning Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revolutionizing-ai-dialogue-key-traits-for-next-gen-gpt-5/"><u>Revolutionizing AI Dialogue: Key Traits for Next-Gen GPT-5</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/running-freechat-on-win-a-freedomgpt-guide/"><u>Running FreeChat on Win: A FreedomGPT Guide</u></a></li>
<li><a href="https://extra-information.techidaily.com/seeking-the-perfect-samsung-gear-360-replacement-our-list-of-2023s-best-cameras/"><u>Seeking the Perfect Samsung Gear 360 Replacement  Our List of 2023'S Best Cameras</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/streamline-your-workflow-setting-up-gpt-on-ubuntu/"><u>Streamline Your Workflow: Setting up GPT on Ubuntu</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/swift-communication-with-bing-ai-chat-on-your-android-keyboard/"><u>Swift Communication with Bing AI Chat on Your Android Keyboard</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/talking-ai-futures-when-will-gpt-5-be-unveiled/"><u>Talking AI Futures: When Will GPT-5 Be Unveiled?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-art-of-trimming-excess-filtering-out-superfluous-gpt-plugins/"><u>The Art of Trimming Excess: Filtering Out Superfluous GPT Plugins</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-best-way-to-get-more-out-of-gpt-4-turbo-copilot/"><u>The Best Way to Get More Out of GPT-4 Turbo: Copilot</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-conundrum-of-tech-empathy-can-ai-mirror-our-feelings/"><u>The Conundrum of Tech Empathy: Can AI Mirror Our Feelings?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unanswerable-inquiries-in-language-models/"><u>Unanswerable Inquiries in Language Models</u></a></li>
<li><a href="https://techidaily.com/update-usb-drivers-in-windows-11-7-8-and-81-easily/"><u>Update USB Drivers in Windows 11, 7, 8 & 8.1. Easily</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/why-personal-therapy-shouldnt-be-a-computer-game/"><u>Why Personal Therapy Shouldn't Be a Computer Game</u></a></li>
</ul></div>
