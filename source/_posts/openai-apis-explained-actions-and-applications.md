---
title: "OpenAI APIs Explained: Actions and Applications"
date: 2025-02-28T23:47:54.420Z
updated: 2025-03-04T17:13:23.395Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: "This Article Describes OpenAI APIs Explained: Actions and Applications"
excerpt: "This Article Describes OpenAI APIs Explained: Actions and Applications"
thumbnail: https://thmb.techidaily.com/b461869fdc65b7a58affdd23329a3336b55cdb42a5e0550c353e9047546c19d2.jpg
---

## OpenAI APIs Explained: Actions and Applications

 ChatGPT's generative power has caused a frenzy in the tech world since it launched. To share the AI's intuition, OpenAI released the ChatGPT and Whisper APIs on March 1, 2023, for developers to explore and consume in-app.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 OpenAI's APIs feature many valuable endpoints that make AI integration easy. Let's explore the power of OpenAI APIs to see how they can benefit you.

## What Can the OpenAI API Do?

 The [OpenAI API](https://platform.openai.com/) packs in a bunch of utilities for programmers. If you intend to deliver in-app AI daily, OpenAI will make your life easier with the following abilities.

### Chat

 The OpenAI API chat completion endpoint helps the end user to spin up a natural, human-friendly interactive session with a virtual assistant using the GPT-3.5-turbo model.

 Backstage, the API call uses a message array of roles and content. On the user side, content is a set of instructions for the virtual assistant, which engages the user, while for the model, content is its response.

 The top-level role is the system, where you define the overall function of the virtual assistant. For instance, when the programmer tells the system something like "you are a helpful virtual assistant," you expect it to respond to various questions within its learning capacity.

 After telling it to be "a helpful virtual assistant," here's how one of our command-line chats went with the GPT-3.5-turbo model:

![Chat completion chat CLI logs](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/chat-completion-chat-cli-logs.jpg)

 You can even improve the model's performance by supplying parameters like temperature, presence-penalty, frequency-penalty, and more. If you've ever used ChatGPT, you already know how OpenAI's chat completion model work.

### Text Completion

 The text completion API provides conversational, text insertion, and text completion functionalities based on advanced GPT-3.5 models.

 The champion model in the text completion endpoint is text-davinci-003, which is considerably more intuitive than GPT-3 natural language models. The endpoint accepts a user prompt, allowing the model to respond naturally and complete simple to complex sentences using human-friendly text.

 Although the text-completion endpoint isn't as intuitive as the chat endpoint, it gets better—as you increase the text tokens supplied to the text-davinci-003 model.

 For instance, we got some half-baked completions when we placed the model on a max\_tokens of seven:

![Text completion model test via CLI](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/text-completion-model-test-via-cli.jpg)

 However, increasing the max\_tokens to 70 generated more coherent thoughts:

![Text completion model test via CLI more complete](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/text-completion-model-test-via-cli-more-complete.jpg)

### Speech-to-Text

 You can transcribe and translate audio speech using the OpenAI transcription and translation endpoints. The speech-to-text endpoints are based on the Whisper v2-large model, developed through large-scale weak supervision.

 However, OpenAI says there's no difference between its Whisper model and the one in open-source. So it offers endless opportunities for integrating a multilingual transcriber and translator AI into your app at scale.

 The endpoint usage is simple. All you have to do is to supply the model with an audio file and call the **openai.Audio.translate** or **openai.Audio.transcribe** endpoint to translate or transcribe it respectively. These endpoints accept a maximum file size of 25 MB and support most audio file types, including mp3, mp4, MPEG, MPGA, m4a, wav, and webm.

### Text Comparison

 OpenAI API text comparison endpoint measures the relationship between texts using the text-embedding-ada-002 model, a second-generation embedding model. The embedding API uses this model to evaluate the relationship between texts based on the distance between two vector points. The wider the difference, the less related the texts under comparison are.

 The embedding endpoint features text clustering, differences, relevance, recommendations, sentiments, and classification. Plus, it charges per token volume.

 Although the OpenAI documentation says you can use the other first-generation embedding models, the former is better with a cheaper price point. However, OpenAI warns that the embedding model might show social bias towards certain people, as proven in tests.

### Code Completion

 The code completion endpoint is built on the OpenAI Codex, a set of models trained using natural language and billions of code lines from public repositories.

 The endpoint is in limited beta and free as of writing, offering support for many modern programming languages, including JavaScript, Python, Go, PHP, Ruby, Shell, TypeScript, Swift, Perl, and SQL.

 With the code-davinci-002 or code-cushman-001 model, the code completion endpoint can auto-insert code lines or spin up code blocks from a user's prompt. While the latter model is faster, the former is the powerhouse of the endpoint, as it features code insertions for code auto-completion.

 For instance, you can generate a code block by sending a prompt to the endpoint in the target language comment.

 Here are some responses we got when we tried generating some code blocks in Python and JavaScript via the terminal:

![OpenAI code completion command prompt](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/openai-code-completion-command-prompt.jpg)

### Image Generation

 This is one of the most intuitive features of the OpenAI API. Based on the DALL.E image model, the OpenAI API's image functionality features endpoints for generating, editing, and creating image variations from natural language prompts.

 Although it doesn't yet have advanced features like upscaling as it's still in beta, its unscaled outputs are more impressive than those of generative [art models like Midjourney](http://www.makeuseof.com/how-to-use-midjourney-create-ai-art/) and Stable Diffusion.

 While hitting the image generation endpoint, you only need to supply a prompt, image size, and image count. But the image editing endpoint requires you to include the image you wish to edit and an RGBA mask marking the edit point in addition to the other parameters.

 The variation endpoint, on the other hand, only requires the target image, the variation count, and the output size. At the time of writing, OpenAI's beta image endpoints can only accept square frames in the range 256x256, 512x512, and 1024x1024 pixels.

 We created a simple image generation application using this endpoint, and though it missed some details, it gave an incredible result:

![Image generation test for OpenAI](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/image-generation-test-for-openai.jpg)

## How to Use the OpenAI API

![OpenAI API secret key page](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/openai-api-secret-key-page.jpg)

 ​​​​​ The OpenAI API usage is simple and follows the conventional API consumption pattern.

1. Install the **openai** package using pip: **pip install openai**.If using Node instead, you can do so using npm: **npm install openai**.
2. **Grab your API keys**: Log into your OpenAI dashboard and click your profile icon at the top right. Go to **View API Keys** and click **Create new secret key** to generate your API secret key.
3. Make API calls to your chosen model endpoints via a server-side language like Python or JavaScript (Node). Feed these to your custom APIs and test your endpoints.
4. Then [fetch custom APIs via JavaScript](http://www.makeuseof.com/how-to-consume-apis-in-react-using-fetch-and-axios/) frameworks like React, Vue, or Angular.
5. Present data (user requests and model responses) in a visually appealing UI, and your app is ready for real-world use.

## What Can You Create With the OpenAI API?

 The OpenAI APIs create entry points for real-life usage of machine learning and reinforcement learning. While opportunities for creativity abound, here are a few of what you can build with the OpenAI APIs:

1. Integrate an intuitive virtual assistant chatbot into your website or application using the chat completion endpoint.
2. Create an image editing and manipulation app that can naturally insert an object into an image at any specified point using the image generation endpoints.
3. Build a custom machine learning model from the ground up using OpenAI's model fine-tune endpoint.
4. Fix subtitles and translations for videos, audio, and live conversations using the speech-to-text model endpoint.
5. Identify negative sentiments in your app using the OpenAI embedding model endpoint.
6. Create programming language-specific code completion plugins for code editors and integrated development environments (IDEs).

## Build Endlessly With the OpenAI APIs

 Our daily communication often involves the exchange of written content. The OpenAI API only extends its creative tendencies and potential, with seemingly limitless natural language use cases.

 It’s still early days for the OpenAI API. But expect it to evolve with more features as time passes.

**SCROLL TO CONTINUE WITH CONTENT**

 OpenAI's APIs feature many valuable endpoints that make AI integration easy. Let's explore the power of OpenAI APIs to see how they can benefit you.

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
<li><a href="https://fox-friendly.techidaily.com/new-in-2024-the-future-shaped-by-quantum-hdr-tech/"><u>[New] In 2024, The Future Shaped by Quantum HDR Tech</u></a></li>
<li><a href="https://remote-screen-capture.techidaily.com/updated-in-2024-the-ultimate-slack-filmora-duo-for-meeting-management-excellence/"><u>[Updated] In 2024, The Ultimate Slack-Filmora Duo for Meeting Management Excellence</u></a></li>
<li><a href="https://extra-tips.techidaily.com/2024-approved-crafting-subc-from-srt-efficient-actionable-paths/"><u>2024 Approved Crafting SUBC From SRT Efficient, Actionable Paths</u></a></li>
<li><a href="https://some-guidance.techidaily.com/best-free-mkv-splitting-tool-divide-your-video-files-into-halves-or-thirds-download-now/"><u>Best FREE MKV Splitting Tool: Divide Your Video Files Into Halves or Thirds – Download Now!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/effortlessly-convert-avi-videos-to-wav-audio-on-the-web-for-free-try-movavis-expert-service-now/"><u>Effortlessly Convert AVI Videos to WAV Audio on the Web for Free - Try Movavi's Expert Service Now!</u></a></li>
<li><a href="https://program-issues.techidaily.com/1723002024009-lost-in-digital-battlefields-reboot-your-link-with-blizzard-gaming-servers-now/"><u>Lost in Digital Battlefields? Reboot Your Link with Blizzard Gaming Servers Now!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/reinventer-votre-contenu-au-format-mp4-gratuitement-guide-simple-avec-movavi/"><u>Réinventer Votre Contenu Au Format MP4 Gratuitement: Guide Simple Avec Movavi!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/top-19-best-free-video-editing-software-replace-wondershare-filmora/"><u>Top 19 Best Free Video Editing Software: Replace Wondershare Filmora</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/ultimate-guide-shrink-your-mov-videos-with-ease-windows-and-mac-tips-and-free-web-tools/"><u>Ultimate Guide: Shrink Your MOV Videos with Ease - Windows & Mac Tips and Free Web Tools</u></a></li>
<li><a href="https://buynow-help.techidaily.com/unveiling-the-microsoft-surface-go-how-this-cost-effective-tablet-balances-utility-and-confusion/"><u>Unveiling the Microsoft Surface Go: How This Cost-Effective Tablet Balances Utility and Confusion</u></a></li>
</ul></div>

