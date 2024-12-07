---
title: How ChatGPT Overlooks Its Own Syntax
date: 2024-11-30T00:27:44.758Z
updated: 2024-12-06T20:48:25.183Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes How ChatGPT Overlooks Its Own Syntax
excerpt: This Article Describes How ChatGPT Overlooks Its Own Syntax
thumbnail: https://thmb.techidaily.com/e19f7ed8ea4947e7863a6b27aaaa0b4c70d6ab972ded390e593c80bf54aa6b43.jpg
---

## How ChatGPT Overlooks Its Own Syntax

 Following the launch of ChatGPT in November 2022, the phenomenal AI chatbot has emerged as one of the most trusted writing tools on the internet. It's simple to use; describe what you need to be written, and ChatGPT prints it on screen in seconds.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 However, in an era where AI-generated text is passed as human-written and used to gain an unfair advantage, identifying AI content is very important. But ChatGPT cannot accurately spot AI content, even its own work—but why?

>  Disclaimer: This post includes affiliate links
>
>  If you click on a link and make a purchase, I may receive a commission at no extra cost to you.
>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/w7c5EHp-GDw?si=UTw7lZR0wTmRjp8W" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## Is There a Difference Between AI Text and Human Writing?

 A precondition for ChatGPT to spot its own writing or any AI-generated text is that there has to be a difference between it and human-written text. So, is there any significant difference between human-written text and AI-generated content? If there is, surely, a tool like ChatGPT should be able to discern it.

 We wrote a short story without any input from any AI tool and then asked ChatGPT whether the story was AI-written content. ChatGPT confidently flagged it as an AI-generated text.

![False positive judgement by ChatGPT](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/06/false-positive-judgement-by-chatgpt.jpg)

 We then asked ChatGPT to generate a story, and in that same chat thread, we copy-pasted the generated text and asked ChatGPT whether the text was AI-created. ChatGPT's response? A confident "No."

![ChatGPT false negative judgement](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/06/chatgpt-false-negative-judgement.jpg)

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/97ydpSmzTJw?si=tFcelmtQX4u-b3u5" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

 ChatGPT failed at identifying human-written or AI-generated text in both cases. So how come ChatGPT cannot detect its own text? Does this mean there is no difference between AI and human text?

 Well, there is. We could write an entire book on the difference between the two, but it won't matter much. So, if there's a difference, why is ChatGPT or any other AI tool unable to identify these differences and accurately point out AI-generated text from a human-written one? The answer lies in [how ChatGPT works and how it generates text](http://www.makeuseof.com/how-does-chatgpt-work/).

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/2Iv3DjT2Fyw?si=pR_z8ZDDVGF2MvKJ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## How ChatGPT Generates Text

![Artificial intelligence and puny human are shaking hands](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/the-power-of-ai.jpg)

 When you ask ChatGPT to generate text, it tries to mimic the human writing process. Firstly, the model behind ChatGPT—Generative Pre-trained Transformer (GPT)—has been trained on a large corpus of human text. Everything from emails, health articles, tech articles, high school essays, and just about any text you can find online has been fed to the model during training. So ChatGPT understands how each of these types of texts should be written.

 If you ask ChatGPT to write an email to your boss, it knows how an email of that nature should look because it has been trained on similar emails—probably thousands of them. Similarly, if you ask it to write a high school essay, it also knows how a high school essay should sound. ChatGPT will try to write whatever you want it to write in a way a human would.

 But there's a catch. Unlike how humans write, ChatGPT does not really understand what it is writing in a way that a human would. Instead, the chatbot tries to predict what would be the most plausible next word in a sentence until it completes the write-up.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/MTb4xHzeQEk?si=9Sqq-gFWnHc8x3_P" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## How ChatGPT Writes by Prediction

 Let's say you ask ChatGPT to write a story about a fictional city called Volkra. There's a huge possibility that the chatbot will start the story with the words "Once upon." This is because the chatbot doesn't think for itself but tries to predict what a human would write based on what it has learned from the thousands of stories it has been fed during training.

 So, believing a human would likely start the story with the words "Once upon," ChatGPT would then try to predict the next logical word, which would be "a" followed by "time." So you would then have "Once upon a time..." followed by the next logical word and the next until the story is completed. ChatGPT basically writes by predicting what word would naturally (or at least has the highest probability) of coming next in a sentence and inserting it.

 So, when an AI tool tries to detect whether a text is AI-generated, one of the criteria it tries to weigh is the predictability of the text since AI tools write by prediction. This measure of predictability is called perplexity in AI parlance. Now, when presented with a text, among other criteria, an AI tool like ChatGPT tries to analyze the text to measure how predictable the sequence of words or sentences in the text is. Greater predictability or low perplexity typically means the text is likely AI-generated. Less predictability or higher perplexity typically means the text is likely written by humans.

 These criteria, along with other factors like the level of creativity of a text, are unfortunately not enough to ascertain with certainty whether a text is written by an AI tool or not. This is because humans can write with greater variance, as in the example text we used for demonstration at the beginning of this article.

 AI chatbots like ChatGPT are designed to mimic natural human language as much as possible. So while AI text may have discernable patterns, those patterns are not so obvious even to a powerful tool like ChatGPT. This is why ChatGPT can not spot its own writing, as well as [why AI-text detector tools do not work](https://www.makeuseof.com/ai-content-detectors-dont-work/).

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/LaWcXdTn5SE?si=QbxEkX-4a17J5RVs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## Will ChatGPT Recognize Its Own Writing In the Future?

 Currently, tools like ChatGPT can not detect whether a text was written by itself or any other AI tool because there's no clear, discernable pattern in AI-generated content. However, there's a good chance that this could change soon. With efforts by companies like ChatGPT to introduce digital watermarks into ChatGPT-generated content, there will be a more discernable pattern to the text generated by the chatbot.

**SCROLL TO CONTINUE WITH CONTENT**

 However, in an era where AI-generated text is passed as human-written and used to gain an unfair advantage, identifying AI content is very important. But ChatGPT cannot accurately spot AI content, even its own work—but why?

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
<li><a href="https://vimeo-videos.techidaily.com/new-2024-approved-celeb-in-a-nutshell-vimeo/"><u>[New] 2024 Approved Celeb in a Nutshell – Vimeo</u></a></li>
<li><a href="https://some-knowledge.techidaily.com/new-exploring-the-frontier-top-360-cameras-for-industry-pros-2023/"><u>[New] Exploring the Frontier Top 360° Cameras for Industry Pros, 2023</u></a></li>
<li><a href="https://instagram-video-recordings.techidaily.com/new-hear-the-difference-mastering-instagram-voice-customizations/"><u>[New] Hear the Difference Mastering Instagram Voice Customizations</u></a></li>
<li><a href="https://screen-video-capture.techidaily.com/new-in-2024-capturing-your-touch-top-8-free-android-recorders/"><u>[New] In 2024, Capturing Your Touch Top 8 Free Android Recorders</u></a></li>
<li><a href="https://article-posts.techidaily.com/updated-enrich-your-screenplay-exclusive-windows-11-creations-for-2024/"><u>[Updated] Enrich Your Screenplay Exclusive Windows 11 Creations for 2024</u></a></li>
<li><a href="https://instagram-clips.techidaily.com/updated-sculpting-visual-stories-editing-vertical-videos-for-ig-in-fcpx/"><u>[Updated] Sculpting Visual Stories Editing Vertical Videos for IG in FCPX</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/favorite-phones-among-experts-the-top-mobile-devices-endorsed-by-zdnet-journalists/"><u>Favorite Phones Among Experts: The Top Mobile Devices Endorsed by ZDNet Journalists</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/freeing-gpt-use-without-openai-accounts/"><u>Freeing GPT Use without OpenAI Accounts</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/how-to-use-chatgpt-for-3d-printing/"><u>How to Use ChatGPT for 3D Printing</u></a></li>
<li><a href="https://bypass-frp.techidaily.com/in-2024-step-by-step-tutorial-how-to-bypass-infinix-hot-40-pro-frp-by-drfone-android/"><u>In 2024, Step-by-Step Tutorial How To Bypass Infinix Hot 40 Pro FRP</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/innovative-enterprise-solutions-through-gpt-chat-whisper-access/"><u>Innovative Enterprise Solutions Through GPT-Chat, Whisper Access</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ready-for-adventure-with-vision-pro-travel-mode-uncover-everything-you-need-to-know-first-a-guide/"><u>Ready for Adventure with Vision Pro Travel Mode? Uncover Everything You Need to Know First - A Guide</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/rethinking-trust-a-closer-look-at-zerogpt/"><u>Rethinking Trust: A Closer Look at ZeroGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/scaling-up-innovative-design-methods-with-canva-and-ai-assistance/"><u>Scaling Up: Innovative Design Methods with Canva & AI Assistance</u></a></li>
<li><a href="https://tech-recovery.techidaily.com/the-essentials-of-ray-tracing-explained-simply/"><u>The Essentials of Ray Tracing Explained Simply</u></a></li>
<li><a href="https://tech-haven.techidaily.com/the-limits-of-ai-detection-tools-insights-and-case-studies-zerogpt/"><u>The Limits of AI Detection Tools - Insights and Case Studies (ZeroGPT)</u></a></li>
<li><a href="https://tech-haven.techidaily.com/unleash-creative-potential-large-scale-workflow-via-canva-and-chatgpt/"><u>Unleash Creative Potential - Large-Scale Workflow via Canva & ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/upgrade-your-mobile-life-with-these-amazing-iphone-eby-16-innovations-as-discovered-on-zdnet/"><u>Upgrade Your Mobile Life with These Amazing iPhone Eby 16 Innovations, as Discovered on ZDNet</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/zdnet-unveils-top-mp3-player-picks-expert-comparison-guide/"><u>ZDNet Unveils Top MP3 Player Picks - Expert Comparison Guide</u></a></li>
</ul></div>

