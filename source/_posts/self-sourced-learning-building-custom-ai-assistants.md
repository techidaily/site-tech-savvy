---
title: "Self-Sourced Learning: Building Custom AI Assistants"
date: 2024-12-24T17:22:27.064Z
updated: 2024-12-27T21:45:34.409Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes Self-Sourced Learning: Building Custom AI Assistants"
excerpt: "This Article Describes Self-Sourced Learning: Building Custom AI Assistants"
thumbnail: https://thmb.techidaily.com/e9f6abd8662955b9fc76151bcfa96786be75ef68a255d5c3126b3ad30bf05b53.jpg
---

## Self-Sourced Learning: Building Custom AI Assistants

 Providing GPT technology in a powerful and easy-to-use chatbot, ChatGPT has become the world's most popular AI tool. Many people use ChatGPT to provide engaging conversations, answer queries, offer creative suggestions, and aid in coding and writing. However, ChatGPT is limited as you cannot store your data for long-term personal use, and its September 2021 knowledge data cutoff point.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 As a workaround, we can use OpenAI's API and LangChain to provide ChatGPT with custom data and updated info past 2021 to create a custom ChatGPT instance.

>  Disclaimer: This post includes affiliate links
>
>  If you click on a link and make a purchase, I may receive a commission at no extra cost to you.
>

## Why Provide ChatGPT with Custom Data?

 Feeding ChatGPT with custom data and providing updated information beyond its knowledge cutoff date provides several benefits over just using ChatGPT as usual. Here are a few of them:

* **Personalized Interactions:** By providing ChatGPT with custom data, users can create a more customized experience. The model can be trained on specific datasets relevant to individual users or organizations, resulting in responses tailored to their unique needs and preferences.
* **Domain-Specific Expertise:** Custom data integration allows ChatGPT to specialize in particular domains or industries. It can be trained on industry-specific knowledge, terminology, and trends, enabling more accurate and insightful responses within those specific areas.
* **Current and Accurate Information:** Access to updated information ensures that ChatGPT stays current with the latest developments and knowledge. It can provide accurate responses based on recent events, news, or research, making it a more reliable source of information.

 Now that you understand the importance of providing custom data to ChatGPT, here's a step-by-step on how to do so on your local computer.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/c17xsnbinCQ?si=xHKslFgC3QbxY4qW" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

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

 When Installing Microsoft C++, you'll want to install **Microsoft Visual Studio Build Tools** first. Once installed, you can tick the **Desktop development with C++** option and click **Install** with all the optional tools automatically ticked on the right sidebar.

![Installing Microsoft C++ through Build Tools](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/2-install-c.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/YezPJZzPJ8Q?si=xF1t4BQHFquzvnzE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Now that you have installed the latest versions of Python3, Git, and Microsoft C++, you can download the Python script to easily query custom local data.

**Download:** [ChatGPT-retrieval script](https://github.com/techleadhd/chatgpt-retrieval) (Free)

 To download the script, click on **Code,** then select **Download ZIP**. This should download the Python script into your default or selected directory.

![Downloading Python script on GitHub](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/3-download-script.jpg)

 Once downloaded, we can now set up a local environment.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/5OmJZ4Z8jgk?si=YIoEaPI8geoiFSYE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## Step 2: Set Up the Local Environment

 To set up the environment, you'll need to open a terminal in the chatgpt-retrieval-main folder you downloaded. To do that, open **chatgpt-retrieval-main** folder, right-click, and select **Open in Terminal**.

![Opening terminal on directory folder](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/4-open-terminal.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/1CdWd06fCwc?si=wzg-68q0jAksPRXp" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 Once the terminal is open, copy and paste this command:

pip install langchain openai chromadb tiktoken unstructured

 This command uses Python's package manager to [create and manage the Python virtual environment](https://www.makeuseof.com/create-manage-python-virtual-environments/) needed.

 After creating the virtual environment, we need to supply an OpenAI API key to access their services. We'll first need to generate an API key from the [OpenAI API keys site](https://platform.openai.com/account/api-keys) by clicking on **Create new secret key**, adding a name for the key, then hitting the **Create secret key button**.

![Creating secret API key](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/generate-api-key.jpg)

 You will be provided with a string of characters. This is your OpenAI API key. Copy it by clicking on the copy icon on the side of the API key. Keep note that this API key should be kept secret. Do not share it with others unless you really intend for them to use it with you.

 Once copied, return to the chatgpt-retrieval-main folder and open constants with **Notepad**. Now replace the placeholder with your API key. Remember to save the file!

![Adding API key as environment variable](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/add-api-key.jpg)

 Now that you have successfully set up your virtual environment and added your OpenAI API key as an environment variable. You can now provide your custom data to ChatGPT.

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

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/KKFdFHaVIJg?si=x2vLw7ty3FtHX-9T" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 As you can see, it correctly described the AMD Instinct MI250x, which was released after ChatGPT -3's knowledge cutoff date.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/jjGL9wFdlbo?si=Vb1JgZqRXNc03UGG" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## Limitations of Custom ChatGPT

 Although feeding GPT-3.5 with custom data opens more ways to apply and use the LLM, there are a few drawbacks and limitations.

 Firstly, you need to provide all the data yourself. You can still access all the knowledge of GPT-3.5 until its knowledge cutoff date; however, you must provide all the extra data. This means if you want your local model to be knowledgeable of a certain subject on the internet that GPT-3.5 don't already know, you'll have to go to the internet and scrape the data yourself and save it as a text on the data folder of chatgpt-retrieval-main.

 Another issue is that querying ChatGPT like this takes more time to load when compared to asking ChatGPT directly.

 Lastly, the only model currently available is GPT-3.5 Turbo. So even if you have access to GPT-4, you won't be able to use it to power your custom ChatGPT instance.

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
<li><a href="https://facebook-video-footage.techidaily.com/new-2024-approved-a-comprehensive-look-editing-and-polishing-yt-videos-via-movie-maker/"><u>[New] 2024 Approved A Comprehensive Look Editing and Polishing YT Videos via Movie Maker</u></a></li>
<li><a href="https://article-files.techidaily.com/new-2024-approved-transform-your-shots-into-art-with-top-10-grids/"><u>[New] 2024 Approved Transform Your Shots Into Art with Top 10 Grids</u></a></li>
<li><a href="https://extra-skills.techidaily.com/new-movavis-enhanced-toolset-examining-plus-edition-2024/"><u>[New] Movavi's Enhanced Toolset Examining Plus Edition 2024</u></a></li>
<li><a href="https://fox-glue.techidaily.com/updated-2024-approved-steady-shot-enhancer-for-traveling-filmmakers/"><u>[Updated] 2024 Approved Steady Shot Enhancer for Traveling Filmmakers</u></a></li>
<li><a href="https://common-error.techidaily.com/comprehensive-solution-guide-to-restore-brightness-overcome-black-screens-on-dell-computers/"><u>Comprehensive Solution Guide to Restore Brightness - Overcome Black Screens on Dell Computers</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/discover-the-best-alternative-to-vizio-and-jbl-with-zdnets-in-depth-immersive-soundbar-testing/"><u>Discover the Best Alternative to Vizio & JBL with ZDNet's In-Depth Immersive Soundbar Testing</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/discovering-superior-sound-a-non-bose-non-sony-portable-speaker-tested-by-zdnet/"><u>Discovering Superior Sound: A Non-Bose, Non-Sony Portable Speaker Tested by ZDNet</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/experience-unmatched-sound-clarity-across-all-genres-using-cutting-edge-wireless-speakers-pcmag/"><u>Experience Unmatched Sound Clarity Across All Genres Using Cutting-Edge Wireless Speakers | PCMag</u></a></li>
<li><a href="https://extra-hints.techidaily.com/in-2024-capturing-eats-a-chefs-handbook-to-food-photography/"><u>In 2024, Capturing Eats A Chef's Handbook to Food Photography</u></a></li>
<li><a href="https://unlock-android.techidaily.com/in-2024-how-to-enable-usb-debugging-on-a-locked-tecno-phantom-v-fold-phone-by-drfone-android/"><u>In 2024, How To Enable USB Debugging on a Locked Tecno Phantom V Fold Phone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/revolutionary-speaker-system-surpasses-bose-outperforms-sonos-the-hidden-gem-you-need-to-know/"><u>Revolutionary Speaker System Surpasses Bose, Outperforms Sonos: The Hidden Gem You Need to Know</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/solution-police-officers-as-providers-of-an-essential-service-are-generally-prohibited-from-striking-by-both-federal-law-nlra-and-various-state-laws-due-to-207/"><u>Solution: Police Officers, as Providers of an Essential Service, Are Generally Prohibited From Striking by Both Federal Law (NLRA) and Various State Laws Due to the Critical Nature of Their Work for Public Safety.</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/top-rated-mobile-bluetooth-speakers-in-2/"><u>Top-Rated Mobile Bluetooth Speakers in 2</u></a></li>
<li><a href="https://win-dash.techidaily.com/ultimate-guide-access-lenovo-thinkpad-t430-driver-downloads-for-optimal-windows-compatibility/"><u>Ultimate Guide: Access Lenovo ThinkPad T430 Driver Downloads for Optimal Windows Compatibility</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ultimate-guide-tips-and-tricks-for-an-unforgettable-labor-day-bash/"><u>Ultimate Guide: Tips and Tricks for an Unforgettable Labor Day Bash</u></a></li>
<li><a href="https://win-amazing.techidaily.com/1722975789552-up-to-date-drivers-for-your-surface-book-fast-and-easy-access-now/"><u>Up-to-Date Drivers for Your Surface Book - Fast & Easy Access Now</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/zdnet-unveils-a-budget-friendly-portable-bluetooth-speaker-delivering-exceptional-audio-performance/"><u>ZDNet Unveils a Budget-Friendly Portable Bluetooth Speaker Delivering Exceptional Audio Performance</u></a></li>
</ul></div>

