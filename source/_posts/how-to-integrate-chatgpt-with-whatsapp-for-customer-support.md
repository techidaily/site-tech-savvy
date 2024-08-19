---
title: How to Integrate ChatGPT With WhatsApp for Customer Support
date: 2024-08-18T09:56:03.156Z
updated: 2024-08-19T09:56:03.156Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes How to Integrate ChatGPT With WhatsApp for Customer Support
excerpt: This Article Describes How to Integrate ChatGPT With WhatsApp for Customer Support
thumbnail: https://thmb.techidaily.com/d0b73eb28e24a2f2ed6215d7e2c211efc75eaeb77baea06879d148a0fe930510.jpg
---

## How to Integrate ChatGPT With WhatsApp for Customer Support

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
<a href="https://shop.mondly.com/affiliate.php?ACCOUNT=ATISTUDI&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.mondly.com%3FAFFILIATE%3D108875%26RESOURCE%3D%2BGeneral%2B970x90%2B"><img src="https://secure.avangate.com/images/merchant/69c418c33ec2e1a4267fa9bb77fa1428/general-970x90.gif" border="0"></a>
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
<a href="https://store.nero.com/order/checkout.php?PRODS=42296985&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/9cea886b9f44a3c2df1163730ab64994/products/copy_nero_burning_rom_cart.png" border="0">
</a>
<!-- affiliate ads end -->
 Move to your WhatsApp mobile app and navigate to **Settings > QR code > Scan code** to add a new linked device and scan the popped QR code on your terminal.

 After logging in, the application will start listening to incoming messages. If someone sends a message, the received message will make a GET request to API with the message as a query parameter and send the response back to the sender on WhatsApp.

 Expected output:

![Output of integrating chatgpt and WhatsApp](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/integrating-whatsapp-and-chatgpt-api-output.jpg)

<!-- affiliate ads begin -->
<a href="https://estore.zonealarm.com/order/checkout.php?PRODS=36245101&QTY=1&AFFILIATE=108875&CART=1"><img src="https://sc1.checkpoint.com/sc1/za/images/boxes/zang_box_trust.png" border="0">ZoneAlarm Extreme Security NextGen</a>
<!-- affiliate ads end -->
## Using WhatsApp Chatbot to Integrate WhatsApp With ChatGPT API

 Another way to integrate ChatGPT into WhatsApp messages is by using a WhatsApp chatbot.

 Once you register your WhatsApp Business API, use a chat builder like OpenDialog to create a flow for the chat. You will then test your chatbot and add it to your mobile phone.

### Integrate OpenAI API With Your WhatsApp Chatbot

 To integrate your WhatsApp chatbot with OpenAI models, use the API key from OpenAI.

 Integrating WhatsApp chatbots with OpenAI GPT models presents a risk of WhatsApp blocking your account on security claims.

 Though this method is easier if you already have a chatbot, you should only opt for it once you’re comfortable with the risks involved.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4742929&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/e09fdffe648a30658a9657bbed7b2388/products/boxshot(2).png" border="0">Kanto Player Professional</a>
<!-- affiliate ads end -->
### Configuring Automated Responses

 To get better customer service, configure automated responses to provide fast and accurate responses to customer messages. These responses will personalize the customer by name and provide relevant responses to customer queries.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4728277&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/f7f07e7dab09533bc71247a5b29a7373/products/1_iDeviceMessageBox.png" border="0"></a>
<!-- affiliate ads end -->
### Testing Your WhatsApp Chatbot

 Like all AI API systems, testing is key before you deploy your WhatsApp chatbot. This is to ensure that it works as expected. API testing tools like Postman and Curl can help to test your chatbot’s responses.

 In this case, the Django REST framework provides a browsable API to help test API requests and responses.

### Measuring Success and Fine-Tuning

 Once your WhatsApp chatbot is in deployment, it is crucial to measure its success and usage over time. This will help with fine-tuning it accordingly. Analytics tools like OpenDialog and Rasa can help to track metrics such as response time, retention rate, and customer satisfaction.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=32667153&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.coolmuster.com/uploads/image/20201228/feature02.png" border="0"></a>
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
<li><a href="https://screen-activity-recording.techidaily.com/new-2024-approved-sweet-scene-capture-masterclass-in-freeze-dried-filmmaking/"><u>[New] 2024 Approved  Sweet Scene Capture  Masterclass in Freeze-Dried Filmmaking</u></a></li>
<li><a href="https://tiktok-video-recordings.techidaily.com/new-2024-approved-the-insider-guide-attending-live-tiktok-gigs/"><u>[New] 2024 Approved  The Insider Guide  Attending Live TikTok Gigs</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/new-boost-your-instagrams-accessibility-with-easy-caption-features/"><u>[New] Boost Your Instagram's Accessibility with Easy Caption Features</u></a></li>
<li><a href="https://eaxpv-info.techidaily.com/new-does-your-channel-benefit-from-regular-youtube-payments-in-2024/"><u>[New] Does Your Channel Benefit From Regular YouTube Payments, In 2024</u></a></li>
<li><a href="https://video-screen-grab.techidaily.com/new-in-2024-unlocking-the-secrets-of-successful-google-meet-engagement/"><u>[New] In 2024, Unlocking the Secrets of Successful Google Meet Engagement</u></a></li>
<li><a href="https://snapchat-videos.techidaily.com/new-straightforward-steps-installing-snapchat-on-mac-for-2024/"><u>[New] Straightforward Steps  Installing Snapchat on Mac for 2024</u></a></li>
<li><a href="https://youtube-lab.techidaily.com/t-loop-technique-for-the-digital-content-wanderer-for-2024/"><u>[New] YT Loop Technique for the Digital Content Wanderer for 2024</u></a></li>
<li><a href="https://facebook-video-footage.techidaily.com/updated-2024-approved-enhancing-video-success-top-8-yt-thumbnail-strategies/"><u>[Updated] 2024 Approved  Enhancing Video Success  Top 8 YT Thumbnail Strategies</u></a></li>
<li><a href="https://youtube-data.techidaily.com/ed-in-2024-best-livestream-capturing-solutions-for-content-makers/"><u>[Updated] In 2024, Best Livestream Capturing Solutions for Content Makers</u></a></li>
<li><a href="https://vp-tips.techidaily.com/updated-in-2024-innovative-practices-for-enhancing-vhs-photos-via-pcs/"><u>[Updated] In 2024, Innovative Practices for Enhancing VHS Photos via PCs</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/2024-approved-from-average-to-spectacular-mastering-dynamic-range-portraits/"><u>2024 Approved  From Average to Spectacular  Mastering Dynamic Range Portraits</u></a></li>
<li><a href="https://location-social.techidaily.com/4-feasible-ways-to-fake-location-on-facebook-for-your-apple-iphone-15-pro-max-drfone-by-drfone-virtual-ios/"><u>4 Feasible Ways to Fake Location on Facebook For your Apple iPhone 15 Pro Max | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-powered-strategies-for-achieving-desired-career/"><u>AI-Powered Strategies for Achieving Desired Career</u></a></li>
<li><a href="https://fake-location.techidaily.com/best-10-mock-location-apps-worth-trying-on-vivo-s18-pro-drfone-by-drfone-virtual-android/"><u>Best 10 Mock Location Apps Worth Trying On Vivo S18 Pro | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/brainpower-battlegrounds-gpt-and-google-bard-collide/"><u>Brainpower Battlegrounds: GPT & Google Bard Collide</u></a></li>
<li><a href="https://facebook-video-recording.techidaily.com/bridging-gaps-online-effective-techniques-for-screenshare-on-fb-for-2024/"><u>Bridging Gaps Online  Effective Techniques for Screenshare on FB for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatai-profits-and-pc-building-hacks-for-enthusiasts/"><u>ChatAI Profits & PC Building Hacks for Enthusiasts</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-evolved-discover-the-features-that-matter-most/"><u>ChatGPT Evolved: Discover the Features That Matter Most!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-an-emerging-seo-hurdle/"><u>ChatGPT: An Emerging SEO Hurdle?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpts-comedy-craft-does-ai-bring-laughter-to-life/"><u>ChatGPT's Comedy Craft: Does AI Bring Laughter to Life?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/cyber-survival-skills-predictive-trends-for-protection/"><u>Cyber Survival Skills: Predictive Trends for Protection</u></a></li>
<li><a href="https://ios-unlock.techidaily.com/how-to-access-your-iphone-15-pro-when-you-forget-the-passcode-by-drfone-ios/"><u>How to Access Your iPhone 15 Pro When You Forget the Passcode?</u></a></li>
<li><a href="https://location-social.techidaily.com/how-to-change-location-on-tiktok-to-see-more-content-on-your-samsung-galaxy-m34-5g-drfone-by-drfone-virtual-android/"><u>How to Change Location on TikTok to See More Content On your Samsung Galaxy M34 5G | Dr.fone</u></a></li>
<li><a href="https://android-unlock.techidaily.com/how-to-unlock-vivo-s17-pro-phone-without-any-data-loss-by-drfone-android/"><u>How to Unlock Vivo S17 Pro Phone without Any Data Loss</u></a></li>
<li><a href="https://unlock-android.techidaily.com/how-to-unlock-xiaomi-civi-3-pin-codepattern-lockpassword-by-drfone-android/"><u>How to Unlock Xiaomi Civi 3 PIN Code/Pattern Lock/Password</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-usechatgpts-co-pilot-expands-ai-capabilities-in-conversations/"><u>How UseChatGPT's Co-Pilot Expands AI Capabilities in Conversations</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/hugging-face-breakdown-meaning-and-uses/"><u>Hugging Face Breakdown: Meaning & Uses</u></a></li>
<li><a href="https://extra-approaches.techidaily.com/in-2024-mastering-memes-top-ten-template-showcase/"><u>In 2024, Mastering Memes  Top Ten Template Showcase</u></a></li>
<li><a href="https://youtube-stream.techidaily.com/in-2024-rapid-growth-techniques-for-youtube-views-via-collaborative-videos/"><u>In 2024, Rapid Growth Techniques for YouTube Views via Collaborative Videos</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/instant-gpt-worldwide-entry-via-chatgpt-everywhere/"><u>Instant GPT Worldwide Entry via ChatGPT Everywhere</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/interactive-innovation-will-claude-surpass-gpts-skills/"><u>Interactive Innovation: Will Claude Surpass GPT's Skills?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/labor-landscapes-altered-by-ais-advances/"><u>Labor Landscapes Altered by AI's Advances</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/leverage-ai-for-reading-pdfs-with-these-four-tactics/"><u>Leverage AI for Reading PDFs with These Four Tactics</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/master-methods-chronicling-your-ps3-gameplay-for-2024/"><u>Master Methods  Chronicling Your PS3 Gameplay for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-ai-art-gpt-powered-image-creation/"><u>Mastering AI Art: GPT-Powered Image Creation</u></a></li>
<li><a href="https://extra-information.techidaily.com/prime-soundstage-narratives-for-radio/"><u>Prime Soundstage Narratives for Radio</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/protecting-originality-openais-gpt-output-detector/"><u>Protecting Originality: OpenAI's GPT Output Detector</u></a></li>
<li><a href="https://review-topics.techidaily.com/put-and-play-mkv-movies-on-huawei-by-aiseesoft-video-converter-play-mkv-on-android/"><u>Put and play MKV movies on Huawei </u></a></li>
<li><a href="https://tech-savvy.techidaily.com/redefining-smarts-outsmarting-a-machine-oracle/"><u>Redefining Smarts: Outsmarting a Machine Oracle</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/regaining-full-access-to-chatgpt-post-blocking/"><u>Regaining Full Access to ChatGPT Post-Blocking</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revolutionizing-rides-mercedes-benz-infuses-cars-with-chatgpt/"><u>Revolutionizing Rides: Mercedes-Benz Infuses Cars with ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/secure-and-eternalize-a-chatgpt-storage-solution/"><u>Secure & Eternalize: A ChatGPT Storage Solution</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/should-we-demonstrate-decorum-with-chatgpt-siri-and-more/"><u>Should We Demonstrate Decorum with ChatGPT? Siri & More</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/sifting-through-codegpt-can-it-realistically-write-complex-code/"><u>Sifting Through CodeGPT: Can It Realistically Write Complex Code?</u></a></li>
<li><a href="https://sound-issues.techidaily.com/solve-your-windows-11-or-7-speaker-noise-problems-today/"><u>Solve Your Windows 11 or 7 Speaker Noise Problems Today</u></a></li>
<li><a href="https://screen-recording.techidaily.com/splitcam-probe-in-video-techs-top-spot/"><u>SplitCam Probe - In Video Tech's Top Spot?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-art-and-science-of-paperclip-optimization-in-ais-ecosystem/"><u>The Art and Science of Paperclip Optimization in AI's Ecosystem</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-forbidden-queries-for-ai-engagement/"><u>The Forbidden Queries for AI Engagement</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-unpredictable-consequences-of-unquestioned-ai/"><u>The Unpredictable Consequences of Unquestioned AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unleashing-potential-effective-chatgpt-use-on-macs/"><u>Unleashing Potential: Effective ChatGPT Use on Macs</u></a></li>
<li><a href="https://facebook.techidaily.com/unlock-advanced-account-protection-with-fb-mtgc/"><u>Unlock Advanced Account Protection with FB MTGC</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unmatched-efficiency-choosing-the-top-5-expert-ai-prompt-creators/"><u>Unmatched Efficiency: Choosing the Top 5 Expert AI Prompt Creators</u></a></li>
<li><a href="https://ios-pokemon-go.techidaily.com/ways-to-trade-pokemon-go-from-far-away-on-apple-iphone-11-pro-drfone-by-drfone-virtual-ios/"><u>Ways to trade pokemon go from far away On Apple iPhone 11 Pro? | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/write-winning-cover-letters-with-the-help-of-chatgpt/"><u>Write Winning Cover Letters with the Help of ChatGPT</u></a></li>
</ul></div>
