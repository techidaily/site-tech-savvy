---
title: "Enhancing Helpdesk Operations: GPT-3 & WhatsApp Alliance"
date: 2024-09-02T20:37:41.438Z
updated: 2024-09-03T20:37:41.438Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Enhancing Helpdesk Operations: GPT-3 & WhatsApp Alliance"
excerpt: "This Article Describes Enhancing Helpdesk Operations: GPT-3 & WhatsApp Alliance"
thumbnail: https://thmb.techidaily.com/d9de24816d3ddace39801c0414212d66853043d5f11ffbf1394765ef078e9e33.jpg
---

## Enhancing Helpdesk Operations: GPT-3 & WhatsApp Alliance

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
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4600114&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.epubor.com/images/drm-removal-feature2.png" border="0">Any DRM Removal for Mac： Remove DRM from Adobe, Kindle, Sony eReader, Kobo, etc, read your ebooks anywhere.</a>
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
<a href="https://checkout.devart.com/order/checkout.php?PRODS=5023555&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/45b430710ad04765a6afd58d9d9fafca/products/dotConnect_O.png" border="0">dotConnect for Oracle is an ADO.NET data provider for Oracle with Entity Framework Support.</a>
<!-- affiliate ads end -->
 Move to your WhatsApp mobile app and navigate to **Settings > QR code > Scan code** to add a new linked device and scan the popped QR code on your terminal.

 After logging in, the application will start listening to incoming messages. If someone sends a message, the received message will make a GET request to API with the message as a query parameter and send the response back to the sender on WhatsApp.

 Expected output:

![Output of integrating chatgpt and WhatsApp](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/integrating-whatsapp-and-chatgpt-api-output.jpg)

## Using WhatsApp Chatbot to Integrate WhatsApp With ChatGPT API

 Another way to integrate ChatGPT into WhatsApp messages is by using a WhatsApp chatbot.

 Once you register your WhatsApp Business API, use a chat builder like OpenDialog to create a flow for the chat. You will then test your chatbot and add it to your mobile phone.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=35038891&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.dupinout.com/wp-content/uploads/2021/12/DupInOut-New-Duplicate-Scan-Tab.png" border="0"></a>
<!-- affiliate ads end -->
### Integrate OpenAI API With Your WhatsApp Chatbot

 To integrate your WhatsApp chatbot with OpenAI models, use the API key from OpenAI.

 Integrating WhatsApp chatbots with OpenAI GPT models presents a risk of WhatsApp blocking your account on security claims.

 Though this method is easier if you already have a chatbot, you should only opt for it once you’re comfortable with the risks involved.

### Configuring Automated Responses

 To get better customer service, configure automated responses to provide fast and accurate responses to customer messages. These responses will personalize the customer by name and provide relevant responses to customer queries.

<!-- affiliate ads begin -->
<a href="https://store.revouninstaller.com/order/checkout.php?PRODS=28010250&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/4282ec8de8c9be897e7aff4aa231b1a4/336__280a.jpg" border="0"></a>
<!-- affiliate ads end -->
### Testing Your WhatsApp Chatbot

 Like all AI API systems, testing is key before you deploy your WhatsApp chatbot. This is to ensure that it works as expected. API testing tools like Postman and Curl can help to test your chatbot’s responses.

 In this case, the Django REST framework provides a browsable API to help test API requests and responses.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4726807&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/c14a8df1e1b4d5297e9cb30cb34d5a00/products/copy_copy_power-tools-48.png" border="0">Power Tools add-on for Google Sheets, Lifetime subscription</a>
<!-- affiliate ads end -->
### Measuring Success and Fine-Tuning

 Once your WhatsApp chatbot is in deployment, it is crucial to measure its success and usage over time. This will help with fine-tuning it accordingly. Analytics tools like OpenDialog and Rasa can help to track metrics such as response time, retention rate, and customer satisfaction.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4576829&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/9e740b84bb48a64dde25061566299467/products/copy_1_jp_box_big.png" border="0">Jet Profiler for MySQL, Enterprise Version： Jet Profiler for MySQL is real-time query performance and diagnostics tool for the MySQL database server. Its detailed query information, graphical interface and ease of use makes this a great tool for finding performance bottlenecks in your MySQL databases. </a>
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
<li><a href="https://facebook-video-share.techidaily.com/new-2024-approved-direct-to-device-converting-youtube-tracks-for-idevices/"><u>[New] 2024 Approved  Direct to Device  Converting YouTube Tracks for iDevices</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/new-building-immersive-thumbnails-for-igtv-videos/"><u>[New] Building Immersive Thumbnails for IGTV Videos</u></a></li>
<li><a href="https://fox-direct.techidaily.com/updated-in-2024-all-you-need-to-know-about-google-docs-audio-to-text-functionality/"><u>[Updated] In 2024, All You Need to Know About Google Docs Audio-to-Text Functionality</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1-harness-the-timeless-secret-transfer-files-to-your-phone-with-a-classic-technique/"><u>1. Harness the Timeless Secret: Transfer Files to Your Phone with a Classic Technique</u></a></li>
<li><a href="https://win11-tips.techidaily.com/5-routes-to-reviving-the-elusive-windows-terminal/"><u>5 Routes to Reviving the Elusive Windows Terminal</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/budget-friendly-productivity-software-evaluation-comparing-a-viable-and-economic-microsoft-office-rival/"><u>Budget-Friendly Productivity Software Evaluation: Comparing a Viable and Economic Microsoft Office Rival</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/complete-tutorial-make-taskbar-invisible-on-windows-11/"><u>Complete Tutorial: Make Taskbar Invisible on Windows 11</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/demystifying-phantom-sensation-in-virtual-reality-is-this-a-common-perception-among-users/"><u>Demystifying Phantom Sensation in Virtual Reality – Is This a Common Perception Among Users?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/discover-how-google-chromes-latest-update-includes-gemini-ai-for-an-advanced-smart-browser-functionality/"><u>Discover How Google Chrome's Latest Update Includes Gemini AI for an Advanced, Smart Browser Functionality</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/future-proofing-your-privacy-the-next-generation-of-cryptography/"><u>Future-Proofing Your Privacy: The Next Generation of Cryptography</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/general-motors-deploys-thousands-of-electric-vehicle-charging-stations-in-us-and-canadian-markets/"><u>General Motors Deploys Thousands of Electric Vehicle Charging Stations in U.S. and Canadian Markets</u></a></li>
<li><a href="https://fake-location.techidaily.com/how-to-fix-my-tecno-spark-20-pro-location-is-wrong-drfone-by-drfone-virtual-android/"><u>How to Fix My Tecno Spark 20 Pro Location Is Wrong | Dr.fone</u></a></li>
<li><a href="https://apple-account.techidaily.com/how-to-remove-an-airtag-from-your-apple-id-account-on-iphone-7-plus-by-drfone-ios/"><u>How to Remove an AirTag from Your Apple ID Account On iPhone 7 Plus?</u></a></li>
<li><a href="https://iphone-unlock.techidaily.com/how-to-unlock-iphone-13-pro-max-passcode-without-itunes-without-knowing-passcode-drfone-by-drfone-ios/"><u>How to Unlock iPhone 13 Pro Max Passcode without iTunes without Knowing Passcode? | Dr.fone</u></a></li>
<li><a href="https://unlock-android.techidaily.com/in-2024-how-to-unlock-infinix-note-30-vip-phone-with-broken-screen-by-drfone-android/"><u>In 2024, How to Unlock Infinix Note 30 VIP Phone with Broken Screen</u></a></li>
<li><a href="https://some-approaches.techidaily.com/in-2024-ultimate-360-degree-shoot-selecting-your-perfect-model/"><u>In 2024, Ultimate 360-Degree Shoot  Selecting Your Perfect Model</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/join-the-exclusive-listing-experience-googles-groundbreaking-bard-ai-chatbot-today/"><u>Join the Exclusive Listing: Experience Google's Groundbreaking BARD AI Chatbot Today!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-the-art-of-customized-wallpaper-designs-for-all-gadgets-with-midjourney-techniques/"><u>Mastering the Art of Customized Wallpaper Designs for All Gadgets with MidJourney Techniques</u></a></li>
<li><a href="https://tech-haven.techidaily.com/1722120515701-navigate-through-the-best-free-ai-image-synthesis-programs-our-open-source-selection/"><u>Navigate Through the Best Free AI Image Synthesis Programs – Our Open Source Selection!</u></a></li>
<li><a href="https://fox-that.techidaily.com/revitalize-your-iphone-top-10-fixes-for-non-functioning-safari-browser/"><u>Revitalize Your iPhone: Top 10 Fixes for Non-Functioning Safari Browser</u></a></li>
<li><a href="https://games-able.techidaily.com/swiftly-swapping-steam-deck-storage-cloning-made-simple/"><u>Swiftly Swapping Steam Deck Storage: Cloning Made Simple</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/tesla-battery-replacement-expenses-understanding-the-average-price/"><u>Tesla Battery Replacement Expenses: Understanding the Average Price</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/tesla-unveils-groundbreaking-new-electrical-utilities-venture/"><u>Tesla Unveils Groundbreaking New Electrical Utilities Venture</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-missing-link-between-xbox-series-x-and-virtual-gaming-an-in-depth-look-into-its-unavailability/"><u>The Missing Link Between Xbox Series X and Virtual Gaming - An In-Depth Look Into Its Unavailability</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-must-know-facts-for-choosing-the-right-smart-ring-a-preemptive-guide/"><u>The Must-Know Facts for Choosing the Right Smart Ring: A Preemptive Guide</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-ultimate-tutorial-on-crafting-non-fungible-tokens-nfts-for-beginners/"><u>The Ultimate Tutorial on Crafting Non-Fungible Tokens (NFTs) for Beginners</u></a></li>
<li><a href="https://win-able.techidaily.com/troubleshooting-tips-overcoming-frequent-crashes-while-playing-genshin-impact-on-pc/"><u>Troubleshooting Tips: Overcoming Frequent Crashes While Playing Genshin Impact on PC</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/understanding-and-assessing-the-condition-of-your-electric-vehicles-power-pack/"><u>Understanding and Assessing the Condition of Your Electric Vehicle's Power Pack</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/understanding-bifacial-solar-panels-benefits-and-considerations-before-your-next-purchase/"><u>Understanding Bifacial Solar Panels: Benefits & Considerations Before Your Next Purchase</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/understanding-the-limits-of-ai-exploring-6-instances-where-chatgpt-falls-short/"><u>Understanding the Limits of AI: Exploring 6 Instances Where ChatGPT Falls Short</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/upcoming-october-unveiling-metas-revolutionary-project-cambria-headset-redefines-vr-experience/"><u>Upcoming October Unveiling: Meta's Revolutionary Project Cambria Headset Redefines VR Experience</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/witness-the-next-generation-of-rocketry-four-must-see-spacecraft-lift-offs-coming-soon/"><u>Witness the Next Generation of Rocketry: Four Must-See Spacecraft Lift-Offs Coming Soon</u></a></li>
</ul></div>
