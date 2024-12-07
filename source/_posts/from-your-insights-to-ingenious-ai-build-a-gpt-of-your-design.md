---
title: "From Your Insights to Ingenious AI: Build a GPT of Your Design"
date: 2024-12-02T20:10:44.596Z
updated: 2024-12-06T17:00:49.350Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes From Your Insights to Ingenious AI: Build a GPT of Your Design"
excerpt: "This Article Describes From Your Insights to Ingenious AI: Build a GPT of Your Design"
thumbnail: https://thmb.techidaily.com/aaf0974e4ab83d3cc5b35041225761e54de0f8418307a4877fba8e369a6e30f0.jpg
---

## From Your Insights to Ingenious AI: Build a GPT of Your Design

 Providing GPT technology in a powerful and easy-to-use chatbot, ChatGPT has become the world's most popular AI tool. Many people use ChatGPT to provide engaging conversations, answer queries, offer creative suggestions, and aid in coding and writing. However, ChatGPT is limited as you cannot store your data for long-term personal use, and its September 2021 knowledge data cutoff point.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 As a workaround, we can use OpenAI's API and LangChain to provide ChatGPT with custom data and updated info past 2021 to create a custom ChatGPT instance.

>  Disclaimer: This post includes affiliate links
>
>  If you click on a link and make a purchase, I may receive a commission at no extra cost to you.
>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/ITtcSWvS8bo?si=4M4BfMgaabrW6148" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/5EKBEujWCw4?si=PwVvvervi8OrYaEA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 When Installing Microsoft C++, you'll want to install **Microsoft Visual Studio Build Tools** first. Once installed, you can tick the **Desktop development with C++** option and click **Install** with all the optional tools automatically ticked on the right sidebar.

![Installing Microsoft C++ through Build Tools](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/2-install-c.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/RCYs8keh-Vs?si=uDC28-9yh-k6HLj4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<iframe width="560" height="315" src="https://www.youtube.com/embed/620kcQ7Dw7w?si=a5ussGs5HV7sG3hF" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Now that you have successfully set up your virtual environment and added your OpenAI API key as an environment variable. You can now provide your custom data to ChatGPT.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/qObsqoJB9LI?si=ppqxfXzP0UL4J6Tp" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## Step 3: Adding Custom Data

 To add custom data, place all your custom text data in the **data** folder within chatgpt-retrieval-main. The format of the text data may be in the form of a PDF, TXT, or DOC.

![Adding custom data for ChatGPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/adding-data.jpg)

 As you can see from the screenshot above, I've added a text file containing a made-up personal schedule, an article I wrote on [AMD's Instinct Accelerators](https://www.makeuseof.com/what-are-amd-instinct-ai-accelerators/), and a PDF document.

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

## Limitations of Custom ChatGPT

 Although feeding GPT-3.5 with custom data opens more ways to apply and use the LLM, there are a few drawbacks and limitations.

 Firstly, you need to provide all the data yourself. You can still access all the knowledge of GPT-3.5 until its knowledge cutoff date; however, you must provide all the extra data. This means if you want your local model to be knowledgeable of a certain subject on the internet that GPT-3.5 don't already know, you'll have to go to the internet and scrape the data yourself and save it as a text on the data folder of chatgpt-retrieval-main.

 Another issue is that querying ChatGPT like this takes more time to load when compared to asking ChatGPT directly.

 Lastly, the only model currently available is GPT-3.5 Turbo. So even if you have access to GPT-4, you won't be able to use it to power your custom ChatGPT instance.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/yDuvbv0QOYI?si=byottcEM_Rrvi4EL" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
<li><a href="https://facebook-record-videos.techidaily.com/new-innovative-templates-for-stellar-youtube-video-decks/"><u>[New] Innovative Templates for Stellar YouTube Video Decks</u></a></li>
<li><a href="https://facebook-video-footage.techidaily.com/new-the-ultimate-android-video-editor-app-roundup/"><u>[New] The Ultimate Android Video Editor App Roundup</u></a></li>
<li><a href="https://youtube-blog.techidaily.com/ed-in-2024-youtube-clip-maker/"><u>[Updated] In 2024, Youtube Clip Maker</u></a></li>
<li><a href="https://youtube-lab.techidaily.com/approved-from-capture-to-share-proven-methods-for-live-360-video-on-youtube/"><u>2024 Approved From Capture to Share Proven Methods for Live 360° Video on Youtube</u></a></li>
<li><a href="https://desktop-recording.techidaily.com/2024-approved-universal-iptv-broadcasting/"><u>2024 Approved Universal IPTV Broadcasting</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ais-textual-adventure-uncovering-the-methodology-and-companies/"><u>AI's Textual Adventure: Uncovering the Methodology & Companies</u></a></li>
<li><a href="https://buynow-tips.techidaily.com/apple-ipad-air-4-review-like-a-more-affordable-ipad-pro/"><u>Apple iPad Air 4 Review: Like a More Affordable iPad Pro</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/charge-and-chill-with-the-ultimate-magsafe-multi-device-dock-for-apple-gadgets-top-picks/"><u>Charge and Chill with the Ultimate MagSafe Multi-Device Dock for Apple Gadgets Top Picks!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/discover-the-finest-july-2024-promotions-for-your-new-apple-watch-exclusive-deals/"><u>Discover the Finest July 2024 Promotions for Your New Apple Watch – Exclusive Deals!</u></a></li>
<li><a href="https://buynow-info.techidaily.com/experts-weigh-in-the-most-reliable-fintie-case-for-your-macbook-pro-13/"><u>Experts Weigh In: The Most Reliable Fintie Case for Your MacBook Pro 13?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/gpt-powered-text-interaction-for-paper-files/"><u>GPT-Powered Text Interaction for Paper Files</u></a></li>
<li><a href="https://hardware-tips.techidaily.com/huge-savings-on-elite-qled-television-models-up-to-1000-off-for-labor-day-sale-gadgetpundit-review/"><u>Huge Savings on Elite QLED Television Models - Up to $1,000 Off for Labor Day Sale | GadgetPundit Review</u></a></li>
<li><a href="https://change-location.techidaily.com/in-2024-6-ways-to-change-spotify-location-on-your-vivo-y78plus-drfone-by-drfone-virtual-android/"><u>In 2024, 6 Ways to Change Spotify Location On Your Vivo Y78+ | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/laughing-machines-the-genesis-of-laptops-and-advancements-in-vpn-security/"><u>Laughing Machines: The Genesis of Laptops & Advancements in VPN Security</u></a></li>
<li><a href="https://extra-support.techidaily.com/must-have-settings-for-online-broadcasting-for-2024/"><u>Must-Have Settings for Online Broadcasting for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/redefine-digital-conversation-explore-critical-updates-in-gpt/"><u>Redefine Digital Conversation: Explore Critical Updates in GPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-enduring-impact-and-future-role-of-the-turing-test/"><u>The Enduring Impact and Future Role of the Turing Test</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/top-ranking-iphone-and-ipad-vpn-apps-comprehensive-tests-and-reviews-by-tech-gurus-zdnet/"><u>Top-Ranking iPhone & iPad VPN Apps: Comprehensive Tests and Reviews by Tech Gurus | ZDNet</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/which-iphones-can-run-ios-18-detailed-compatibility-breakdown-for-apple-devices-techadvisoryorg/"><u>Which iPhones Can Run iOS 18? Detailed Compatibility Breakdown for Apple Devices | TechAdvisory.org</u></a></li>
</ul></div>

