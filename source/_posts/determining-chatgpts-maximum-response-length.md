---
title: Determining ChatGPT’s Maximum Response Length
date: 2024-09-28T23:53:07.379Z
updated: 2024-10-03T19:17:26.195Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Determining ChatGPT’s Maximum Response Length
excerpt: This Article Describes Determining ChatGPT’s Maximum Response Length
thumbnail: https://thmb.techidaily.com/92e9b29713cc88b11300b903399854331375d2de8a951965b47ae1bc4c0fa3c6.jpg
---

## Determining ChatGPT’s Maximum Response Length

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

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2135416/19272" target="_top" id="2135416">
  <img src="//a.impactradius-go.com/display-ad/19272-2135416" border="0" alt="https://techidaily.com" width="336" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135416/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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

<!-- affiliate ads begin -->
<a href="https://ephamedtechinc.pxf.io/c/5597632/2137224/26400" target="_top" id="2137224">
  <img src="//a.impactradius-go.com/display-ad/26400-2137224" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://ephamedtechinc.pxf.io/i/5597632/2137224/26400" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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
<a href="https://aligracehair.sjv.io/c/5597632/2135398/19272" target="_top" id="2135398">
  <img src="//a.impactradius-go.com/display-ad/19272-2135398" border="0" alt="https://techidaily.com" width="250" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135398/19272" style="position:absolute;visibility:hidden;" border="0" />
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
<a href="https://dhgate.sjv.io/c/5597632/2106658/12108" target="_top" id="2106658">
  <img src="//a.impactradius-go.com/display-ad/12108-2106658" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://dhgate.sjv.io/i/5597632/2106658/12108" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

## How to Get Longer Responses From ChatGPT

 Once you understand that there is a "hidden limit" to ChatGPT's responses, there are some simple ways to help you get more complete responses.

1. **Ask ChatGPT to Continue:** If ChatGPT stops partway through an answer, then one option is to simply ask it to continue. In the example below, we typed "Go on," and it added another two hundred words to the response.  
![Screenshot of ChatGPT being prompted to continue](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/screenshot-of-chatgpt-being-prompted-to-continue.jpg)
2. **Break your question into smaller sections:** For instance, we asked it several times to write an essay on the impact of AI on society. One option here is to ask it to bullet-point some topics for an essay on AI, then use the supplied bullet points as individual prompts.  
![Screenshot of ChatGPT response to AI Bullet points](https://static1.makeuseofimages.com/wordpress/wp-content/uploads/2023/03/screenshot-of-chatgpt-response-to-ai-bullet-points.jpg)
3. **Use the Regenerate option:** While this might throw up the same error, with nothing to lose, it is always worth a shot.

<!-- affiliate ads begin -->
<a href="https://appsumo.8odi.net/c/5597632/2082533/7443" target="_top" id="2082533">
  <img src="//a.impactradius-go.com/display-ad/7443-2082533" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://appsumo.8odi.net/i/5597632/2082533/7443" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2135404/19272" target="_top" id="2135404">
  <img src="//a.impactradius-go.com/display-ad/19272-2135404" border="0" alt="https://techidaily.com" width="468" height="60"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135404/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2135396/19272" target="_top" id="2135396">
  <img src="//a.impactradius-go.com/display-ad/19272-2135396" border="0" alt="https://techidaily.com" width="160" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135396/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

 The sentence "How many words have I typed" and answer "6" were "tokenized" to a value of nine tokens. This is consistent with OpenAI's "rule of thumb" that one token is equivalent to around three-quarters of a word.

 Here's where things get a little bit tricky. OpenAI's GPT models come in varying token lengths. The standard GPT-4 model that comes with your ChatGPT Plus subscription offers anywhere between 4k and 8k token context length. OpenAI also provides an extended 32k token context length GPT-4 model. The GPT-3.5 series offers even more token variety. There are 4k, 8k, and 16k GPT-3.5 models. However, not all these models are publicly available.

 We used the base GPT-3.5 and supposed GPT-4 8k models for this test. We say "supposed" because the 8k tag didn't check out when we ran a context window test. And then there's the fact that there's no confirmation from official sources that the GPT-4 model at chat.openai.com is an 8k model.

 The base GPT 3.5 4k model is supposed to restrict user questions and replies to 4,097 tokens. Similarly, the GPT-4 8k model is supposed to deliver 8,192 tokens. By OpenAI's reckoning, this equates to about 3,000 words for the GPT-3.5 and around 5,000 to 6,000 words for the GPT-4 8k tokens. But wait a minute. With an approximate 3,000 to 6,000 words capacity on either model, why wasn't ChatGPT able to deliver a 2,500-word or even 1,500-word article when we requested? Why are ChatGPT responses much less than their advertised token count or context length?

<!-- affiliate ads begin -->
<a href="https://wigfever.sjv.io/c/5597632/2014849/22899" target="_top" id="2014849">
  <img src="//a.impactradius-go.com/display-ad/22899-2014849" border="0" alt="https://techidaily.com" width="728" height="90"/>
</a>
<img height="0" width="0" src="https://wigfever.sjv.io/i/5597632/2014849/22899" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

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
<li><a href="https://fox-access.techidaily.com/updated-explore-the-finest-iosdesktop-video-to-file-converters-for-2024/"><u>[Updated] Explore the Finest iOS/Desktop Video to File Converters for 2024</u></a></li>
<li><a href="https://youtube-docs.techidaily.com/ed-in-2024-decoding-youtubes-economic-strategy-the-rise-of-short-videos/"><u>[Updated] In 2024, Decoding YouTube’s Economic Strategy The Rise of Short Videos</u></a></li>
<li><a href="https://extra-skills.techidaily.com/updated-pioneering-tomorrow-visionary-developments-in-vr/"><u>[Updated] Pioneering Tomorrow Visionary Developments in VR</u></a></li>
<li><a href="https://desktop-recording.techidaily.com/2024-approved-essential-windows-8-tips-record-your-screen/"><u>2024 Approved Essential Windows 8 Tips Record Your Screen</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/crafting-content-like-a-pro-avoid-these-four-slip-ups-using-chatgpt/"><u>Crafting Content Like a Pro: Avoid These Four Slip-Ups Using ChatGPT</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/crafting-powerful-speeches-chatgpts-guide/"><u>Crafting Powerful Speeches: ChatGPT's Guide</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/discovering-day-to-day-chatgpt-integrations/"><u>Discovering Day-to-Day ChatGPT Integrations</u></a></li>
<li><a href="https://visual-screen-recording.techidaily.com/effective-group-meetings-googles-top-solutions-4/"><u>Effective Group Meetings Google's Top Solutions (#4)</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/harnessing-ai-7-tricks-that-work-wonders/"><u>Harnessing AI: 7 Tricks That Work Wonders</u></a></li>
<li><a href="https://iphone-unlock.techidaily.com/how-to-remove-passcode-from-apple-iphone-15-complete-guide-drfone-by-drfone-ios/"><u>How To Remove Passcode From Apple iPhone 15? Complete Guide | Dr.fone</u></a></li>
<li><a href="https://activate-lock.techidaily.com/how-to-unlock-icloud-lock-on-your-apple-iphone-12-mini-and-ipad-by-drfone-ios/"><u>How to Unlock iCloud lock on your Apple iPhone 12 mini and iPad?</u></a></li>
<li><a href="https://review-topics.techidaily.com/how-to-update-iphone-se-2022-to-the-latest-iosipados-version-drfone-by-drfone-ios-system-repair-ios-system-repair/"><u>How to Update iPhone SE (2022) to the Latest iOS/iPadOS Version? | Dr.fone</u></a></li>
<li><a href="https://youtube-stream.techidaily.com/in-2024-should-you-pay-for-unlimited-youtube/"><u>In 2024, Should You Pay for Unlimited YouTube?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/navigating-auto-gpt-installation-overcoming-6-frequent-hurdles/"><u>Navigating Auto-GPT Installation: Overcoming 6 Frequent Hurdles</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/nexus-of-innovation-chatai-plus-cryptocurrency/"><u>Nexus of Innovation: ChatAI + Cryptocurrency</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/simple-chatgpt-versus-browsing-enhanced-gpt-functions/"><u>Simple ChatGPT Versus Browsing-Enhanced GPT Functions</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/the-evolutionary-tale-of-openais-language-powers-gpt-1-to-4/"><u>The Evolutionary Tale of OpenAI's Language Powers (GPT-1 to 4)</u></a></li>
</ul></div>

