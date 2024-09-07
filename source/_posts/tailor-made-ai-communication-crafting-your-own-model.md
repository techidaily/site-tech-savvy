---
title: "Tailor-Made AI Communication: Crafting Your Own Model"
date: 2024-09-06T23:32:25.003Z
updated: 2024-09-07T23:32:25.003Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Tailor-Made AI Communication: Crafting Your Own Model"
excerpt: "This Article Describes Tailor-Made AI Communication: Crafting Your Own Model"
thumbnail: https://thmb.techidaily.com/73077bb518e58764d0d667c24acb26e31ce2706dfa4d55a382cb32e354e1f132.jpg
---

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2115933/19272" target="_top" id="2115933">
  <img src="//a.impactradius-go.com/display-ad/19272-2115933" border="0" alt="https://techidaily.com" width="320" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2115933/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Tailor-Made AI Communication: Crafting Your Own Model

 Providing GPT technology in a powerful and easy-to-use chatbot, ChatGPT has become the world's most popular AI tool. Many people use ChatGPT to provide engaging conversations, answer queries, offer creative suggestions, and aid in coding and writing. However, ChatGPT is limited as you cannot store your data for long-term personal use, and its September 2021 knowledge data cutoff point.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 As a workaround, we can use OpenAI's API and LangChain to provide ChatGPT with custom data and updated info past 2021 to create a custom ChatGPT instance.

<!-- affiliate ads begin -->
<a href="https://ephamedtechinc.pxf.io/c/5597632/2137221/26400" target="_top" id="2137221">
  <img src="//a.impactradius-go.com/display-ad/26400-2137221" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://ephamedtechinc.pxf.io/i/5597632/2137221/26400" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Why Provide ChatGPT with Custom Data?

 Feeding ChatGPT with custom data and providing updated information beyond its knowledge cutoff date provides several benefits over just using ChatGPT as usual. Here are a few of them:

* **Personalized Interactions:** By providing ChatGPT with custom data, users can create a more customized experience. The model can be trained on specific datasets relevant to individual users or organizations, resulting in responses tailored to their unique needs and preferences.
* **Domain-Specific Expertise:** Custom data integration allows ChatGPT to specialize in particular domains or industries. It can be trained on industry-specific knowledge, terminology, and trends, enabling more accurate and insightful responses within those specific areas.
* **Current and Accurate Information:** Access to updated information ensures that ChatGPT stays current with the latest developments and knowledge. It can provide accurate responses based on recent events, news, or research, making it a more reliable source of information.

 Now that you understand the importance of providing custom data to ChatGPT, here's a step-by-step on how to do so on your local computer.

## Step 1: Install and Download Software and Pre-Made Script

 Please note the following instructions are for a Windows 10 or Windows 11 machine.

 To provide custom data to ChatGPT, you'll need to install and download the latest Python3, Git, Microsoft C++, and the ChatGPT-retrieval script from GitHub. If you already have some of the software installed on your PC, make sure they are updated with the latest version to avoid any hiccups during the process.

 Start by installing:

* **Download:**[Python3](https://www.python.org/downloads/) (Free)
* **Download:**[Git](https://git-scm.com/downloads) (Free)
* **Download:**[Microsoft Visual Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/) (Free)

### Python3 and Microsoft C++ Installation Notes

 When installing Python3, make sure that you tick the **Add python.exe to PATH** option before clicking **Install Now**. This is important as it allows you to access Python in any directory on your computer.

![Adding Python to PATH](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/1-download-python.jpg)

<!-- affiliate ads begin -->
<a href="https://ephamedtechinc.pxf.io/c/5597632/2123512/26400" target="_top" id="2123512">
  <img src="//a.impactradius-go.com/display-ad/26400-2123512" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://ephamedtechinc.pxf.io/i/5597632/2123512/26400" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 When Installing Microsoft C++, you'll want to install **Microsoft Visual Studio Build Tools** first. Once installed, you can tick the **Desktop development with C++** option and click **Install** with all the optional tools automatically ticked on the right sidebar.

![Installing Microsoft C++ through Build Tools](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/2-install-c.jpg)

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2115947/19272" target="_top" id="2115947">
  <img src="//a.impactradius-go.com/display-ad/19272-2115947" border="0" alt="https://techidaily.com" width="320" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2115947/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 Now that you have installed the latest versions of Python3, Git, and Microsoft C++, you can download the Python script to easily query custom local data.

**Download:** [ChatGPT-retrieval script](https://github.com/techleadhd/chatgpt-retrieval) (Free)

 To download the script, click on **Code,** then select **Download ZIP**. This should download the Python script into your default or selected directory.

![Downloading Python script on GitHub](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/3-download-script.jpg)

 Once downloaded, we can now set up a local environment.

## Step 2: Set Up the Local Environment

 To set up the environment, you'll need to open a terminal in the chatgpt-retrieval-main folder you downloaded. To do that, open **chatgpt-retrieval-main** folder, right-click, and select **Open in Terminal**.

![Opening terminal on directory folder](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/4-open-terminal.jpg)

 Once the terminal is open, copy and paste this command:

pip install langchain openai chromadb tiktoken unstructured

 This command uses Python's package manager to [create and manage the Python virtual environment](https://www.makeuseof.com/create-manage-python-virtual-environments/) needed.

 After creating the virtual environment, we need to supply an OpenAI API key to access their services. We'll first need to generate an API key from the [OpenAI API keys site](https://platform.openai.com/account/api-keys) by clicking on **Create new secret key**, adding a name for the key, then hitting the **Create secret key button**.

![Creating secret API key](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/generate-api-key.jpg)

 You will be provided with a string of characters. This is your OpenAI API key. Copy it by clicking on the copy icon on the side of the API key. Keep note that this API key should be kept secret. Do not share it with others unless you really intend for them to use it with you.

 Once copied, return to the chatgpt-retrieval-main folder and open constants with **Notepad**. Now replace the placeholder with your API key. Remember to save the file!

![Adding API key as environment variable](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/add-api-key.jpg)

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2130875/7443" target="_top" id="2130875">
  <img src="//a.impactradius-go.com/display-ad/7443-2130875" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2130875/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 Now that you have successfully set up your virtual environment and added your OpenAI API key as an environment variable. You can now provide your custom data to ChatGPT.

## Step 3: Adding Custom Data

 To add custom data, place all your custom text data in the **data** folder within chatgpt-retrieval-main. The format of the text data may be in the form of a PDF, TXT, or DOC.

![Adding custom data for ChatGPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/adding-data.jpg)

<!-- affiliate ads begin -->
<a href="https://ephamedtechinc.pxf.io/c/5597632/2137220/26400" target="_top" id="2137220">
  <img src="//a.impactradius-go.com/display-ad/26400-2137220" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://ephamedtechinc.pxf.io/i/5597632/2137220/26400" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 As you can see from the screenshot above, I've added a text file containing a made-up personal schedule, an article I wrote on [AMD's Instinct Accelerators](https://www.makeuseof.com/what-are-amd-instinct-ai-accelerators/), and a PDF document.

<!-- affiliate ads begin -->
<a href="https://aidotcom.pxf.io/c/5597632/2134501/19576" target="_top" id="2134501">
  <img src="//a.impactradius-go.com/display-ad/19576-2134501" border="0" alt="https://techidaily.com" width="640" height="90"/>
</a>
<img height="0" width="0" src="https://aidotcom.pxf.io/i/5597632/2134501/19576" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Step 4: Querying ChatGPT Through Terminal

 The Python script allows us to query data from the custom data we've added to the data folder and the internet. In other words, you will have access to the usual ChatGPT backend and all the data stored locally in the data folder.

 To use the script, run the python [chatgpt.py](http://chatgpt.py) script and then add your question or query as the argument.

python [chatgpt.py](http://chatgpt.py) "YOUR QUESTION"

 Make sure to put your questions in quotation marks.

 To test if we have successfully fed ChatGPT our data, I'll ask a personal question regarding the **Personal Sched.txt** file.

![Testing ChatGPT with custom data](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/visit.jpg)

 It worked! This means ChatGPT was able to read the Personal Sched.txt provided earlier. Now let's see if we have successfully fed ChatGPT with information it does not know due to its knowledge cutoff date.

![Asking custom ChatGPT about topic outside knowledge cut off data](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/m250x.jpg)

 As you can see, it correctly described the AMD Instinct MI250x, which was released after ChatGPT -3's knowledge cutoff date.

<!-- affiliate ads begin -->
<a href="https://25home.pxf.io/c/5597632/2123482/16836" target="_top" id="2123482">
  <img src="//a.impactradius-go.com/display-ad/16836-2123482" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://25home.pxf.io/i/5597632/2123482/16836" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Limitations of Custom ChatGPT

 Although feeding GPT-3.5 with custom data opens more ways to apply and use the LLM, there are a few drawbacks and limitations.

 Firstly, you need to provide all the data yourself. You can still access all the knowledge of GPT-3.5 until its knowledge cutoff date; however, you must provide all the extra data. This means if you want your local model to be knowledgeable of a certain subject on the internet that GPT-3.5 don't already know, you'll have to go to the internet and scrape the data yourself and save it as a text on the data folder of chatgpt-retrieval-main.

 Another issue is that querying ChatGPT like this takes more time to load when compared to asking ChatGPT directly.

 Lastly, the only model currently available is GPT-3.5 Turbo. So even if you have access to GPT-4, you won't be able to use it to power your custom ChatGPT instance.

<!-- affiliate ads begin -->
<a href="https://wigfever.sjv.io/c/5597632/2014850/22899" target="_top" id="2014850">
  <img src="//a.impactradius-go.com/display-ad/22899-2014850" border="0" alt="https://techidaily.com" width="320" height="90"/>
</a>
<img height="0" width="0" src="https://wigfever.sjv.io/i/5597632/2014850/22899" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## Custom ChatGPT Is Awesome But Limited

 Providing custom data to ChatGPT is a powerful way to get more out of the model. Through this method, you can feed the model with any text data you want and prompt it just like regular ChatGPT, albeit with some limitations. However, this will change in the future as it becomes easier to integrate our data with the LLM, along with access to the latest GPT-4 model.

**SCROLL TO CONTINUE WITH CONTENT**

 As a workaround, we can use OpenAI's API and LangChain to provide ChatGPT with custom data and updated info past 2021 to create a custom ChatGPT instance.


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
<li><a href="https://vimeo-videos.techidaily.com/new-2024-approved-guide-to-adding-creative-closure-in-vimeo-videos/"><u>[New] 2024 Approved Guide to Adding Creative Closure in Vimeo Videos</u></a></li>
<li><a href="https://fox-hovers.techidaily.com/new-2024-approved-superior-editing-software-tailored-to-dji-filmmaking/"><u>[New] 2024 Approved Superior Editing Software Tailored to DJi Filmmaking</u></a></li>
<li><a href="https://some-skills.techidaily.com/new-strategies-for-purchasing-clear-visual-content/"><u>[New] Strategies for Purchasing Clear Visual Content</u></a></li>
<li><a href="https://facebook-video-recording.techidaily.com/updated-2024-approved-facebook-videos-stop-buffering-and-glitches-on-devices/"><u>[Updated] 2024 Approved Facebook Videos Stop Buffering & Glitches on Devices</u></a></li>
<li><a href="https://facebook-videos.techidaily.com/updated-2024-approved-the-ultimate-strategy-for-creating-viral-hashtags-on-facebook/"><u>[Updated] 2024 Approved The Ultimate Strategy for Creating Viral Hashtags on Facebook</u></a></li>
<li><a href="https://vp-tips.techidaily.com/updated-experience-the-next-level-of-virtual-reality-with-htcs-vive-headset-for-2024/"><u>[Updated] Experience the Next Level of Virtual Reality with HTC's Vive Headset for 2024</u></a></li>
<li><a href="https://iphone-transfer.techidaily.com/5-ways-to-transfer-music-from-apple-iphone-14-plus-to-android-drfone-by-drfone-transfer-from-ios/"><u>5 Ways to Transfer Music from Apple iPhone 14 Plus to Android | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/adapting-careers-in-an-ai-driven-world/"><u>Adapting Careers in an AI-Driven World</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/avoid-data-sharing-by-opting-out-of-chatgpt/"><u>Avoid Data Sharing by Opting Out of ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/boosting-browsers-conversational-power-our-top-7-plugin-lists/"><u>Boosting Browsers' Conversational Power: Our Top 7 Plugin Lists</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/boosting-efficiency-the-ultimate-guide-to-using-chatgpt-effectively/"><u>Boosting Efficiency: The Ultimate Guide to Using ChatGPT Effectively</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/breaking-through-gpt-3-limits-solving-four-common-problems/"><u>Breaking Through GPT-3 Limits: Solving Four Common Problems</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/cutting-through-the-noise-persuasive-proposals-and-chatgpt/"><u>Cutting Through The Noise: Persuasive Proposals & ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/embark-on-a-venture-into-dialogue-system-crafting/"><u>Embark on a Venture Into Dialogue System Crafting</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/exploring-bards-ai-evolution-7-innovative-traits-announced/"><u>Exploring Bard's AI Evolution: 7 Innovative Traits Announced</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/from-code-to-conversation-ai-written-tales/"><u>From Code to Conversation: AI' Written Tales</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/from-conversation-to-creativity-4-reasons-for-claude-3-preference/"><u>From Conversation to Creativity: 4 Reasons for Claude 3 Preference</u></a></li>
<li><a href="https://instagram-video-files.techidaily.com/harmonize-video-quality-with-instagrams-visual-theme-for-2024/"><u>Harmonize Video Quality with Instagram's Visual Theme for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/leveraging-chatgpts-plugin-for-wolfram-alpha-triad/"><u>Leveraging ChatGPT's Plugin for Wolfram Alpha Triad</u></a></li>
<li><a href="https://facebook-video-files.techidaily.com/leveraging-high-roi-crafting-dynamic-animated-ads-for-fb/"><u>Leveraging High ROI Crafting Dynamic Animated Ads for FB</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/maximizing-business-value-with-7-innovative-uses-of-chatgpt/"><u>Maximizing Business Value with 7 Innovative Uses of ChatGPT</u></a></li>
<li><a href="https://ai-video-apps.techidaily.com/new-2024-approved-editing-canon-videos-on-a-budget-free-and-affordable-software-options/"><u>New 2024 Approved Editing Canon Videos on a Budget Free and Affordable Software Options</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/simplifying-clean-up-the-route-to-fresh-gpt-dialogues/"><u>Simplifying Clean-Up: The Route to Fresh GPT Dialogues</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-best-4-ai-writing-companions-for-every-wordsmith/"><u>The Best 4 AI Writing Companions for Every Wordsmith</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-editors-guide-to-responsible-ai-engagement/"><u>The Editor's Guide to Responsible AI Engagement</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/toms-tech-gear-comprehensive-hardware-reviews/"><u>Tom's Tech Gear - Comprehensive Hardware Reviews</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/top-6-frequent-gpt-missteps-and-corrections-guide/"><u>Top 6 Frequent GPT Missteps & Corrections Guide</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unlocking-potential-with-quoras-poe-access/"><u>Unlocking Potential with Quora's POE Access</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/vital-upgrades-to-revolutionize-the-gpt-plugin-registry/"><u>Vital Upgrades to Revolutionize the GPT Plugin Registry</u></a></li>
</ul></div>
