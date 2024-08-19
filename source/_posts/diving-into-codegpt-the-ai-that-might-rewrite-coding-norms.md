---
title: "Diving Into CodeGPT: The AI That Might Rewrite Coding Norms"
date: 2024-08-18T10:06:55.687Z
updated: 2024-08-19T10:06:55.687Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Diving Into CodeGPT: The AI That Might Rewrite Coding Norms"
excerpt: "This Article Describes Diving Into CodeGPT: The AI That Might Rewrite Coding Norms"
thumbnail: https://thmb.techidaily.com/250855bb01ff5d1f68da39bedfd2fea2571983e53726cd5cc186abc1510baddd.jpg
---

## Diving Into CodeGPT: The AI That Might Rewrite Coding Norms

### Quick Links

* [What Is CodeGPT?](https://zonlipartnershipprogram.pxf.io/b0rbxy)
* [How Much Does CodeGPT Cost?](https://coinrule.sjv.io/rqzonv)
* [Can CodeGPT Really Write Code?](https://sentrypc.7eer.net/dkpkgn)

### Key Takeaways

* CodeGPT is an AI-powered coding assistant that helps programmers write and fix code, with features like auto-completion and code explanation.
* CodeGPT is available for free, but subscription plans for some features range from $9.99 to $49.99 per month.
* While CodeGPT can write code, its output may not always be error-free or follow best practices, so you should aim to understand and modify the generated code as necessary.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 If you're looking for an AI-powered assistant to help you write code, chances are you've encountered CodeGPT. It's one of many AI-powered tools you can use to assist you when programming. But can CodeGPT actually write code?

<!-- affiliate ads begin -->
<h3 id="200610"><a href="https://sentrypc.7eer.net/c/5597632/200610/3022">Parental Control Software</a></h3>
<span class="text-ad-content">
	#1 Rated Parental Control Software.<br/>
	Monitor & Control all PC Activity!<br/>
		<cite style="color:green">sentrypc.com/parental-controls/</cite>
	</span><img height="0" width="0" src="https://sentrypc.7eer.net/i/5597632/200610/3022" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## What Is CodeGPT?

 CodeGPT is a dedicated extension that uses different artificial intelligence (AI) models to help programmers write and fix code. It includes various features geared towards faster and easier programming, including auto-completion, code explanation, refactoring, documentation, unit testing, error-checking, and bug-fixing. It also has a ChatGPT-like interface you can access from your code editor.

 The extension is particularly powerful because it lets you connect to various mainstream [large language models (LLMs)](https://www.makeuseof.com/what-are-large-langauge-models-how-do-they-work/) from different providers like OpenAI and Google. On top of that, CodeGPT lets you create your own AI agents that you can use in your projects or share with others.

 While there are several [code editors for Linux](https://www.makeuseof.com/best-ide-code-editors-for-linux/), macOS, and Windows, CodeGPT is only available in two. Today, you can either [install and use CodeGPT in VS Code](https://www.makeuseof.com/install-use-codegpt-in-vs-code/) or in Cursor, which is a fork of VS Code.

<!-- affiliate ads begin -->
<a href="https://secure.2checkout.com/order/checkout.php?PRODS=2067133&QTY=1&AFFILIATE=108875&CART=1"><img src="https://www.pearlmountainsoft.com/n_img/product/gcb/banScrn.jpg" border="0">Greeting Card Builder</a>
<!-- affiliate ads end -->
## How Much Does CodeGPT Cost?

 You can download and install CodeGPT for free, but using the extension comes at a cost. CodeGPT offers various subscription packages that you can pay for if you need unlimited access.

 CodeGPT Plus has three subscription plans. The Basic plan goes for $9.99/month, followed by Standard ($19.99/month) and Gold ($49.99/month). There's a free trial period available, which you can use to evaluate the extension. Each package gives you access to specific AI agents with unlimited interactions.

 Bear in mind that you'll need to pay for unlimited usage of third-party AI models like OpenAI's GPT-4 model, for example. Although you can [access Open AI's GPT-4 model for free](https://www.makeuseof.com/ways-access-gpt-4-free/), you cannot do so from within VS Code or Cursor.

<!-- affiliate ads begin -->
<a href="https://otszone.ots7.com/order/checkout.php?PRODS=4713324&QTY=1&AFFILIATE=108875&CART=1"><img src="https://green.ots7.com/screenshots/OtsAV/OtsAVTV1.90-300x188.jpg" border="0">OtsAV TV Webcaster</a>
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
<li><a href="https://youtube-clips.techidaily.com/new-essential-apps-best-10-software-to-capture-your-screens/"><u>[New] Essential Apps  Best 10 Software to Capture Your Screens</u></a></li>
<li><a href="https://tiktok-video-recordings.techidaily.com/new-in-2024-crafting-a-tiktok-twosome-film/"><u>[New] In 2024, Crafting a TikTok Twosome Film</u></a></li>
<li><a href="https://screen-recording.techidaily.com/new-selecting-prime-4k-recorders-and-tools/"><u>[New] Selecting Prime 4K Recorders and Tools</u></a></li>
<li><a href="https://fox-access.techidaily.com/new-tunes-terms-and-copyrights-on-instagram/"><u>[New] Tunes, Terms, and Copyrights on Instagram</u></a></li>
<li><a href="https://some-techniques.techidaily.com/2024-approved-exclusive-list-general-knowledge-quiz-channels-24/"><u>2024 Approved  Exclusive List  General Knowledge Quiz Channels '24</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/2024-approved-step-up-your-game-techniques-for-bordered-instagram-videos/"><u>2024 Approved  Step Up Your Game  Techniques for Bordered Instagram Videos</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ai-assistance-for-complex-equations/"><u>AI Assistance for Complex Equations</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/an-overview-what-is-openai/"><u>An Overview: What Is OpenAI?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/analyzing-the-yin-and-yang-of-ai-and-creativity/"><u>Analyzing the Yin & Yang of AI and Creativity</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/battle-of-brilliance-gemini-vs-upgraded-chatgpt/"><u>Battle of Brilliance: Gemini Vs. Upgraded ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/best-practices-for-preventing-flaws-in-ai-generation/"><u>Best Practices for Preventing Flaws in AI Generation</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatting-with-ai-androids-voice-controlled-gpt-explained/"><u>Cha[t]ting with AI? Android's Voice Controlled GPT Explained</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-ban-by-italy-an-immediate-explancion/"><u>ChatGPT Ban by Italy: An Immediate Explanción</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/comparative-analysis-of-gpt-for-enterprises/"><u>Comparative Analysis of GPT for Enterprises</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/converse-confidently-with-nvidias-rtx-bot-on-your-computer/"><u>Converse Confidently with Nvidia's RTX Bot on Your Computer</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/customizing-workouts-with-ai-trainers-guide/"><u>Customizing Workouts with AI: Trainers' Guide</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/cyber-savvy-needed-recognize-authenticity-in-tech-titles/"><u>Cyber Savvy Needed: Recognize Authenticity in Tech Titles!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/daily-life-ais-who-takes-the-helm-in-taskland/"><u>Daily Life AIs: Who Takes the Helm in Taskland?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/deceiving-plugin-for-chatgpt-larcensively-saps-fb-logins/"><u>Deceiving Plugin for ChatGPT: Larcensively Saps FB Logins</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/discover-4-powerful-ai-story-generators-to-test/"><u>Discover 4 Powerful AI Story Generators to Test</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/emoji-less-tweets-on-twitter-linuss-revelations-explored-trojan-explained-and-chatgpt-concerns-addressed/"><u>Emoji-Less Tweets on Twitter, Linus’s Revelations Explored, Trojan Explained, & ChatGPT Concerns Addressed</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/essential-rules-for-freelancers-leveraging-chatgpt/"><u>Essential Rules for Freelancers Leveraging ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/examining-the-prestige-of-chatgpt-premium/"><u>Examining the Prestige of ChatGPT Premium</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/exploring-the-lags-chatgpt-4-versus-its-predecessor-gpt-35/"><u>Exploring the Lags: ChatGPT-4 Versus Its Predecessor GPT-3.5</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/google-palm-2-vs-openai-gpt-4-whats-the-difference/"><u>Google PaLM 2 Vs. OpenAI GPT-4: What's the Difference?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/gpt-4-demystified-in-verified-social-circles-by-meta/"><u>GPT-4 Demystified in Verified Social Circles by Meta</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/harnessing-ai-powered-search-on-bing-registration-tips/"><u>Harnessing AI-Powered Search on Bing: Registration Tips</u></a></li>
<li><a href="https://bypass-frp.techidaily.com/in-2024-is-gsm-flasher-adb-legit-full-review-to-bypass-your-vivo-y78t-phone-frp-lock-by-drfone-android/"><u>In 2024, Is GSM Flasher ADB Legit? Full Review To Bypass Your Vivo Y78t Phone FRP Lock</u></a></li>
<li><a href="https://unlock-android.techidaily.com/in-2024-universal-unlock-pattern-for-xiaomi-13t-by-drfone-android/"><u>In 2024, Universal Unlock Pattern for Xiaomi 13T</u></a></li>
<li><a href="https://facebook-video-share.techidaily.com/in-2024-youtube-mastery-elevate-your-content-with-smart-tag-techniques/"><u>In 2024, YouTube Mastery  Elevate Your Content with Smart Tag Techniques</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/innovating-conversation-key-enhancements-from-gpt-3/"><u>Innovating Conversation: Key Enhancements From GPT-3</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/innovation-in-content-creation-7-smart-ai-uses/"><u>Innovation in Content Creation: 7 Smart AI Uses</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/leading-edge-ai-methods-optimizing-internet-exploration/"><u>Leading-Edge AI Methods Optimizing Internet Exploration</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-chatgpt-a-guide-for-aspiring-freelancers/"><u>Mastering ChatGPT: A Guide for Aspiring Freelancers</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/navigate-with-ease-into-ai-enhanced-bing-setup-guide/"><u>Navigate with Ease Into AI-Enhanced Bing: Setup Guide</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/optimizing-writings-with-ai-help/"><u>Optimizing Writings with AI Help</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/quadruple-regulatory-routes-in-artificial-intelligence-by-government/"><u>Quadruple Regulatory Routes in Artificial Intelligence by Government</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/redefine-your-document-creation-10-must-have-ai-apps/"><u>Redefine Your Document Creation: 10 Must-Have AI Apps</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/rising-sea-levels-are-not-just-coastal-concerns/"><u>Rising Sea Levels Are Not Just Coastal Concerns</u></a></li>
<li><a href="https://fix-guide.techidaily.com/spotify-keeps-crashing-a-complete-list-of-fixes-you-can-use-on-nokia-c12-pro-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>Spotify Keeps Crashing A Complete List of Fixes You Can Use on Nokia C12 Pro | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/spotting-fraudulent-bingpt-crypto-before-its-too-late/"><u>Spotting Fraudulent BinGPT Crypto Before It's Too Late</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-content-creators-dilemma-notion-vs-openais-chatgpt/"><u>The Content Creators' Dilemma: Notion Vs. OpenAI's ChatGPT</u></a></li>
</ul></div>
