---
title: Shield Site From Web-Scouring AIs
date: 2024-08-18T09:59:51.461Z
updated: 2024-08-19T09:59:51.461Z
tags:
  - chatgpt
  - open-ai
categories:
  - openAI
  - chatgpt
description: This Article Describes Shield Site From Web-Scouring AIs
excerpt: This Article Describes Shield Site From Web-Scouring AIs
thumbnail: https://thmb.techidaily.com/8d7927945f03c1a6cf48bac233c269180a3c469aaa2f85169e12252b9874460a.png
---

## Shield Site From Web-Scouring AIs

 While users love ChatGPT for the sheer amount of information that it currently holds, the same can't be said about website owners.

**MUO VIDEO OF THE DAY**

**SCROLL TO CONTINUE WITH CONTENT**

 OpenAI's ChatGPT uses crawlers to scrape websites, but if you're a website owner, and you don't want OpenAI's crawler to access your website, here are a few things that you can do to prevent it.

## How Does OpenAI Crawling Work?

 A [web crawler](https://www.makeuseof.com/what-is-a-web-crawlerspider-and-how-does-it-work/) (also known as a spider or a search engine bot) is an automated program that scans the internet for information. It then compiles that information in a way that's easy for your search engine to access it.

 Web crawlers index every page of every relevant URL, usually focusing on websites that are more relevant to your search queries. For example, let's assume you're googling a particular Windows error. The web crawler within your search engine will scan all the URLs from websites that it deems more authoritative on the topic of Windows errors.

 OpenAI's web crawler is called GPTBot, and according to [OpenAI's documentation](https://platform.openai.com/docs/gptbot), giving GPTBot access to your website can help train the AI model to become safer, and more accurate, and it can even help expand the AI model's capabilities.

## How to Prevent OpenAI From Crawling Your Website

 Like most other web crawlers, GPTBot can be blocked from accessing your website by modifying the website's **robots.txt** protocol (also known as the robots exclusion protocol). This .txt file is hosted on the website's server, and it controls how web crawlers and other automated programs behave on your website.

 Here's a short list of what the **robot.txt** file can do:

* It can completely block GPTBot from accessing the website.
* It can block only certain pages from a URL from being accessed by GPTBot.
* It can tell GPTBot which links it can follow, and which it cannot.

 Here's how to control what GPTBot can do on your website:

<!-- affiliate ads begin -->
<a href="https://dhgate.sjv.io/c/5597632/1678785/12108" target="_top" id="1678785"><img src="//a.impactradius-go.com/display-ad/12108-1678785" border="0" alt="" width="300" height="250"/></a>
<!-- affiliate ads end -->
### Completely Block GPTBot From Accessing Your Website

1. [Set up the robot.txt file](https://www.makeuseof.com/tag/how-to-correctly-set-up-robots-txt/), and then edit it with any text editing tool.
2. Add the GPTBot to your site’s **robots.txt** as follows:

`User-agent: GPTBot  
Disallow: /`

<!-- affiliate ads begin -->
<a href="https://homestyler.sjv.io/c/5597632/2044747/22993" target="_top" id="2044747"><img src="//a.impactradius-go.com/display-ad/22993-2044747" border="0" alt="" width="300" height="250"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/2044747/22993" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
### Block Only Certain Pages From Being Accessed by GPTBot

1. Set up the **robot.txt** file, and then edit it with your preferred text editing tool.
2. Add the GPTBot to your site’s **robots.txt** as follows:

`User-agent: GPTBot  
Allow: /directory-1/  
Disallow: /directory-2/`

 However, keep in mind that changing the **robot.txt** file is not a retroactive solution, and any information that GPTBot may have already gathered from your website will not be recoverable.

<!-- affiliate ads begin -->
<a href="https://modlily.sjv.io/c/5597632/1997817/17059" target="_top" id="1997817"><img src="//a.impactradius-go.com/display-ad/17059-1997817" border="0" alt="" width="300" height="250"/></a><img height="0" width="0" src="https://imp.pxf.io/i/5597632/1997817/17059" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->
## OpenAI Allows Website Owners to Opt-Out From Crawling

 Ever since crawlers have been used to train AI models, website owners have been looking for ways to keep their data private.

 Some fear that AI models are basically stealing their work, even attributing fewer website visits to the fact that now users get their information without ever having to visit their websites.

 All in all, whether you want to completely block AI chatbots from scanning your websites is completely your choice.

**SCROLL TO CONTINUE WITH CONTENT**

 OpenAI's ChatGPT uses crawlers to scrape websites, but if you're a website owner, and you don't want OpenAI's crawler to access your website, here are a few things that you can do to prevent it.


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


