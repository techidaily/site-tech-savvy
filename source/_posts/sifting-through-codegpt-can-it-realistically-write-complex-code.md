---
title: "Sifting Through CodeGPT: Can It Realistically Write Complex Code?"
date: 2024-08-15T02:45:11.351Z
updated: 2024-08-16T02:45:11.351Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Sifting Through CodeGPT: Can It Realistically Write Complex Code?"
excerpt: "This Article Describes Sifting Through CodeGPT: Can It Realistically Write Complex Code?"
thumbnail: https://thmb.techidaily.com/c6867ae9c4f4e3df3c9379b15f4163ebd35319a50b7aab7a2fe4029be64b0298.jpg
---

## Sifting Through CodeGPT: Can It Realistically Write Complex Code?

### Quick Links

* [What Is CodeGPT?](https://zonlipartnershipprogram.pxf.io/b0rbxy)
* [How Much Does CodeGPT Cost?](https://coinrule.sjv.io/rqzonv)
* [Can CodeGPT Really Write Code?](https://sentrypc.7eer.net/dkpkgn)

<!-- affiliate ads begin -->
<a href="https://order.glarysoft.com/order/checkout.php?PRODS=35504869&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/6734fa703f6633ab896eecbdfad8953a/products/1_FR-200-1.png" border="0">Glarysoft File Recovery Pro Annually -  Helps to recover your lost file/data, even permanently deleted data. 
</a>
<!-- affiliate ads end -->
### Key Takeaways

* CodeGPT is an AI-powered coding assistant that helps programmers write and fix code, with features like auto-completion and code explanation.
* CodeGPT is available for free, but subscription plans for some features range from $9.99 to $49.99 per month.
* While CodeGPT can write code, its output may not always be error-free or follow best practices, so you should aim to understand and modify the generated code as necessary.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 If you're looking for an AI-powered assistant to help you write code, chances are you've encountered CodeGPT. It's one of many AI-powered tools you can use to assist you when programming. But can CodeGPT actually write code?

<!-- affiliate ads begin -->
<a href="https://store.movavi.com/affiliate.php?ACCOUNT=MOVAVI&AFFILIATE=108875&PATH=https%3A%2F%2Fwww.movavi.com%3FAFFILIATE%3D108875%26RESOURCE%3DMovavi%2BVideo%2BEditor%2Bbox"><img src="https://mcusercontent.com/0885a03ded3d480dca9287f12/images/6d3207fd-9f15-4c21-f0ad-59c68e6a7e2a.png" border="0"></a>
<!-- affiliate ads end -->
## What Is CodeGPT?

 CodeGPT is a dedicated extension that uses different artificial intelligence (AI) models to help programmers write and fix code. It includes various features geared towards faster and easier programming, including auto-completion, code explanation, refactoring, documentation, unit testing, error-checking, and bug-fixing. It also has a ChatGPT-like interface you can access from your code editor.

 The extension is particularly powerful because it lets you connect to various mainstream [large language models (LLMs)](https://www.makeuseof.com/what-are-large-langauge-models-how-do-they-work/) from different providers like OpenAI and Google. On top of that, CodeGPT lets you create your own AI agents that you can use in your projects or share with others.

 While there are several [code editors for Linux](https://www.makeuseof.com/best-ide-code-editors-for-linux/), macOS, and Windows, CodeGPT is only available in two. Today, you can either [install and use CodeGPT in VS Code](https://www.makeuseof.com/install-use-codegpt-in-vs-code/) or in Cursor, which is a fork of VS Code.

<!-- affiliate ads begin -->
<a href="https://estore.zonealarm.com/order/checkout.php?PRODS=36245101&QTY=1&AFFILIATE=108875&CART=1"><img src="https://sc1.checkpoint.com/sc1/za/images/boxes/zang_box_trust.png" border="0">ZoneAlarm Extreme Security NextGen</a>
<!-- affiliate ads end -->
## How Much Does CodeGPT Cost?

 You can download and install CodeGPT for free, but using the extension comes at a cost. CodeGPT offers various subscription packages that you can pay for if you need unlimited access.

 CodeGPT Plus has three subscription plans. The Basic plan goes for $9.99/month, followed by Standard ($19.99/month) and Gold ($49.99/month). There's a free trial period available, which you can use to evaluate the extension. Each package gives you access to specific AI agents with unlimited interactions.

 Bear in mind that you'll need to pay for unlimited usage of third-party AI models like OpenAI's GPT-4 model, for example. Although you can [access Open AI's GPT-4 model for free](https://www.makeuseof.com/ways-access-gpt-4-free/), you cannot do so from within VS Code or Cursor.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=4531356&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/8fdd149fcaa7058caccc9c4ad5b0d89a/products/tss-box.JPG" border="0">The Tube Sites Submitter is a fast and efficient tool for anyone who needs to upload videos quickly, easily and automatically to hundreds of tube sites in mere minutes . </a>
<!-- affiliate ads end -->
## Can CodeGPT Really Write Code?

 To evaluate this, we'll use the extension to help us generate two different code samples in Python.

 First, we ask the model to generate a stack data structure in Python with all the relevant methods. We used this prompt:

> Create a stack in Python and include all the necessary methods

 The model generated the following response:

`class Stack:  
    def __init__(self):  
        self.stack = []  
​  
    def push(self, item):  
        self.stack.append(item)  
​  
    def pop(self):  
        if self.is_empty():  
            raise IndexError("Pop from empty stack")  
        return self.stack.pop()  
​  
    def peek(self):  
        if self.is_empty():  
            raise IndexError("Peek from empty stack")  
        return self.stack [-1]  
​  
    def is_empty(self):  
        return len(self.stack) == 0  
​  
    def size(self):  
        return len(self.stack)`

 This sample shows that CodeGPT is clever enough to create the stack using a **class** and include the necessary checks to handle specific errors that may arise. For instance, the code throws informative errors if you try to **peek** or **pop** an empty stack.

 In a second challenge, we asked CodeGPT to save a response formatted in JSON from the [JSONPlaceholder](https://jsonplaceholder.typicode.com/) API to a CSV file. For context, the response from the JSONPlaceholder API looks like this:

`{  
 'userId': 1,  
 'id': 1,  
 'title': 'sunt aut facere repellat provident occaecati excepturi optio reprehenderit',  
 'body': 'quia et suscipit\nsuscipit recusandae consequuntur expedita et cum\nreprehenderit molestiae ut ut quas totam\nnostrum rerum est autem sunt rem eveniet architecto'  
}`

 We asked CodeGPT the following:

> I've made a request to an external API at <https://jsonplaceholder.typicode.com/posts/1> and I'm getting a response back. I've formatted the response as json, how can I save it in a csv file?

 The code that CodeGPT responded with was:

`import csv  
import requests  
  
# Make a GET request to the API  

response = requests.get('<https://jsonplaceholder.typicode.com/posts/1>')  

# Convert the response to JSON format  

data = response.json()  
  
# Since we're receiving a dictionary, we need to turn it into a list of one dictionary  

data = [data]  
  
# Open (or create) a CSV file to write the data  

with open('output.csv', 'w', newline='') as output_file:  
   # Create a CSV writer object  
   writer = csv.DictWriter(output_file, fieldnames=data [0].keys())  
   # Write the CSV headers  
   writer.writeheader()  
   # Write the data to the CSV file  
   writer.writerows(data)  
`

 Generally, this response is good; it doesn't need any tweaking to work. CodeGPT also added comments explaining the purpose of the various lines of code, which is useful if you're doing something for the first time.

 The only issue here is the response doesn't specify an encoding type while calling **open()**. While a default will automatically be included, specifying an encoding type is recommended and considered best practice when [writing to files in Python](https://www.makeuseof.com/write-print-to-file-python/). This might save you from incorrect interpretation, leading to jumbled text.

 So: CodeGPT can write code, but you should be careful because it won't always give you the best output. What you get might be error-prone and might not follow the best practices. Whenever you use CodeGPT or any other AI-powered tool to write code, strive to understand what the code does first. Don't just copy and paste.

</article

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
<li><a href="https://facebook-video-share.techidaily.com/new-2024-approved-budget-conscious-broadcayers-guide-to-cheap-mics/"><u>[New] 2024 Approved  Budget-Conscious Broadcayer's Guide to Cheap Mics</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/new-2024-approved-speak-slide-and-convince-the-vo-powerpoint-pathway/"><u>[New] 2024 Approved  Speak, Slide & Convince - The VO Powerpoint Pathway</u></a></li>
<li><a href="https://screen-sharing-recording.techidaily.com/new-cut-the-clutter-advanced-techniques-for-cam-recordings-for-2024/"><u>[New] Cut the Clutter  Advanced Techniques for Cam Recordings for 2024</u></a></li>
<li><a href="https://screen-video-capture.techidaily.com/new-in-2024-leading-tools-to-elevate-webcam-video-quality/"><u>[New] In 2024, Leading Tools to Elevate Webcam Video Quality</u></a></li>
<li><a href="https://facebook-video-share.techidaily.com/new-unveil-the-best-free-backdrop-and-footage-sources-top-8-online-lists/"><u>[New] Unveil the Best Free Backdrop & Footage Sources  Top 8 Online Lists</u></a></li>
<li><a href="https://facebook-video-footage.techidaily.com/updated-2024-approved-amplify-youtube-performance-rapid-video-rendering-guide/"><u>[Updated] 2024 Approved  Amplify YouTube Performance - Rapid Video Rendering Guide</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/updated-capture-your-gaming-moments-xbox-one-screenshots-made-simple/"><u>[Updated] Capture Your Gaming Moments  Xbox One Screenshots Made Simple</u></a></li>
<li><a href="https://fox-info.techidaily.com/updated-master-list-of-8-gratis-cutting-edge-video-players-for-pcmac-os/"><u>[Updated] Master List of 8 Gratis, Cutting-Edge Video Players for PC/Mac OS</u></a></li>
<li><a href="https://youtube-tips.techidaily.com/ed-sharing-stories-that-resonate-with-a-digital-audience-yt-for-2024/"><u>[Updated] Sharing Stories that Resonate with a Digital Audience YT for 2024</u></a></li>
<li><a href="https://facebook-video-footage.techidaily.com/updated-top-9-premium-wedding-films-online-youtube-and-vimeo/"><u>[Updated] Top 9 Premium Wedding Films Online  Youtube & Vimeo</u></a></li>
<li><a href="https://some-tips.techidaily.com/2024-approved-the-standard-edition-review-of-djis-drone-model-3/"><u>2024 Approved  The Standard Edition Review of DJI's Drone Model 3</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-innovations-showdown-dissecting-forefront-and-chatgpts-features/"><u>AI Innovations Showdown: Dissecting Forefront and ChatGPT's Features</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/artists-claim-vindication-against-openaimeta-in-court/"><u>Artists Claim Vindication: Against OpenAI/Meta in Court</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/backup-plans-for-elusive-chatgpt-exchanges/"><u>Backup Plans for Elusive ChatGPT Exchanges</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/bank-data-at-risk-the-role-of-gpt-in-todays-cyber-threats/"><u>Bank Data at Risk? The Role of GPT in Today's Cyber Threats</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/beyond-the-turing-emerging-evaluation-methods/"><u>Beyond The Turing: Emerging Evaluation Methods</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/bing-the-brainiac-search-engine/"><u>Bing, The Brainiac Search Engine</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-revolutionizing-office-writing-the-new-norm-in-word/"><u>ChatGPT Revolutionizing Office Writing: The New Norm in Word</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-powered-guide-to-youtube-video-script-creation/"><u>ChatGPT-Powered Guide to YouTube Video Script Creation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/deciphering-the-turing-tests-implications-and-future-victors/"><u>Deciphering The Turing Test's Implications & Future Victors</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/designing-balanced-dietary-patterns-with-gpt-aid/"><u>Designing Balanced Dietary Patterns with GPT Aid</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/detailed-insight-into-the-operation-of-shared-chatgpt-links/"><u>Detailed Insight Into the Operation of Shared ChatGPT Links</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/dodging-ai-crafted-windows-11-keys-a-good-practice/"><u>Dodging AI-Crafted Windows 11 Keys: A Good Practice</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/enhancing-analytical-prowess-in-excel-through-chatgpt-integration/"><u>Enhancing Analytical Prowess in Excel Through ChatGPT Integration</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/eye-catching-clues-to-fraudulent-chatgpt-websites/"><u>Eye-Catching Clues to Fraudulent ChatGPT Websites</u></a></li>
<li><a href="https://easy-unlock-android.techidaily.com/in-2024-lock-your-oppo-reno-10-proplus-5g-phone-in-style-the-top-5-gesture-lock-screen-apps-by-drfone-android/"><u>In 2024, Lock Your Oppo Reno 10 Pro+ 5G Phone in Style The Top 5 Gesture Lock Screen Apps</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/innovating-interaction-tomorrows-ai-evolution/"><u>Innovating Interaction: Tomorrow's AI Evolution</u></a></li>
<li><a href="https://vp-tips.techidaily.com/is-max-360-superior-to-hero-11-in-video-quality-in-2024/"><u>Is Max 360 Superior to Hero 11 in Video Quality, In 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/making-history-revolutionary-gpt-4-by-openai/"><u>Making History: Revolutionary GPT-4 by OpenAI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-chatgpt-an-openai-guide/"><u>Mastering ChatGPT: An OpenAI Guide</u></a></li>
<li><a href="https://extra-approaches.techidaily.com/mastering-video-creation-on-windows-10-a-step-by-step-guide-for-2024/"><u>Mastering Video Creation on Windows 10  A Step-by-Step Guide for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/perfecting-persuasion-the-smart-way-to-write-convincing-proposals-using-ai/"><u>Perfecting Persuasion: The Smart Way to Write Convincing Proposals Using AI</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/pilot-progressions-understanding-copilot-enhancements/"><u>Pilot Progressions: Understanding CoPilot Enhancements</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/proton-vpn-browser-extension-how-to-change-your-email-address-and-the-chatgpt-windows-app-is-fake/"><u>Proton VPN Browser Extension, How to Change Your Email Address, and the ChatGPT Windows App Is Fake</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/quick-fixes-for-stuck-chatgpt-apps-on-iphones/"><u>Quick Fixes for Stuck ChatGPT Apps on iPhones</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/quick-service-access-how-to-use-chatgpt-without-numbers/"><u>Quick Service Access: How to Use ChatGPT without Numbers</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-future-unfolds-top-features-of-newest-gpt-release/"><u>The Future Unfolds: Top Features of Newest GPT Release</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-paperclip-challenge-and-the-revolution-of-artificial-intelligence/"><u>The Paperclip Challenge and the Revolution of Artificial Intelligence</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/troubleshooting-tactics-to-salvage-your-iphones-chatgpt/"><u>Troubleshooting Tactics to Salvage Your iPhone's ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unveiling-the-potential-of-gpt-with-android/"><u>Unveiling the Potential of GPT with Android</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/vanguard-dialogues-how-gemini-meets-plus-gpt/"><u>Vanguard Dialogues: How Gemini Meets Plus-GPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/your-guide-to-understanding-and-using-claude-3/"><u>Your Guide to Understanding and Using Claude 3</u></a></li>
</ul></div>
