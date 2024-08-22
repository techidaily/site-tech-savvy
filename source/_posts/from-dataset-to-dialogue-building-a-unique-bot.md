---
title: "From Dataset to Dialogue: Building a Unique Bot"
date: 2024-08-21T15:40:35.947Z
updated: 2024-08-22T15:40:35.947Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes From Dataset to Dialogue: Building a Unique Bot"
excerpt: "This Article Describes From Dataset to Dialogue: Building a Unique Bot"
thumbnail: https://thmb.techidaily.com/859749633d2fe977555173ddfc42dda3acc4bf2fd5329788d0569c467b1120f3.jpg
---

## From Dataset to Dialogue: Building a Unique Bot

 Providing GPT technology in a powerful and easy-to-use chatbot, ChatGPT has become the world's most popular AI tool. Many people use ChatGPT to provide engaging conversations, answer queries, offer creative suggestions, and aid in coding and writing. However, ChatGPT is limited as you cannot store your data for long-term personal use, and its September 2021 knowledge data cutoff point.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 As a workaround, we can use OpenAI's API and LangChain to provide ChatGPT with custom data and updated info past 2021 to create a custom ChatGPT instance.

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

<!-- affiliate ads begin -->
<a href="https://store.nero.com/order/checkout.php?PRODS=42296985&QTY=1&AFFILIATE=108875&CART=1"><img src="https://secure.avangate.com/images/merchant/9cea886b9f44a3c2df1163730ab64994/products/copy_nero_burning_rom_cart.png" border="0">
</a>
<!-- affiliate ads end -->
### Python3 and Microsoft C++ Installation Notes

 When installing Python3, make sure that you tick the **Add python.exe to PATH** option before clicking **Install Now**. This is important as it allows you to access Python in any directory on your computer.

![Adding Python to PATH](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/1-download-python.jpg)

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
 When Installing Microsoft C++, you'll want to install **Microsoft Visual Studio Build Tools** first. Once installed, you can tick the **Desktop development with C++** option and click **Install** with all the optional tools automatically ticked on the right sidebar.

![Installing Microsoft C++ through Build Tools](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/2-install-c.jpg)

 Now that you have installed the latest versions of Python3, Git, and Microsoft C++, you can download the Python script to easily query custom local data.

**Download:** [ChatGPT-retrieval script](https://github.com/techleadhd/chatgpt-retrieval) (Free)

 To download the script, click on **Code,** then select **Download ZIP**. This should download the Python script into your default or selected directory.

![Downloading Python script on GitHub](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/3-download-script.jpg)

<!-- affiliate ads begin -->
<a href="https://lightailing.sjv.io/c/5597632/1638364/17190" target="_top" id="1638364"><img src="//a.impactradius-go.com/display-ad/17190-1638364" border="0" alt="" width="1280" height="720"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1638364/17190" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 Once downloaded, we can now set up a local environment.

<!-- affiliate ads begin -->
<a href="https://estore.zonealarm.com/order/checkout.php?PRODS=38658749&QTY=1&AFFILIATE=108875&CART=1"><img src="https://sc1.checkpoint.com/sc1/za/images/boxes/pa_500.png" border="0">ZoneAlarm Pro Antivirus + Firewall NextGen</a>
<!-- affiliate ads end -->
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
<a href="https://versadesk.pxf.io/c/5597632/1892107/21290" target="_top" id="1892107"><img src="//a.impactradius-go.com/display-ad/21290-1892107" border="0" alt="" width="1200" height="628"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1892107/21290" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
 Now that you have successfully set up your virtual environment and added your OpenAI API key as an environment variable. You can now provide your custom data to ChatGPT.

## Step 3: Adding Custom Data

 To add custom data, place all your custom text data in the **data** folder within chatgpt-retrieval-main. The format of the text data may be in the form of a PDF, TXT, or DOC.

![Adding custom data for ChatGPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/07/adding-data.jpg)

<!-- affiliate ads begin -->
<a href="https://ukaidot.sjv.io/c/5597632/1793233/19578" target="_top" id="1793233"><img src="//a.impactradius-go.com/display-ad/19578-1793233" border="0" alt="" width="1200" height="1200"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1793233/19578" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
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
<a href="https://store.bitdefender.com/affiliate.php?ACCOUNT=BITLATIN&AFFILIATE=108875&PATH=http%3A%2F%2Fwww.bitdefender.com%2Fbusiness%3FAFFILIATE%3D108875%26RESOURCE%3D30%2525%2BOff%2Ball%2BGravityZone%2BProducts"><img src="https://www.bitdefender.com/content/dam/bitdefender/business/campaign/1200X628.png" border="0"></a>
<!-- affiliate ads end -->
 As you can see, it correctly described the AMD Instinct MI250x, which was released after ChatGPT -3's knowledge cutoff date.

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
<li><a href="https://youtube-data.techidaily.com/-new-take-on-favorite-movies-7-alternatives-for-2024/"><u>[New] A New Take on Favorite Movies - #7 Alternatives for 2024</u></a></li>
<li><a href="https://article-files.techidaily.com/new-customizing-your-faithful-phone-tunes-for-2024/"><u>[New] Customizing Your Faithful Phone Tunes for 2024</u></a></li>
<li><a href="https://screen-activity-recording.techidaily.com/new-efficient-techniques-unveiled-mastering-screen-recordings-with-showmore/"><u>[New] Efficient Techniques Unveiled  Mastering Screen Recordings with ShowMore</u></a></li>
<li><a href="https://facebook-clips.techidaily.com/new-for-beginners-leveraging-facebook-data-with-ease/"><u>[New] For Beginners  Leveraging Facebook Data with Ease</u></a></li>
<li><a href="https://instagram-videos.techidaily.com/new-how-to-add-good-bokeh-effects-in-instagram-stories/"><u>[New] How to Add Good Bokeh Effects in Instagram Stories</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/solved-cant-install-google-chrome-on-windows-10-in-s-mode/"><u>[SOLVED] | Can’t Install Google Chrome on Windows 10 in S Mode</u></a></li>
<li><a href="https://facebook-video-recording.techidaily.com/updated-2024-approved-keeping-your-browsing-free-of-pop-up-videos/"><u>[Updated] 2024 Approved  Keeping Your Browsing Free of Pop-Up Videos</u></a></li>
<li><a href="https://desktop-recording.techidaily.com/updated-navigating-google-translate-for-superior-speech-to-text/"><u>[Updated] Navigating Google Translate for Superior Speech-to-Text</u></a></li>
<li><a href="https://screen-video-capture.techidaily.com/updated-the-ultimate-farming-revamp-7-14-mod-comparison-guide/"><u>[Updated] The Ultimate Farming Revamp  #7-14 Mod Comparison Guide</u></a></li>
<li><a href="https://youtube-stream.techidaily.com/2024-approved-from-creator-to-earnings-successful-youtube-short-strategies/"><u>2024 Approved  From Creator to Earnings  Successful YouTube Short Strategies</u></a></li>
<li><a href="https://sim-unlock.techidaily.com/android-unlock-code-sim-unlock-your-realme-11-5g-phone-and-remove-locked-screen-by-drfone-android/"><u>Android Unlock Code Sim Unlock Your Realme 11 5G Phone and Remove Locked Screen</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/asus-laptop-touchpad-issues-solve-problems-in-windows-11-and-10-with-these-fixes/"><u>ASUS Laptop Touchpad Issues? Solve Problems in Windows 11 & 10 with These Fixes</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/best-vpn-for-windows-gaming/"><u>Best VPN for Windows Gaming</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/capturing-your-screen-easily-the-ultimate-guide-to-screenshots-on-a-dell-pc/"><u>Capturing Your Screen Easily: The Ultimate Guide to Screenshots on a Dell PC</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/complete-guide-steps-to-uninstall-chrome-add-ons-successfully/"><u>Complete Guide: Steps to Uninstall Chrome Add-Ons Successfully</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/comprehensive-guide-to-using-utorrent-for-easy-and-safe-film-acquisition/"><u>Comprehensive Guide to Using uTorrent for Easy and Safe Film Acquisition</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/create-a-zip-file-easily-for-windows-7-and-windows-11/"><u>Create a ZIP File Easily for Windows 7 & Windows 11</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/diagnosing-and-fixing-high-cpu-load-caused-by-security-software-in-windows-11-and-10-environments/"><u>Diagnosing and Fixing High CPU Load Caused by Security Software in Windows 11 & 10 Environments</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/effortless-steps-to-determine-your-nvidia-graphics-cards-current-driver/"><u>Effortless Steps to Determine Your NVIDIA Graphics Card's Current Driver</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1723808345167-effortlessly-start-your-pc-in-safe-mode-on-windows-11-a-comprehensive-guide-to-all-4-strategies-and-their-images/"><u>Effortlessly Start Your PC in Safe Mode on Windows 11 - A Comprehensive Guide to All 4 Strategies and Their Images!</u></a></li>
<li><a href="https://tech-revival.techidaily.com/elusive-tracking-safe-storing-of-gpt-interactions/"><u>Elusive Tracking: Safe Storing of GPT Interactions</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/error-free-windows-11-upgrade-overcoming-installation-hurdle-code-80240020/"><u>Error-Free Windows 11 Upgrade! Overcoming Installation Hurdle Code 80240020</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/expert-tips-to-overcome-the-quirky-crash-problem-in-goose-goose-duck-games/"><u>Expert Tips to Overcome the Quirky Crash Problem in Goose-Goose-Duck Games</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/guide-reducing-high-resource-demand-of-tiworkerexe-process-in-windows-11-systems/"><u>Guide: Reducing High Resource Demand of TiWorker.exe Process in Windows 11 Systems</u></a></li>
<li><a href="https://change-location.techidaily.com/how-do-you-get-sun-stone-evolutions-in-pokemon-for-samsung-galaxy-a14-4g-drfone-by-drfone-virtual-android/"><u>How Do You Get Sun Stone Evolutions in Pokémon For Samsung Galaxy A14 4G? | Dr.fone</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-correct-a-no-color-screen-in-windows-11/"><u>How to Correct a No-Color Screen in Windows 11</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-create-bootable-usb-for-windows-7-easily/"><u>How to Create Bootable USB for Windows 7 Easily</u></a></li>
<li><a href="https://fake-location.techidaily.com/in-2024-apply-these-techniques-to-improve-how-to-detect-fake-gps-location-on-vivo-y17s-drfone-by-drfone-virtual-android/"><u>In 2024, Apply These Techniques to Improve How to Detect Fake GPS Location On Vivo Y17s | Dr.fone</u></a></li>
<li><a href="https://apple-account.techidaily.com/in-2024-how-to-reset-apple-id-and-apple-password-from-apple-iphone-7-plus-by-drfone-ios/"><u>In 2024, How to Reset Apple ID and Apple Password From Apple iPhone 7 Plus</u></a></li>
<li><a href="https://iphone-unlock.techidaily.com/in-2024-how-to-unlock-iphone-7-plus-without-swiping-up-6-ways-drfone-by-drfone-ios/"><u>In 2024, How To Unlock iPhone 7 Plus Without Swiping Up? 6 Ways | Dr.fone</u></a></li>
<li><a href="https://bypass-frp.techidaily.com/in-2024-ultimate-guide-from-realme-11x-5g-frp-bypass-by-drfone-android/"><u>In 2024, Ultimate Guide from Realme 11X 5G FRP Bypass</u></a></li>
<li><a href="https://sound-optimizing.techidaily.com/new-in-2024-unleash-your-creative-potential-with-these-5-leading-audio-distortion-programs/"><u>New In 2024, Unleash Your Creative Potential with These 5 Leading Audio Distortion Programs</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/seamless-film-downloads-made-simple-navigating-the-ins-and-outs-of-utorrent/"><u>Seamless Film Downloads Made Simple: Navigating the Ins and Outs of uTorrent</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/1723808131903-seamlessly-integrate-a-bluetooth-mouse-into-windows-or-macos-environments/"><u>Seamlessly Integrate a Bluetooth Mouse Into Windows or macOS Environments.</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/solving-the-mystery-restored-my-missing-desktop-icons-in-windows-11/"><u>Solving the Mystery: Restored My Missing Desktop Icons in Windows 11</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/step-by-step-guide-hooking-up-your-laptop-to-a-television-via-hdmi-includes-images/"><u>Step-by-Step Guide: Hooking Up Your Laptop to a Television via HDMI - Includes Images!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/step-by-step-guide-updating-device-drivers-with-windows-10s-built-in-utility/"><u>Step-by-Step Guide: Updating Device Drivers with Windows 10'S Built-In Utility</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ultimate-guide-wirelessly-linking-your-pc-or-laptop-to-wi-fi/"><u>Ultimate Guide: Wirelessly Linking Your PC or Laptop to Wi-Fi</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/wi-fi-installation-tutorial-for-windows-7-users-step-by-step-solutions/"><u>Wi-Fi Installation Tutorial for Windows 7 Users: Step-by-Step Solutions</u></a></li>
</ul></div>
