---
title: Uniting ChatGPT with WhatsApp for Top-Tier Support
date: 2024-08-25T17:38:29.836Z
updated: 2024-08-26T17:38:29.836Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Uniting ChatGPT with WhatsApp for Top-Tier Support
excerpt: This Article Describes Uniting ChatGPT with WhatsApp for Top-Tier Support
thumbnail: https://thmb.techidaily.com/f4ca93c2e74735632031e3a4405d77d7b0983d4143ac728b22e36df439e2bb35.jpg
---

## Uniting ChatGPT with WhatsApp for Top-Tier Support

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
<a href="https://vapordna.pxf.io/c/5597632/1496243/17238" target="_top" id="1496243"><img src="//a.impactradius-go.com/display-ad/17238-1496243" border="0" alt="" width="1000" height="1221"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1496243/17238" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://appsumo.8odi.net/c/5597632/2075461/7443" target="_top" id="2075461"><img src="//a.impactradius-go.com/display-ad/7443-2075461" border="0" alt="" width="1200" height="600"/></a><img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2075461/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 Move to your WhatsApp mobile app and navigate to **Settings > QR code > Scan code** to add a new linked device and scan the popped QR code on your terminal.

 After logging in, the application will start listening to incoming messages. If someone sends a message, the received message will make a GET request to API with the message as a query parameter and send the response back to the sender on WhatsApp.

 Expected output:

![Output of integrating chatgpt and WhatsApp](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/integrating-whatsapp-and-chatgpt-api-output.jpg)

## Using WhatsApp Chatbot to Integrate WhatsApp With ChatGPT API

 Another way to integrate ChatGPT into WhatsApp messages is by using a WhatsApp chatbot.

 Once you register your WhatsApp Business API, use a chat builder like OpenDialog to create a flow for the chat. You will then test your chatbot and add it to your mobile phone.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=37100474&QTY=1&AFFILIATE=108875&CART=1"><img src="https://awario.com/images/pages/index/img-platform-ui-1280@1x.avif" border="0"></a>
<!-- affiliate ads end -->
### Integrate OpenAI API With Your WhatsApp Chatbot

 To integrate your WhatsApp chatbot with OpenAI models, use the API key from OpenAI.

 Integrating WhatsApp chatbots with OpenAI GPT models presents a risk of WhatsApp blocking your account on security claims.

 Though this method is easier if you already have a chatbot, you should only opt for it once you’re comfortable with the risks involved.

### Configuring Automated Responses

 To get better customer service, configure automated responses to provide fast and accurate responses to customer messages. These responses will personalize the customer by name and provide relevant responses to customer queries.

<!-- affiliate ads begin -->
<a href="https://estore.zonealarm.com/order/checkout.php?PRODS=36245101&QTY=1&AFFILIATE=108875&CART=1"><img src="https://sc1.checkpoint.com/sc1/za/images/boxes/zang_box_trust.png" border="0">ZoneAlarm Extreme Security NextGen</a>
<!-- affiliate ads end -->
### Testing Your WhatsApp Chatbot

 Like all AI API systems, testing is key before you deploy your WhatsApp chatbot. This is to ensure that it works as expected. API testing tools like Postman and Curl can help to test your chatbot’s responses.

 In this case, the Django REST framework provides a browsable API to help test API requests and responses.

<!-- affiliate ads begin -->
<a href="https://shop.manycam.com/order/checkout.php?PRODS=17728032&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/8230bea7d54bcdf99cdfe85cb07313d5/mcaffbanner920x120.png" border="0"></a>
<!-- affiliate ads end -->
### Measuring Success and Fine-Tuning

 Once your WhatsApp chatbot is in deployment, it is crucial to measure its success and usage over time. This will help with fine-tuning it accordingly. Analytics tools like OpenDialog and Rasa can help to track metrics such as response time, retention rate, and customer satisfaction.

<!-- affiliate ads begin -->
<span id="1993650">
					<video width="720" height="300" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1993650.jpeg"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/22993-1993650">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1993650.jpeg" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:720px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Fhomestyler.sjv.io%2Fc%2F5597632%2F1993650%2F22993'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1993650/22993" style="position:absolute;visibility:hidden;" border="0" />
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
<li><a href="https://video-capture.techidaily.com/new-2024-approved-frame-rate-dilemma-30-vs-60-fps-in-video-production/"><u>[New] 2024 Approved  Frame Rate Dilemma  30 Vs. 60 FPS in Video Production</u></a></li>
<li><a href="https://facebook-video-recording.techidaily.com/new-2024-approved-mastering-facebook-vids-the-top-20-marketing-hacks/"><u>[New] 2024 Approved  Mastering Facebook Vids  The Top 20 Marketing Hacks</u></a></li>
<li><a href="https://instagram-clips.techidaily.com/new-highlight-heroes-iosandroid-covers-that-shine-bright/"><u>[New] Highlight Heroes  IOS/Android Covers That Shine Bright</u></a></li>
<li><a href="https://some-techniques.techidaily.com/new-how-to-use-preview-app-on-mac/"><u>[New] How to Use Preview App on Mac</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/new-innovative-online-tools-ranked-best-10-free-image-converters/"><u>[New] Innovative Online Tools Ranked  Best 10 Free Image Converters</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/new-odins-vengeance-realm-awakens-for-2024/"><u>[New] Odin’s Vengeance  Realm Awakens for 2024</u></a></li>
<li><a href="https://on-screen-recording.techidaily.com/updated-2024-approved-from-basic-recording-to-masterpiece-your-webcam-guide/"><u>[Updated] 2024 Approved  From Basic Recording to Masterpiece  Your WebCam Guide</u></a></li>
<li><a href="https://snapchat-videos.techidaily.com/updated-easy-steps-to-record-your-snapchat-screen-for-2024/"><u>[Updated] Easy Steps to Record Your Snapchat Screen for 2024</u></a></li>
<li><a href="https://youtube-data.techidaily.com/ed-from-raw-footage-to-highlight-hits-for-2024/"><u>[Updated] From Raw Footage to Highlight Hits for 2024</u></a></li>
<li><a href="https://video-capture.techidaily.com/updated-in-2024-professional-academic-recording-a-trio-of-methods-for-students-with-apple-devices/"><u>[Updated] In 2024, Professional Academic Recording  A Trio of Methods for Students with Apple Devices</u></a></li>
<li><a href="https://screen-mirroring-recording.techidaily.com/updated-in-2024-simplifying-tasks-with-ez-grabber-techniques/"><u>[Updated] In 2024, Simplifying Tasks with EZ Grabber Techniques</u></a></li>
<li><a href="https://fox-hovers.techidaily.com/2024-approved-how-to-fix-no-video-on-sony-a6400-camera/"><u>2024 Approved  How to Fix No Video On Sony A6400 Camera</u></a></li>
<li><a href="https://youtube-stream.techidaily.com/2024-approved-the-ultimate-hash-playbook-for-video-gamers-on-youtube/"><u>2024 Approved  The Ultimate Hash Playbook for Video Gamers on YouTube</u></a></li>
<li><a href="https://location-fake.techidaily.com/5-easy-ways-to-change-location-on-youtube-tv-on-vivo-s17t-drfone-by-drfone-virtual-android/"><u>5 Easy Ways to Change Location on YouTube TV On Vivo S17t | Dr.fone</u></a></li>
<li><a href="https://extra-information.techidaily.com/a-compreranium-of-hand-tracking-systems-for-2024/"><u>A Compreranium of Hand Tracking Systems for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-boost-for-hr-routine-challenges/"><u>AI Boost for HR Routine Challenges</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-driven-fake-news-a-potential-risk/"><u>AI-Driven Fake News: A Potential Risk?</u></a></li>
<li><a href="https://phone-solutions.techidaily.com/all-about-factory-reset-what-is-it-and-what-it-does-to-your-oppo-k11-5g-drfone-by-drfone-reset-android-reset-android/"><u>All About Factory Reset, What Is It and What It Does to Your Oppo K11 5G? | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/artificial-intelligence-lexicon-breaking-down-complex-words/"><u>Artificial Intelligence Lexicon: Breaking Down Complex Words</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/assessing-the-risk-of-employer-sanctions-for-using-chatgpt-tools/"><u>Assessing the Risk of Employer Sanctions for Using ChatGPT Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/bots-banter-beyond-boundaries-will-it-make-us-merry/"><u>Bot's Banter Beyond Boundaries: Will It Make Us Merry?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/cha-ching-better-ai-talks-10-customizations-for-chatgpts-growth/"><u>Cha-Ching Better AI Talks: 10 Customizations for ChatGPT's Growth</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/crafting-smart-workflows-with-ai-communication-tools/"><u>Crafting Smart Workflows with AI Communication Tools</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/cybersecurity-exposed-a-call-to-action/"><u>Cybersecurity Exposed: A Call to Action</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/deactivate-chatgpts-record-functionality-for-secure-talks/"><u>Deactivate ChatGPT’s Record Functionality for Secure Talks</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/demystifying-claude-3-and-its-potential/"><u>Demystifying Claude 3 and Its Potential</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/dissecting-machine-might-strong-vs-weak-ai/"><u>Dissecting Machine Might: Strong Vs. Weak AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/explore-the-finest-ai-powered-note-taking-software/"><u>Explore the Finest AI-Powered Note-Taking Software</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/fixing-communication-breakdown-with-chatgpts-plugin-services/"><u>Fixing Communication Breakdown with ChatGPT's Plugin Services</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/from-online-to-offline-installed-llama-2-basics/"><u>From Online to Offline: Installed Llama 2 Basics</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/gpt-tech-for-developing-habitual-inner-peace-practices/"><u>GPT-Tech for Developing Habitual Inner Peace Practices</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/grasping-the-operation-and-mechanism-of-predictive-ai/"><u>Grasping the Operation and Mechanism of Predictive AI</u></a></li>
<li><a href="https://blog-min.techidaily.com/how-to-play-hevc-h-265-video-on-samsung-galaxy-a54-5g-by-aiseesoft-video-converter-play-hevc-video-on-android/"><u>How to play HEVC H.265 video on Samsung Galaxy A54 5G?</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/in-2024-detailed-guide-of-ispoofer-for-pogo-installation-on-lava-blaze-curve-5g-drfone-by-drfone-virtual-android/"><u>In 2024, Detailed guide of ispoofer for pogo installation On Lava Blaze Curve 5G | Dr.fone</u></a></li>
<li><a href="https://iphone-unlock.techidaily.com/in-2024-how-can-i-unlock-my-iphone-x-after-forgetting-my-pin-code-drfone-by-drfone-ios/"><u>In 2024, How Can I Unlock My iPhone X After Forgetting my PIN Code? | Dr.fone</u></a></li>
<li><a href="https://unlock-android.techidaily.com/in-2024-how-to-reset-a-infinix-note-30i-phone-that-is-locked-by-drfone-android/"><u>In 2024, How to Reset a Infinix Note 30i Phone that is Locked?</u></a></li>
<li><a href="https://android-unlock.techidaily.com/in-2024-how-to-unlock-a-network-locked-oppo-f25-pro-5g-phone-by-drfone-android/"><u>In 2024, How to Unlock a Network Locked Oppo F25 Pro 5G Phone?</u></a></li>
<li><a href="https://instagram-video-files.techidaily.com/in-2024-instagram-videos-how-long-can-they-be/"><u>In 2024, Instagram Videos - How Long Can They Be?</u></a></li>
<li><a href="https://activate-lock.techidaily.com/in-2024-the-ultimate-guide-to-unlocking-apple-watch-or-apple-iphone-6-plus-from-icloud-by-drfone-ios/"><u>In 2024, The Ultimate Guide to Unlocking Apple Watch Or Apple iPhone 6 Plus from iCloud</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/intuitive-bavarder-installation-on-linux-distros/"><u>Intuitive Bavarder Installation on Linux Distros</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/language-architecture-showdown-deciphering-gpt-and-bert-mechanics/"><u>Language Architecture Showdown: Deciphering GPT and BERT Mechanics</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-poetry-through-chatgpt-explorations/"><u>Mastering Poetry Through ChatGPT Explorations</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/microsoft-infuses-bing-with-advanced-ai/"><u>Microsoft Infuses Bing With Advanced AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/plot-and-pixel-combining-chatgpt-with-game-script-development/"><u>Plot and Pixel: Combining ChatGPT with Game Script Development</u></a></li>
<li><a href="https://extra-skills.techidaily.com/prime-frame-rate-enhancing-laggard-motion-for-2024/"><u>Prime Frame Rate Enhancing Laggard Motion for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/propel-your-mobile-search-the-impactful-usage-of-ai-in-bing-app/"><u>Propel Your Mobile Search: The Impactful Usage of AI in Bing App</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revolutionize-ai-talks-in-chrome-here-are-7-tips/"><u>Revolutionize AI Talks in Chrome, Here Are 7 Tips</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revolutionizing-development-with-ai/"><u>Revolutionizing Development with AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/terminal-talk-command-line-tools-to-engage-chatgpt/"><u>Terminal Talk: Command Line Tools to Engage ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/top-6-ai-enhanced-note-apps-for-optimal-information-capture/"><u>Top 6 AI-Enhanced Note Apps for Optimal Information Capture</u></a></li>
<li><a href="https://techtrends.techidaily.com/troubleshooting-steps-getting-tiktok-up-and-running-again/"><u>Troubleshooting Steps: Getting TikTok Up and Running Again</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unlocking-chatgpt-overcoming-login-problems/"><u>Unlocking ChatGPT: Overcoming Login Problems</u></a></li>
<li><a href="https://android-pokemon-go.techidaily.com/what-pokemon-evolve-with-a-dawn-stone-for-oppo-find-x7-drfone-by-drfone-virtual-android/"><u>What Pokémon Evolve with A Dawn Stone For Oppo Find X7? | Dr.fone</u></a></li>
<li><a href="https://win11.techidaily.com/windows-graphics-scheduler-control-explained/"><u>Windows Graphics Scheduler Control Explained</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/your-path-to-advanced-interactions-with-new-chatgpt-extensions/"><u>Your Path to Advanced Interactions with New ChatGPT Extensions</u></a></li>
</ul></div>
