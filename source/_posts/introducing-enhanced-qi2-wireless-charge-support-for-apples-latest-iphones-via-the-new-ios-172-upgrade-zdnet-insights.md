---
title: Introducing Enhanced Qi2 Wireless Charge Support for Apple's Latest iPhones via the New iOS 17.2 Upgrade - ZDNet Insights
date: 2024-12-14T17:29:58.019Z
updated: 2024-12-22T07:13:26.255Z
tags:
  - apple
categories:
  - tech
thumbnail: https://www.zdnet.com/topic/apple/    https://www.zdnet.com/a/img/resize/71d813eb2b2863bb1128c63817820f8d43561e4b/2023/03/08/a8562d5b-e8e3-47da-8117-0b4754ddb39b/yellow-iphone-14-plus-4.jpg?width=170&height=96&fit=crop&auto=webp
---

## Apple's High-Cost Plan Limits AI Upgrades to New iPhones, Leaving Older Models in the Dust - Insights

![iPhone 13 at the Apple Store](https://www.zdnet.com/a/img/resize/fbfed4a2dd07fa0757458d10ad780941f10086e7/2022/09/08/2ea29ae7-298e-4127-a6f9-189e2f77f492/iphone-13-at-apple-store.jpg?auto=webp&precrop=2047,1150,x0,y216&width=1280)

Jason Hiner/ZDNET

During [WWDC 2024](https://www.zdnet.com/article/live-updates-everything-apple-announced-at-wwdc-2024-including-ios-18-siri-ai-more/), Apple unveiled "[Apple Intelligence](https://www.zdnet.com/article/what-is-apple-intelligence-how-it-works-with-on-device-and-cloud-based-ai/)," which incorporates advanced AI capabilities throughout its ecosystem. However, these features are only available on high-end devices such as the [iPhone 15 Pro](https://www.zdnet.com/article/iphone-15-pro-review/), [iPad Pro](https://www.zdnet.com/article/ipad-pro-2024-review/) with M-series chips, and [Macs](https://www.zdnet.com/article/m3-macbook-air-review/) running on Apple Silicon. 

**Also: [Apple staged the AI comeback we've been hoping for - but here's where it still needs work](https://www.zdnet.com/article/apple-staged-the-ai-comeback-weve-been-hoping-for-but-heres-where-it-still-needs-work/)**

Why didn't Apple roll these features out to the entry-level iPhone 15 and earlier models? Although there may be other reasons why the company chose not to do so, the decision is almost certainly influenced by the substantial costs and infrastructure challenges involved in large-scale [AI](https://www.zdnet.com/article/what-is-ai-heres-everything-you-need-to-know-about-artificial-intelligence/) implementation.

#### Newsletters

ZDNET Tech Today

ZDNET's Tech Today newsletter is a daily briefing of the newest, most talked about stories, five days a week.

 Subscribe

[See all](https://www.zdnet.com/newsletters/)

>  Disclaimer: This post includes affiliate links
>
>  If you click on a link and make a purchase, I may receive a commission at no extra cost to you.
>

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/rdNq2Sp031s?si=3FcJa3dQLraUDHKv" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## The cost of GPU processing

Advanced AI features require substantial computational power, typically provided by high-performance GPUs. For instance, [NVIDIA's MGX with GH 200 and Grace Hopper superchip](https://www.nvidia.com/en-us/data-center/grace-hopper-superchip/) designed for AI training, inference, 5G, and HPC cost around $65,000 each. Deploying these servers regionally to support lower-end devices would be prohibitively expensive. Apple would easily need thousands of these units to support its entire user base, resulting in astronomical costs likely passed on to consumers through service fees.

**Also: [Apple partners with OpenAI to bring ChatGPT to iOS, iPadOS, and MacOS](https://www.zdnet.com/article/apple-announces-new-openai-iphone-features-at-wwdc/)**

Even [major AI service providers](https://www.zdnet.com/article/best-ai-chatbot/) such as OpenAI, Microsoft, and Google encounter challenges in offering dependable and quick access to LLM and Generative AI models to the general public without downtime and overcommitting resources. The shortage and cost of GPU-enabled servers make these issues worse. To maintain the rapid response times expected by its customers, Apple will need to invest substantially in servers, data centers, and edge infrastructure -- an infrastructure level it likely does not currently possess.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/hXIq2G0nShk?si=5Z4Fwv7ZB6oKWsdd" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## Apple's approach to Private Cloud Compute (PCC)

For the initial rollout of Apple Intelligence, the company has chosen a hybrid approach to balance cost and performance, combining on-device processing with [Private Cloud Compute](https://www.zdnet.com/article/heres-how-apples-keeping-your-cloud-processed-ai-data-safe-and-why-it-matters/) (PCC). On-device processing utilizes the A17 Pro chip in the iPhone 15 Pro line and the M-series chips in iPads and Macs to enhance security and privacy. For more demanding tasks, PCC allows cloud operations while maintaining user privacy. PCC is designed with custom Apple silicon and a robust operating system to ensure personal data security and prevent unauthorized access.

**Also: [Here's how Apple's keeping your cloud-processed AI data safe (and why it matters)](https://www.zdnet.com/article/heres-how-apples-keeping-your-cloud-processed-ai-data-safe-and-why-it-matters/)**

Apple is currently focused on rolling out its [Generative AI services](https://www.zdnet.com/article/apple-unveils-on-device-ai-image-generator-for-iphone-ipad-and-mac/) to high-end devices as part of the initial phase of Apple Intelligence deployment. This allows Apple to enhance its AI capabilities and infrastructure before expanding to a wider range of devices. To bring Apple Intelligence to the rest of its ecosystem, the company will likely deploy AI-accelerated server appliances at the edge, enabling less capable devices to benefit from advanced AI features. However, this infrastructure is not yet ready for large-scale deployment, as Apple's shift towards AI development is still recent.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/slm2NjVPNtk?si=9ow6g1ucmf0TnT4T" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## The challenges of edge computing

[Edge computing](https://www.zdnet.com/article/what-are-5g-and-edge-computing-and-why-should-you-care/), which involves processing data closer to where it is generated rather than relying solely on centralized data centers, could significantly enhance performance and reduce latency. However, deploying edge computing infrastructure is complex and costly, requiring robust hardware and software solutions to ensure seamless integration and security. Apple is known for its meticulous approach to hardware and software development, and the company is likely still testing and refining its edge computing solutions before rolling them out at scale.

**Also: [Make room for RAG: How Gen AI's balance of power is shifting](https://www.zdnet.com/article/make-room-for-rag-how-gen-ais-balance-of-power-is-shifting/)**

While NVIDIA is a major player in the GPU server space, others include traditional x86 Intel-based and Arm-based server providers like Qualcomm and Ampere. These servers can also use NVIDIA GPUs, but Apple likely wants to control the integration with its operating system and silicon to deploy AI computing. Additionally, the supply chain from NVIDIA or any other HPC server vendor is likely insufficient to meet Apple's large-scale deployment requirements.

As reported by _The Register_, Apple is [developing its own AI servers](https://www.theregister.com/2024/06/11/apple%5Fbuilt%5Fai%5Fcloud%5Fservers%5Fos/), which are expected to be more cost-effective and better integrated with its ecosystem. These servers are currently being tested in data centers for foundation model use, and a broader rollout is anticipated in 2025\. This phased approach ensures Apple can maintain high privacy, security, and user experience standards while gradually expanding its AI capabilities across its device lineup.

<!-- affiliate ads begin -->
<iframe width="560" height="315" src="https://www.youtube.com/embed/KKFdFHaVIJg?si=x2vLw7ty3FtHX-9T" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
<!-- affiliate ads end -->

## Broader implications for IoT and other devices

Apple's decision to limit Apple Intelligence to high-end models is driven by the significant cost and infrastructure challenges associated with deploying AI at scale, allowing the company to ensure a smooth and secure user experience while laying the groundwork for future expansions.

The need for AI-accelerated servers isn't just about [older phones](https://www.zdnet.com/article/best-phone/) and lower-end devices. Apple's IoT products, like the Apple Watch, Apple TV, and HomePod, which lack the computational power for on-device AI, would also benefit from such infrastructure. These devices will unlikely handle on-device AI computation shortly, making cloud and edge solutions even more critical.

**Also: [Here's every iPhone model that will support Apple's new AI features (for now)](https://www.zdnet.com/article/heres-every-iphone-model-that-will-support-apples-upcoming-ai-features-for-now/)**

As Apple introduces Apple Intelligence, users with older or non-Pro models may feel left out. Clear communication from Apple regarding the phased rollout strategy and plans for broader deployment will be important in managing user expectations.

As Apple continues developing its AI infrastructure, including potential edge computing solutions, we expect that a broader rollout of Apple Intelligence will be deployed in the coming years. This phased approach ensures that Apple can maintain its high privacy, security, and user experience standards while gradually expanding its AI capabilities across its device lineup.

#### Apple

[iPhone 16 Pro upgrade: If you have a 3 year-old iPhone, here are all the new features you'll get](https://www.zdnet.com/article/iphone-16-pro-and-pro-max-hands-on/ "iPhone 16 Pro upgrade: If you have a 3 year-old iPhone, here are all the new features you'll get")

[My biggest regret with upgrading my iPhone to iOS 18 (and I'm not alone)](https://www.zdnet.com/article/my-biggest-regret-with-upgrading-my-iphone-to-ios-18-and-im-not-alone/ "My biggest regret with upgrading my iPhone to iOS 18 (and I'm not alone)")

[We've used every iPhone 16 model and here's our best buying advice for 2024](https://www.zdnet.com/article/iphone-16-pro-max-buying-advice-2024/ "We've used every iPhone 16 model and here's our best buying advice for 2024")

[6 iOS 18 settings I changed immediately - and why you should too](https://www.zdnet.com/article/6-ios-18-settings-i-changed-immediately-and-why-you-should-too/ "6 iOS 18 settings I changed immediately - and why you should too")

* [iPhone 16 Pro upgrade: If you have a 3 year-old iPhone, here are all the new features you'll get](https://www.zdnet.com/article/iphone-16-pro-and-pro-max-hands-on/ "iPhone 16 Pro upgrade: If you have a 3 year-old iPhone, here are all the new features you'll get")
* [My biggest regret with upgrading my iPhone to iOS 18 (and I'm not alone)](https://www.zdnet.com/article/my-biggest-regret-with-upgrading-my-iphone-to-ios-18-and-im-not-alone/ "My biggest regret with upgrading my iPhone to iOS 18 (and I'm not alone)")
* [We've used every iPhone 16 model and here's our best buying advice for 2024](https://www.zdnet.com/article/iphone-16-pro-max-buying-advice-2024/ "We've used every iPhone 16 model and here's our best buying advice for 2024")
* [6 iOS 18 settings I changed immediately - and why you should too](https://www.zdnet.com/article/6-ios-18-settings-i-changed-immediately-and-why-you-should-too/ "6 iOS 18 settings I changed immediately - and why you should too")

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
<li><a href="https://vimeo-videos.techidaily.com/new-2024-approved-elevating-vimeo-video-speed/"><u>[New] 2024 Approved Elevating Vimeo Video Speed</u></a></li>
<li><a href="https://article-tips.techidaily.com/new-unlocking-the-potential-of-slug-line-formats-in-screenplays-for-2024/"><u>[New] Unlocking the Potential of Slug Line Formats in Screenplays for 2024</u></a></li>
<li><a href="https://video-capture.techidaily.com/updated-streamlabs-vs-obs-which-livestream-tool-reigns-supreme-for-2024/"><u>[Updated] Streamlabs Vs. OBS Which Livestream Tool Reigns Supreme for 2024</u></a></li>
<li><a href="https://twitter-videos.techidaily.com/2023-trend-analysis-twitters-top-video-shares/"><u>2023 Trend Analysis Twitter's Top Video Shares</u></a></li>
<li><a href="https://howto.techidaily.com/7-solutions-to-fix-error-code-963-on-google-play-of-realme-narzo-60-pro-5g-drfone-by-drfone-fix-android-problems-fix-android-problems/"><u>7 Solutions to Fix Error Code 963 on Google Play Of Realme Narzo 60 Pro 5G | Dr.fone</u></a></li>
<li><a href="https://win-howtos.techidaily.com/effective-remedies-for-restoring-functionality-to-dell-laptops-dead-keys/"><u>Effective Remedies for Restoring Functionality to Dell Laptop's Dead Keys</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/enhanced-icloud-support-apple-rolls-out-major-updates-and-bug-fixes-for-windows-users-zdnet/"><u>Enhanced iCloud Support: Apple Rolls Out Major Updates and Bug Fixes for Windows Users - ZDNet</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/exclusive-deal-save-20-on-top-pick-nomadic-cellphone-accessories-and-apple-watch-straps-now-at-zdnet/"><u>Exclusive Deal: Save 20% on Top-Pick Nomadic Cellphone Accessories & Apple Watch Straps - Now at ZDNet!</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/find-your-ideal-sound-companion-a-side-by-side-review-of-apples-homepod-vs-homepod-mini-gadget-guides/"><u>Find Your Ideal Sound Companion: A Side-by-Side Review of Apple's HomePod Vs. HomePod Mini | Gadget Guides</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/guide-setting-up-multiple-network-interfaces-on-macos-for-enhanced-connectivity-options-techtalk/"><u>Guide: Setting Up Multiple Network Interfaces on macOS for Enhanced Connectivity Options | TechTalk</u></a></li>
<li><a href="https://location-social.techidaily.com/in-2024-how-to-change-your-apple-iphone-12-mini-location-on-life360-without-anyone-knowing-drfone-by-drfone-virtual-ios/"><u>In 2024, How to Change Your Apple iPhone 12 mini Location on life360 Without Anyone Knowing? | Dr.fone</u></a></li>
<li><a href="https://techtrends.techidaily.com/is-it-time-to-switch-to-an-rtx-gpu-for-your-pc/"><u>Is It Time to Switch to an RTX GPU for Your PC?</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/maximize-your-online-presence-with-gpts-4-strategies/"><u>Maximize Your Online Presence with GPT's 4 Strategies</u></a></li>
<li><a href="https://network-issues.techidaily.com/minimize-windows-10-resolution-highs/"><u>Minimize Windows 10 Resolution Highs</u></a></li>
<li><a href="https://facebook-record-videos.techidaily.com/perfect-shots-start-with-the-right-camera-and-lens-selection-for-2024/"><u>Perfect Shots Start With The Right Camera & Lens Selection for 2024</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/transform-chatgpt-today-with-these-1-9-must-have-addons/"><u>Transform ChatGPT Today with These #1-#9 Must-Have Addons</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/understanding-apples-ios-175-feature-how-it-recovers-lost-images-and-next-steps-for-users/"><u>Understanding Apple's iOS 17.5 Feature: How It Recovers Lost Images & Next Steps for Users</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/unlocking-energy-savings-activating-your-apple-watchs-battery-saving-features-explained/"><u>Unlocking Energy Savings: Activating Your Apple Watch's Battery-Saving Features Explained</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/warning-ios-15-may-cause-your-ipad-to-malfunction-essential-info-pre-installation-techinsight/"><u>Warning: IOS 15 May Cause Your iPad to Malfunction - Essential Info Pre-Installation | TechInsight</u></a></li>
</ul></div>

