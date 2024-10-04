---
title: Understanding the Length Restrictions of AI Outputs
date: 2024-10-02T17:34:14.365Z
updated: 2024-10-03T18:16:19.249Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Understanding the Length Restrictions of AI Outputs
excerpt: This Article Describes Understanding the Length Restrictions of AI Outputs
thumbnail: https://thmb.techidaily.com/bc22e110eacd1143aa0bdeeb05b2f88960a893ae5ff7866bf9fbfc4c2eddab7b.jpg
---

## Understanding the Length Restrictions of AI Outputs

>  Disclaimer: This post includes affiliate links
>
>  If you click on a link and make a purchase, I may receive a commission at no extra cost to you.
>

### Key Takeaways

* ChatGPT responses are not limitless in length, despite the initial claim. There are hidden limits determined by the token system, past conversations, and system demands.
* The token system used by ChatGPT considers both the length of queries and answers. The available token lengths vary depending on the GPT model used.
* To get longer responses from ChatGPT, you can ask it to continue, break your question into smaller sections, use the regenerate option, specify a word count limit, or start a new conversation. These techniques can help you work around the unofficial limits and receive more complete answers.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 ChatGPT is big news. But how big are the responses you get from this all-purpose chatbot?

 Establishing this is not as simple as you may think. For starters, ask ChatGPT this question, and you will be assured that there are no set limits to the length of its responses.

 However, as we uncover here, it isn't that straightforward. There are hidden limits to the length of a ChatGPT response, but there are also some nifty and simple workarounds to help you get longer answers.

## How Does ChatGPT Determine the Length of a Response?

[How ChatGPT works is complex](https://www.makeuseof.com/how-does-chatgpt-work/), and the response length varies depending on what is being asked and the level of detail requested. As the next screenshot shows, ChatGPT claims there are no strict limits.

![Screenshot of ChatGPT Declaring No Limits](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/screenshot-of-chatgpt-declaring-no-limits.jpg)

 Of course, asking ChatGPT about itself isn't a good idea since it isn't typically objective about its abilities or has limited information. So, we ran some tests to determine the length limits of ChatGPT responses. We asked the chatbot to write a 5000-word article on the history of the FIFA World Cup. ChatGPT's assessment of itself differed from the results we found.

![Asking ChatGPT to write 5000 words article](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/asking-chatgpt-to-write-5000-words-article.jpg)

 ChatGPT is a powerful tool. But maybe 5,000 words was asking a bit too much, so I asked for 2,500 words instead.

![Asking ChatGPT to write 2500 words article](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/asking-chatgpt-to-write-2500-words-article.jpg)

 ChatGPT still said it wasn't able to fulfill the request. We worked down to 1,000 words before the chatbot produced the article. But there was another problem: no matter how many times we tried, ChatGPT couldn't produce 1,000 words on the subject. But why? What's limiting the chatbot's ability to produce longer replies?

 Part of the answer as to why this happens lies in something called the token system.

### What Is the Token System ChatGPT Uses?

 When you ask ChatGPT a question, the length of the replies it can provide depends on a token system. Rather than a simple word count to determine the length of both queries and answers, ChatGPT uses this system. Notice something? The length of both "queries and answers" is taken into consideration. The token system breaks down each input and output into a series of tokens to classify the request and response size.

 While word count does play a part in this, it isn't the whole story. For instance, the example below was entered into [OpenAI's Tokenizer tool](https://platform.openai.com/tokenizer).

![Screenshot of ChatGPT Tokenizer tool test](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/screenshot-of-chatgpt-tokenizer-tool-test.jpg)

 The sentence "How many words have I typed" and answer "6" were "tokenized" to a value of nine tokens. This is consistent with OpenAI's "rule of thumb" that one token is equivalent to around three-quarters of a word.

 Here's where things get a little bit tricky. OpenAI's GPT models come in varying token lengths. The standard GPT-4 model that comes with your ChatGPT Plus subscription offers anywhere between 4k and 8k token context length. OpenAI also provides an extended 32k token context length GPT-4 model. The GPT-3.5 series offers even more token variety. There are 4k, 8k, and 16k GPT-3.5 models. However, not all these models are publicly available.

 We used the base GPT-3.5 and supposed GPT-4 8k models for this test. We say "supposed" because the 8k tag didn't check out when we ran a context window test. And then there's the fact that there's no confirmation from official sources that the GPT-4 model at chat.openai.com is an 8k model.

 The base GPT 3.5 4k model is supposed to restrict user questions and replies to 4,097 tokens. Similarly, the GPT-4 8k model is supposed to deliver 8,192 tokens. By OpenAI's reckoning, this equates to about 3,000 words for the GPT-3.5 and around 5,000 to 6,000 words for the GPT-4 8k tokens. But wait a minute. With an approximate 3,000 to 6,000 words capacity on either model, why wasn't ChatGPT able to deliver a 2,500-word or even 1,500-word article when we requested? Why are ChatGPT responses much less than their advertised token count or context length?

## Why Are ChatGPT's Responses Limited?

 While token length looks straightforward and good in theory, there's more to how AI models consider these limits. There are two notable considerations.

1. **Past Conversations**: Because ChatGPT is a conversational chatbot, whenever you ask a question, the chatbot considers older conversations to stay consistent and ensure natural-sounding interactions. This means in longer conversations, older prompts and responses are invariably considered as part of the context window and end up eating your token length. So, it is not just the immediate question and replies that is considered in the context window calculation.
2. **System Demand**: [ChatGPT has quickly become one of the fastest-growing apps of all time](https://www.makeuseof.com/how-chatgpt-became-fastest-growing-app/). This has generated a huge demand for ChatGPT. To ensure everyone gets a piece of the action, 8k tokens might not always be 8k. Remember, the more tokens to process, the more demand on the system. To lessen the average demand from each user, responses are curtailed to far below the stated limits.

 To stress, this is not a fixed rule—we generated outputs that exceeded this by almost two hundred words. However, this can be considered a safe upper limit to achieve complete answers.

## How to Get Longer Responses From ChatGPT

 Once you understand that there is a "hidden limit" to ChatGPT's responses, there are some simple ways to help you get more complete responses.

1. **Ask ChatGPT to Continue:** If ChatGPT stops partway through an answer, then one option is to simply ask it to continue. In the example below, we typed "Go on," and it added another two hundred words to the response.  
![Screenshot of ChatGPT being prompted to continue](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/screenshot-of-chatgpt-being-prompted-to-continue.jpg)
2. **Break your question into smaller sections:** For instance, we asked it several times to write an essay on the impact of AI on society. One option here is to ask it to bullet-point some topics for an essay on AI, then use the supplied bullet points as individual prompts.  
![Screenshot of ChatGPT response to AI Bullet points](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/screenshot-of-chatgpt-response-to-ai-bullet-points.jpg)
3. **Use the Regenerate option:** While this might throw up the same error, with nothing to lose, it is always worth a shot.
4. **Specify an upper limit to your word count in your prompt:** The image below illustrates how this can be used to manipulate the maximum word count in an answer.  
![Screenshot of using a word limit for ChatGPT response](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/screenshot-of-using-a-word-limit-for-chatgpt-response.jpg)
5. **Start a new conversation**: starting a new conversation gives you a clean slate to work with. Remember, ChatGPT considers past prompts and responses in a conversation. Starting a new chat gives you unused context to work with.

 These tips will help you to get more complete answers from ChatGPT and work around the unofficial limit in the length of its responses.

## ChatGPT: Quality Over Quantity

 While there is no official information on the maximum length of ChatGPT responses, in practice, there are hidden constraints. The token system, influenced by past conversations and system demand, all impact how long ChatGPT's answers can be. However, by asking ChatGPT to continue, breaking questions into parts, regenerating responses, specifying word counts, and starting new chats, you can often get more complete, longer replies. Though not perfect, being aware of these unofficial limits and using the right techniques can help you get the most out of this powerful AI chatbot.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 ChatGPT is big news. But how big are the responses you get from this all-purpose chatbot?

 Establishing this is not as simple as you may think. For starters, ask ChatGPT this question, and you will be assured that there are no set limits to the length of its responses.

 However, as we uncover here, it isn't that straightforward. There are hidden limits to the length of a ChatGPT response, but there are also some nifty and simple workarounds to help you get longer answers.

## How Does ChatGPT Determine the Length of a Response?

[How ChatGPT works is complex](https://www.makeuseof.com/how-does-chatgpt-work/), and the response length varies depending on what is being asked and the level of detail requested. As the next screenshot shows, ChatGPT claims there are no strict limits.

![Screenshot of ChatGPT Declaring No Limits](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/screenshot-of-chatgpt-declaring-no-limits.jpg)

 Of course, asking ChatGPT about itself isn't a good idea since it isn't typically objective about its abilities or has limited information. So, we ran some tests to determine the length limits of ChatGPT responses. We asked the chatbot to write a 5000-word article on the history of the FIFA World Cup. ChatGPT's assessment of itself differed from the results we found.

![Asking ChatGPT to write 5000 words article](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/asking-chatgpt-to-write-5000-words-article.jpg)

 ChatGPT is a powerful tool. But maybe 5,000 words was asking a bit too much, so I asked for 2,500 words instead.

![Asking ChatGPT to write 2500 words article](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/asking-chatgpt-to-write-2500-words-article.jpg)

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2087389/7443" target="_top" id="2087389">
  <img src="//a.impactradius-go.com/display-ad/7443-2087389" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2087389/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 ChatGPT still said it wasn't able to fulfill the request. We worked down to 1,000 words before the chatbot produced the article. But there was another problem: no matter how many times we tried, ChatGPT couldn't produce 1,000 words on the subject. But why? What's limiting the chatbot's ability to produce longer replies?

 Part of the answer as to why this happens lies in something called the token system.

### What Is the Token System ChatGPT Uses?

 When you ask ChatGPT a question, the length of the replies it can provide depends on a token system. Rather than a simple word count to determine the length of both queries and answers, ChatGPT uses this system. Notice something? The length of both "queries and answers" is taken into consideration. The token system breaks down each input and output into a series of tokens to classify the request and response size.

 While word count does play a part in this, it isn't the whole story. For instance, the example below was entered into [OpenAI's Tokenizer tool](https://platform.openai.com/tokenizer).

![Screenshot of ChatGPT Tokenizer tool test](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/screenshot-of-chatgpt-tokenizer-tool-test.jpg)

 The sentence "How many words have I typed" and answer "6" were "tokenized" to a value of nine tokens. This is consistent with OpenAI's "rule of thumb" that one token is equivalent to around three-quarters of a word.

 Here's where things get a little bit tricky. OpenAI's GPT models come in varying token lengths. The standard GPT-4 model that comes with your ChatGPT Plus subscription offers anywhere between 4k and 8k token context length. OpenAI also provides an extended 32k token context length GPT-4 model. The GPT-3.5 series offers even more token variety. There are 4k, 8k, and 16k GPT-3.5 models. However, not all these models are publicly available.

 We used the base GPT-3.5 and supposed GPT-4 8k models for this test. We say "supposed" because the 8k tag didn't check out when we ran a context window test. And then there's the fact that there's no confirmation from official sources that the GPT-4 model at chat.openai.com is an 8k model.

 The base GPT 3.5 4k model is supposed to restrict user questions and replies to 4,097 tokens. Similarly, the GPT-4 8k model is supposed to deliver 8,192 tokens. By OpenAI's reckoning, this equates to about 3,000 words for the GPT-3.5 and around 5,000 to 6,000 words for the GPT-4 8k tokens. But wait a minute. With an approximate 3,000 to 6,000 words capacity on either model, why wasn't ChatGPT able to deliver a 2,500-word or even 1,500-word article when we requested? Why are ChatGPT responses much less than their advertised token count or context length?

## Why Are ChatGPT's Responses Limited?

 While token length looks straightforward and good in theory, there's more to how AI models consider these limits. There are two notable considerations.

1. **Past Conversations**: Because ChatGPT is a conversational chatbot, whenever you ask a question, the chatbot considers older conversations to stay consistent and ensure natural-sounding interactions. This means in longer conversations, older prompts and responses are invariably considered as part of the context window and end up eating your token length. So, it is not just the immediate question and replies that is considered in the context window calculation.
2. **System Demand**: [ChatGPT has quickly become one of the fastest-growing apps of all time](https://www.makeuseof.com/how-chatgpt-became-fastest-growing-app/). This has generated a huge demand for ChatGPT. To ensure everyone gets a piece of the action, 8k tokens might not always be 8k. Remember, the more tokens to process, the more demand on the system. To lessen the average demand from each user, responses are curtailed to far below the stated limits.

 To stress, this is not a fixed rule—we generated outputs that exceeded this by almost two hundred words. However, this can be considered a safe upper limit to achieve complete answers.

## How to Get Longer Responses From ChatGPT

 Once you understand that there is a "hidden limit" to ChatGPT's responses, there are some simple ways to help you get more complete responses.

1. **Ask ChatGPT to Continue:** If ChatGPT stops partway through an answer, then one option is to simply ask it to continue. In the example below, we typed "Go on," and it added another two hundred words to the response.  
![Screenshot of ChatGPT being prompted to continue](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/screenshot-of-chatgpt-being-prompted-to-continue.jpg)
2. **Break your question into smaller sections:** For instance, we asked it several times to write an essay on the impact of AI on society. One option here is to ask it to bullet-point some topics for an essay on AI, then use the supplied bullet points as individual prompts.  
![Screenshot of ChatGPT response to AI Bullet points](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/screenshot-of-chatgpt-response-to-ai-bullet-points.jpg)
3. **Use the Regenerate option:** While this might throw up the same error, with nothing to lose, it is always worth a shot.
4. **Specify an upper limit to your word count in your prompt:** The image below illustrates how this can be used to manipulate the maximum word count in an answer.  
![Screenshot of using a word limit for ChatGPT response](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/screenshot-of-using-a-word-limit-for-chatgpt-response.jpg)
5. **Start a new conversation**: starting a new conversation gives you a clean slate to work with. Remember, ChatGPT considers past prompts and responses in a conversation. Starting a new chat gives you unused context to work with.

 These tips will help you to get more complete answers from ChatGPT and work around the unofficial limit in the length of its responses.

## ChatGPT: Quality Over Quantity

 While there is no official information on the maximum length of ChatGPT responses, in practice, there are hidden constraints. The token system, influenced by past conversations and system demand, all impact how long ChatGPT's answers can be. However, by asking ChatGPT to continue, breaking questions into parts, regenerating responses, specifying word counts, and starting new chats, you can often get more complete, longer replies. Though not perfect, being aware of these unofficial limits and using the right techniques can help you get the most out of this powerful AI chatbot.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 ChatGPT is big news. But how big are the responses you get from this all-purpose chatbot?

 Establishing this is not as simple as you may think. For starters, ask ChatGPT this question, and you will be assured that there are no set limits to the length of its responses.

 However, as we uncover here, it isn't that straightforward. There are hidden limits to the length of a ChatGPT response, but there are also some nifty and simple workarounds to help you get longer answers.

## How Does ChatGPT Determine the Length of a Response?

[How ChatGPT works is complex](https://www.makeuseof.com/how-does-chatgpt-work/), and the response length varies depending on what is being asked and the level of detail requested. As the next screenshot shows, ChatGPT claims there are no strict limits.

![Screenshot of ChatGPT Declaring No Limits](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/screenshot-of-chatgpt-declaring-no-limits.jpg)

 Of course, asking ChatGPT about itself isn't a good idea since it isn't typically objective about its abilities or has limited information. So, we ran some tests to determine the length limits of ChatGPT responses. We asked the chatbot to write a 5000-word article on the history of the FIFA World Cup. ChatGPT's assessment of itself differed from the results we found.

![Asking ChatGPT to write 5000 words article](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/asking-chatgpt-to-write-5000-words-article.jpg)

 ChatGPT is a powerful tool. But maybe 5,000 words was asking a bit too much, so I asked for 2,500 words instead.

![Asking ChatGPT to write 2500 words article](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/asking-chatgpt-to-write-2500-words-article.jpg)

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2100534/7443" target="_top" id="2100534">
  <img src="//a.impactradius-go.com/display-ad/7443-2100534" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2100534/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 ChatGPT still said it wasn't able to fulfill the request. We worked down to 1,000 words before the chatbot produced the article. But there was another problem: no matter how many times we tried, ChatGPT couldn't produce 1,000 words on the subject. But why? What's limiting the chatbot's ability to produce longer replies?

 Part of the answer as to why this happens lies in something called the token system.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2068416/7443" target="_top" id="2068416">
  <img src="//a.impactradius-go.com/display-ad/7443-2068416" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2068416/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

### What Is the Token System ChatGPT Uses?

 When you ask ChatGPT a question, the length of the replies it can provide depends on a token system. Rather than a simple word count to determine the length of both queries and answers, ChatGPT uses this system. Notice something? The length of both "queries and answers" is taken into consideration. The token system breaks down each input and output into a series of tokens to classify the request and response size.

 While word count does play a part in this, it isn't the whole story. For instance, the example below was entered into [OpenAI's Tokenizer tool](https://platform.openai.com/tokenizer).

![Screenshot of ChatGPT Tokenizer tool test](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/screenshot-of-chatgpt-tokenizer-tool-test.jpg)

 The sentence "How many words have I typed" and answer "6" were "tokenized" to a value of nine tokens. This is consistent with OpenAI's "rule of thumb" that one token is equivalent to around three-quarters of a word.

 Here's where things get a little bit tricky. OpenAI's GPT models come in varying token lengths. The standard GPT-4 model that comes with your ChatGPT Plus subscription offers anywhere between 4k and 8k token context length. OpenAI also provides an extended 32k token context length GPT-4 model. The GPT-3.5 series offers even more token variety. There are 4k, 8k, and 16k GPT-3.5 models. However, not all these models are publicly available.

 We used the base GPT-3.5 and supposed GPT-4 8k models for this test. We say "supposed" because the 8k tag didn't check out when we ran a context window test. And then there's the fact that there's no confirmation from official sources that the GPT-4 model at chat.openai.com is an 8k model.

 The base GPT 3.5 4k model is supposed to restrict user questions and replies to 4,097 tokens. Similarly, the GPT-4 8k model is supposed to deliver 8,192 tokens. By OpenAI's reckoning, this equates to about 3,000 words for the GPT-3.5 and around 5,000 to 6,000 words for the GPT-4 8k tokens. But wait a minute. With an approximate 3,000 to 6,000 words capacity on either model, why wasn't ChatGPT able to deliver a 2,500-word or even 1,500-word article when we requested? Why are ChatGPT responses much less than their advertised token count or context length?

## Why Are ChatGPT's Responses Limited?

 While token length looks straightforward and good in theory, there's more to how AI models consider these limits. There are two notable considerations.

1. **Past Conversations**: Because ChatGPT is a conversational chatbot, whenever you ask a question, the chatbot considers older conversations to stay consistent and ensure natural-sounding interactions. This means in longer conversations, older prompts and responses are invariably considered as part of the context window and end up eating your token length. So, it is not just the immediate question and replies that is considered in the context window calculation.
2. **System Demand**: [ChatGPT has quickly become one of the fastest-growing apps of all time](https://www.makeuseof.com/how-chatgpt-became-fastest-growing-app/). This has generated a huge demand for ChatGPT. To ensure everyone gets a piece of the action, 8k tokens might not always be 8k. Remember, the more tokens to process, the more demand on the system. To lessen the average demand from each user, responses are curtailed to far below the stated limits.

 To stress, this is not a fixed rule—we generated outputs that exceeded this by almost two hundred words. However, this can be considered a safe upper limit to achieve complete answers.

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/1886069/19272" target="_top" id="1886069">
  <img src="//a.impactradius-go.com/display-ad/19272-1886069" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/1886069/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

## How to Get Longer Responses From ChatGPT

 Once you understand that there is a "hidden limit" to ChatGPT's responses, there are some simple ways to help you get more complete responses.

1. **Ask ChatGPT to Continue:** If ChatGPT stops partway through an answer, then one option is to simply ask it to continue. In the example below, we typed "Go on," and it added another two hundred words to the response.  
![Screenshot of ChatGPT being prompted to continue](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/screenshot-of-chatgpt-being-prompted-to-continue.jpg)
2. **Break your question into smaller sections:** For instance, we asked it several times to write an essay on the impact of AI on society. One option here is to ask it to bullet-point some topics for an essay on AI, then use the supplied bullet points as individual prompts.  

<!-- affiliate ads begin -->
<span id="1424531">
					<video width="864" height="NaN" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1424531.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/16446-1424531">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1424531.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:540px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Flaganoo.pxf.io%2Fc%2F5597632%2F1424531%2F16446'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1424531/16446" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

![Screenshot of ChatGPT response to AI Bullet points](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/screenshot-of-chatgpt-response-to-ai-bullet-points.jpg)
3. **Use the Regenerate option:** While this might throw up the same error, with nothing to lose, it is always worth a shot.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2144297/7443" target="_top" id="2144297">
  <img src="//a.impactradius-go.com/display-ad/7443-2144297" border="0" alt="https://techidaily.com" width="600" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2144297/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

4. **Specify an upper limit to your word count in your prompt:** The image below illustrates how this can be used to manipulate the maximum word count in an answer.  
![Screenshot of using a word limit for ChatGPT response](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/screenshot-of-using-a-word-limit-for-chatgpt-response.jpg)
5. **Start a new conversation**: starting a new conversation gives you a clean slate to work with. Remember, ChatGPT considers past prompts and responses in a conversation. Starting a new chat gives you unused context to work with.

<!-- affiliate ads begin -->
<a href="https://ephamedtechinc.pxf.io/c/5597632/2136616/26400" target="_top" id="2136616">
  <img src="//a.impactradius-go.com/display-ad/26400-2136616" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://ephamedtechinc.pxf.io/i/5597632/2136616/26400" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 These tips will help you to get more complete answers from ChatGPT and work around the unofficial limit in the length of its responses.

## ChatGPT: Quality Over Quantity

 While there is no official information on the maximum length of ChatGPT responses, in practice, there are hidden constraints. The token system, influenced by past conversations and system demand, all impact how long ChatGPT's answers can be. However, by asking ChatGPT to continue, breaking questions into parts, regenerating responses, specifying word counts, and starting new chats, you can often get more complete, longer replies. Though not perfect, being aware of these unofficial limits and using the right techniques can help you get the most out of this powerful AI chatbot.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 ChatGPT is big news. But how big are the responses you get from this all-purpose chatbot?

 Establishing this is not as simple as you may think. For starters, ask ChatGPT this question, and you will be assured that there are no set limits to the length of its responses.

 However, as we uncover here, it isn't that straightforward. There are hidden limits to the length of a ChatGPT response, but there are also some nifty and simple workarounds to help you get longer answers.

## How Does ChatGPT Determine the Length of a Response?

[How ChatGPT works is complex](https://www.makeuseof.com/how-does-chatgpt-work/), and the response length varies depending on what is being asked and the level of detail requested. As the next screenshot shows, ChatGPT claims there are no strict limits.

![Screenshot of ChatGPT Declaring No Limits](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/screenshot-of-chatgpt-declaring-no-limits.jpg)

 Of course, asking ChatGPT about itself isn't a good idea since it isn't typically objective about its abilities or has limited information. So, we ran some tests to determine the length limits of ChatGPT responses. We asked the chatbot to write a 5000-word article on the history of the FIFA World Cup. ChatGPT's assessment of itself differed from the results we found.

![Asking ChatGPT to write 5000 words article](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/asking-chatgpt-to-write-5000-words-article.jpg)

 ChatGPT is a powerful tool. But maybe 5,000 words was asking a bit too much, so I asked for 2,500 words instead.

![Asking ChatGPT to write 2500 words article](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/10/asking-chatgpt-to-write-2500-words-article.jpg)

 ChatGPT still said it wasn't able to fulfill the request. We worked down to 1,000 words before the chatbot produced the article. But there was another problem: no matter how many times we tried, ChatGPT couldn't produce 1,000 words on the subject. But why? What's limiting the chatbot's ability to produce longer replies?

 Part of the answer as to why this happens lies in something called the token system.

### What Is the Token System ChatGPT Uses?

 When you ask ChatGPT a question, the length of the replies it can provide depends on a token system. Rather than a simple word count to determine the length of both queries and answers, ChatGPT uses this system. Notice something? The length of both "queries and answers" is taken into consideration. The token system breaks down each input and output into a series of tokens to classify the request and response size.

 While word count does play a part in this, it isn't the whole story. For instance, the example below was entered into [OpenAI's Tokenizer tool](https://platform.openai.com/tokenizer).

![Screenshot of ChatGPT Tokenizer tool test](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/screenshot-of-chatgpt-tokenizer-tool-test.jpg)

 The sentence "How many words have I typed" and answer "6" were "tokenized" to a value of nine tokens. This is consistent with OpenAI's "rule of thumb" that one token is equivalent to around three-quarters of a word.

 Here's where things get a little bit tricky. OpenAI's GPT models come in varying token lengths. The standard GPT-4 model that comes with your ChatGPT Plus subscription offers anywhere between 4k and 8k token context length. OpenAI also provides an extended 32k token context length GPT-4 model. The GPT-3.5 series offers even more token variety. There are 4k, 8k, and 16k GPT-3.5 models. However, not all these models are publicly available.

 We used the base GPT-3.5 and supposed GPT-4 8k models for this test. We say "supposed" because the 8k tag didn't check out when we ran a context window test. And then there's the fact that there's no confirmation from official sources that the GPT-4 model at chat.openai.com is an 8k model.

 The base GPT 3.5 4k model is supposed to restrict user questions and replies to 4,097 tokens. Similarly, the GPT-4 8k model is supposed to deliver 8,192 tokens. By OpenAI's reckoning, this equates to about 3,000 words for the GPT-3.5 and around 5,000 to 6,000 words for the GPT-4 8k tokens. But wait a minute. With an approximate 3,000 to 6,000 words capacity on either model, why wasn't ChatGPT able to deliver a 2,500-word or even 1,500-word article when we requested? Why are ChatGPT responses much less than their advertised token count or context length?

## Why Are ChatGPT's Responses Limited?

 While token length looks straightforward and good in theory, there's more to how AI models consider these limits. There are two notable considerations.

1. **Past Conversations**: Because ChatGPT is a conversational chatbot, whenever you ask a question, the chatbot considers older conversations to stay consistent and ensure natural-sounding interactions. This means in longer conversations, older prompts and responses are invariably considered as part of the context window and end up eating your token length. So, it is not just the immediate question and replies that is considered in the context window calculation.
2. **System Demand**: [ChatGPT has quickly become one of the fastest-growing apps of all time](https://www.makeuseof.com/how-chatgpt-became-fastest-growing-app/). This has generated a huge demand for ChatGPT. To ensure everyone gets a piece of the action, 8k tokens might not always be 8k. Remember, the more tokens to process, the more demand on the system. To lessen the average demand from each user, responses are curtailed to far below the stated limits.

 To stress, this is not a fixed rule—we generated outputs that exceeded this by almost two hundred words. However, this can be considered a safe upper limit to achieve complete answers.

<!-- affiliate ads begin -->
<span id="1899850">
					<video width="486" height="864" style="cursor:pointer"
           poster="//a.impactradius-go.com/display-clicktoplayimage/1899850.png"
           onclick="if(!this.playClicked){this.play();this.setAttribute('controls',true);this.playClicked=true;}">
	   <source src="//a.impactradius-go.com/display-ad/14483-1899850">
	   <img src="//a.impactradius-go.com/display-clicktoplayimage/1899850.png" style="border: none; height: 100%; width: 100%; object-fit: contain">
	</video>
	<div style="width:304px;text-align:center"><a href="javascript:window.open(decodeURIComponent('https%3A%2F%2Felectronicx.pxf.io%2Fc%2F5597632%2F1899850%2F14483'), '_blank');void(0);">Click here</a></div>
</span>
<img height="0" width="0" src="https://imp.pxf.io/i/5597632/1899850/14483" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

## How to Get Longer Responses From ChatGPT

 Once you understand that there is a "hidden limit" to ChatGPT's responses, there are some simple ways to help you get more complete responses.

1. **Ask ChatGPT to Continue:** If ChatGPT stops partway through an answer, then one option is to simply ask it to continue. In the example below, we typed "Go on," and it added another two hundred words to the response.  
![Screenshot of ChatGPT being prompted to continue](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/screenshot-of-chatgpt-being-prompted-to-continue.jpg)
2. **Break your question into smaller sections:** For instance, we asked it several times to write an essay on the impact of AI on society. One option here is to ask it to bullet-point some topics for an essay on AI, then use the supplied bullet points as individual prompts.  
![Screenshot of ChatGPT response to AI Bullet points](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/screenshot-of-chatgpt-response-to-ai-bullet-points.jpg)
3. **Use the Regenerate option:** While this might throw up the same error, with nothing to lose, it is always worth a shot.
4. **Specify an upper limit to your word count in your prompt:** The image below illustrates how this can be used to manipulate the maximum word count in an answer.  
![Screenshot of using a word limit for ChatGPT response](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/screenshot-of-using-a-word-limit-for-chatgpt-response.jpg)
5. **Start a new conversation**: starting a new conversation gives you a clean slate to work with. Remember, ChatGPT considers past prompts and responses in a conversation. Starting a new chat gives you unused context to work with.

 These tips will help you to get more complete answers from ChatGPT and work around the unofficial limit in the length of its responses.

## ChatGPT: Quality Over Quantity

 While there is no official information on the maximum length of ChatGPT responses, in practice, there are hidden constraints. The token system, influenced by past conversations and system demand, all impact how long ChatGPT's answers can be. However, by asking ChatGPT to continue, breaking questions into parts, regenerating responses, specifying word counts, and starting new chats, you can often get more complete, longer replies. Though not perfect, being aware of these unofficial limits and using the right techniques can help you get the most out of this powerful AI chatbot.

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
<li><a href="https://screen-recording.techidaily.com/updated-in-2024-audio-log-analysis-guidebook/"><u>[Updated] In 2024, Audio Log Analysis Guidebook</u></a></li>
<li><a href="https://youtube-docs.techidaily.com/ed-in-2024-top-8-proven-video-growth-and-promotion-strategies/"><u>[Updated] In 2024, Top 8 Proven Video Growth & Promotion Strategies</u></a></li>
<li><a href="https://article-helps.techidaily.com/2024-approved-chucklechamber-endless-options-to-spread-smiles/"><u>2024 Approved ChuckleChamber Endless Options to Spread Smiles</u></a></li>
<li><a href="https://extra-support.techidaily.com/2024-approved-speedy-iphone-timelapses-made-simple/"><u>2024 Approved Speedy iPhone Timelapses Made Simple</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/aggregate-of-top-20-chatgpt-question-and-response-examples/"><u>Aggregate of Top 20 ChatGPT Question and Response Examples</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/chatgpt-just-added-a-host-of-new-features-here-are-the-ones-youll-care-about/"><u>ChatGPT Just Added a Host of New Features: Here Are the Ones You'll Care About</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/connecting-with-ai-through-quoras-poe-routes/"><u>Connecting with AI Through Quora's POE Routes</u></a></li>
<li><a href="https://extra-information.techidaily.com/craft-crisp-visuals-with-picart-background-sweep-for-2024/"><u>Craft Crisp Visuals with PicArt Background Sweep for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/deciphering-ais-future-the-impact-of-forefront-and-chatgpt/"><u>Deciphering AI's Future: The Impact of Forefront and ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/discounted-devices-and-data-protection-strategies/"><u>Discounted Devices and Data Protection Strategies</u></a></li>
<li><a href="https://android-location-track.techidaily.com/how-to-track-whatsapp-messages-on-lava-blaze-pro-5g-without-them-knowing-drfone-by-drfone-virtual-android/"><u>How to Track WhatsApp Messages on Lava Blaze Pro 5G Without Them Knowing? | Dr.fone</u></a></li>
<li><a href="https://apple-account.techidaily.com/in-2024-how-to-change-credit-card-on-your-apple-iphone-14-pro-apple-id-and-apple-pay-by-drfone-ios/"><u>In 2024, How to Change Credit Card on Your Apple iPhone 14 Pro Apple ID and Apple Pay</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mastering-corporate-communication-with-gpt/"><u>Mastering Corporate Communication with GPT</u></a></li>
<li><a href="https://activate-lock.techidaily.com/new-guide-how-to-check-icloud-activation-lock-status-on-your-iphone-14-pro-max-by-drfone-ios/"><u>New Guide How To Check iCloud Activation Lock Status On Your iPhone 14 Pro Max</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/securing-web-experience-with-proton-vpn-extension/"><u>Securing Web Experience with Proton VPN Extension</u></a></li>
<li><a href="https://win-dash.techidaily.com/step-by-step-guide-computing-loan-payments-and-interest-rates-using-excel/"><u>Step-by-Step Guide: Computing Loan Payments and Interest Rates Using Excel</u></a></li>
</ul></div>

