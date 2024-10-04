---
title: "Master Multi-Operating Systems with MacBook: Run Ubuntu in XCode and Expand Your Tools Arsenal | Guides by ZDNET"
date: 2024-09-27T22:02:20.305Z
updated: 2024-10-03T18:07:11.894Z
tags:
  - apple
categories:
  - tech
thumbnail: https://thmb.techidaily.com/cd3d2360a2d4ccd17e303566ba964ef54de4b2742b9a5d3bf951667fe61ff2f5.jpg
---

## Master Multi-Operating Systems with MacBook: Run Ubuntu in XCode and Expand Your Tools Arsenal | Guides

![xcode-download](https://www.zdnet.com/a/img/resize/72daf9c10a8cbb72018f54fd48d893e5c1fdc697/2024/02/20/72eff26e-8b49-4c53-8f95-e123371d2227/xcode-download.jpg?auto=webp&width=1280)

Screenshot by David Gewirtz/ZDNET

So, you want to install Linux on a Mac? Well, there's more than one way to get that done. Compared to what I'm going to show you below, there's a somewhat easier set of steps that my colleague [Adrian Kingsley-Hughes ran through](https://www.zdnet.com/article/how-to-install-kali-linux-on-apple-silicon-macs/) using an installer on the App Store and Kali Linux.

**Also: [How to install Ubuntu Linux (It's easy!)](https://www.zdnet.com/article/how-to-install-ubuntu-linux/)**

But I'm going full geek. Together, we're going to use Xcode and build our own sample app, which we'll then use to install the full distribution of the [latest Ubuntu release](https://www.zdnet.com/article/ubuntu-desktop-23-10-arrives-a-glimpse-into-ubuntu-linuxs-future/), Noble Numbat.

Once you've done this, you will have considerable bragging rights. There's a lot to cover, so let's dig in. 

>  Disclaimer: This post includes affiliate links
>
>  If you click on a link and make a purchase, I may receive a commission at no extra cost to you.
>

##  Download these first

You'll need to download these items before you get started setting up Linux: 

#### Newsletters

ZDNET Tech Today

ZDNET's Tech Today newsletter is a daily briefing of the newest, most talked about stories, five days a week.

 Subscribe

[See all](https://www.zdnet.com/newsletters/)

**Xcode:** You will need to download and install Xcode from the Mac App Store. Xcode is the primary development environment Apple wants developers to use to build Mac applications and mobile apps. It's free. Just open the App Store app and type "xcode" into the search field.

**The latest build of Ubuntu, for 64-bit Arm:** The Arm installer ISO isn't located on the main Ubuntu download site. Instead, point your browser to the [daily build page](https://cdimage.ubuntu.com/daily-live/current/) and scroll down until you see the desktop image for 64-bit ARM (standard download).

Screenshot by David Gewirtz/ZDNET

**GUILinuxVirtualMachineSampleApp:** [This is a sample app](https://developer.apple.com/documentation/virtualization/running%5Fgui%5Flinux%5Fin%5Fa%5Fvirtual%5Fmachine%5Fon%5Fa%5Fmac) that runs the virtual machine inside of Xcode. You'll need to download it and unzip it. 

Screenshot by David Gewirtz/ZDNET

Before you move on to the next step, be sure that Xcode is fully installed, that you have the Ubuntu .iso file, and that you have downloaded and unzipped the sample app. 

**Also: [Ubuntu Desktop 23.10 arrives: A glimpse into Ubuntu Linux's future](https://www.zdnet.com/article/ubuntu-desktop-23-10-arrives-a-glimpse-into-ubuntu-linuxs-future/)**

Once all of that is done, we can move on. 

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2135408/19272" target="_top" id="2135408">
  <img src="//a.impactradius-go.com/display-ad/19272-2135408" border="0" alt="https://techidaily.com" width="120" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2135408/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Configure the VM hosting app in Xcode

Go ahead and open Xcode. You'll see a starter screen. Tell it to open up an existing project. 

Screenshot by David Gewirtz/ZDNET

From here, navigate inside the folder you created when you extracted the sample application, and look for a file ending in .xcodeproj. Click open. 

Screenshot by David Gewirtz/ZDNET

This will open the sample application. Well, actually, it will warn you that you're opening a project downloaded from the Internet. But since the project comes right off the Apple developer site, I think you're good. 

Screenshot by David Gewirtz/ZDNET

Now, you'll have the project open. You need to do a bit of housekeeping, and then you'll be good. 

In the left-most pane, click the top-level sample app (shown at 1). Then, click the Signing & Capabilities tab (shown at 2), and finally, click the Add Account button at the Team prompt (shown at 3). 

Screenshot by David Gewirtz/ZDNET

This will take you to your Accounts tab, where you'll just set yourself up as a team. 

Screenshot by David Gewirtz/ZDNET

Once you've done this, close the window, and you'll be ready to move on. Here, you can see my app is going to be signed by my personal account. This just tells MacOS that it's my app and I want to allow it to run.

Screenshot by David Gewirtz/ZDNET

You're ready to start running the VM. Hit the little arrow to build and run. 

Screenshot by David Gewirtz/ZDNET

<!-- affiliate ads begin -->
<a href="https://unicoeye.pxf.io/c/5597632/2134239/18498" target="_top" id="2134239">
  <img src="//a.impactradius-go.com/display-ad/18498-2134239" border="0" alt="https://techidaily.com" width="721" height="90"/>
</a>
<img height="0" width="0" src="https://unicoeye.pxf.io/i/5597632/2134239/18498" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Installing Ubuntu

Your Xcode app will open a blank black window and a file chooser. The file chooser (although it doesn't tell you this) is looking for the Ubuntu install .iso file. So navigate to that .iso, click it, and click Open. 

Screenshot by David Gewirtz/ZDNET

Next, GRUB (Grand Unified Bootloader) will show up in that black window. Select Try or Install Ubuntu and hit Enter. 

Screenshot by David Gewirtz/ZDNET

And let the magic commence! Ubuntu is getting settled into your Xcode app: 

Screenshot by David Gewirtz/ZDNET

And here you go. Start configuring your Ubuntu install. 

Screenshot by David Gewirtz/ZDNET

Go ahead and select Install Ubuntu since you're already installing into a VM and not directly onto your computer anyway. 

Screenshot by David Gewirtz/ZDNET

I did the full installation: 

Screenshot by David Gewirtz/ZDNET

**Also: [Fedora Linux now runs on all M-powered Macs - except one](https://www.zdnet.com/article/fedora-linux-now-runs-on-all-m-powered-macs-except-one/)**

Use the default, which is to allow the installer to erase the virtual disk and set up your virtual filesystem: 

Screenshot by David Gewirtz/ZDNET

<!-- affiliate ads begin -->
<a href="https://review-au.sjv.io/c/5597632/2098700/14409" target="_top" id="2098700">
  <img src="//a.impactradius-go.com/display-ad/14409-2098700" border="0" alt="https://techidaily.com" width="160" height="90"/>
</a>
<img height="0" width="0" src="https://review-au.sjv.io/i/5597632/2098700/14409" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Run Ubuntu

Ubuntu is ready to run. Just click Restart Now and go to town. 

Screenshot by David Gewirtz/ZDNET

Once you restart, you'll be in a standard environment, with a nice little virtual machine you can play with. 

Screenshot by David Gewirtz/ZDNET

<!-- affiliate ads begin -->
<a href="https://aligracehair.sjv.io/c/5597632/2115916/19272" target="_top" id="2115916">
  <img src="//a.impactradius-go.com/display-ad/19272-2115916" border="0" alt="https://techidaily.com" width="300" height="90"/>
</a>
<img height="0" width="0" src="https://aligracehair.sjv.io/i/5597632/2115916/19272" style="position:absolute;visibility:hidden;" border="0" />
<!-- affiliate ads end -->

##  Final thoughts

During the installation phase, the Virtualization framework generates a GUI Linux VM.bundle package within your home folder. This grows fairly quickly, so if you're space-constrained, you may want to delete it when you're done Ubuntuing. Mine is 68.72GB after only a few hours of tinkering. 

**Also: [Ubuntu 23.10 seems like the usual boring update - until you dig into it](https://www.zdnet.com/article/ubuntu-23-10-seems-like-the-usual-boring-update-until-you-dig-in/)**

While the example application is limited to operating a single VM concurrently, the MacOS virtualization framework itself is capable of handling several VMs at the same time. This is not controlled by the application we built, but developers can use this framework to build more powerful virtualization management consoles. 

What do you think? Did you go ahead and install Ubuntu inside Xcode? Are you going to tattoo "Ubuntu/Xcode Forever" on your shoulder? Are you going to sing glorious songs of your Xcode prowess to all who will listen? I mean, you could. If you're not going to belt out songs of Macs and Linux, perhaps you could leave us a few comments below. 

---

_You can follow my day-to-day project updates on social media. Be sure to subscribe to my weekly update newsletter [on Substack](https://advancedgeekery.substack.com/), and follow me on Twitter at [@DavidGewirtz](https://twitter.com/davidgewirtz), on Facebook at [Facebook.com/DavidGewirtz](https://www.facebook.com/davidgewirtz), on Instagram at [Instagram.com/DavidGewirtz](https://www.instagram.com/DavidGewirtz/), and on YouTube at [YouTube.com/DavidGewirtzTV](https://www.youtube.com/user/DavidGewirtzTV)._

#### Linux

[The best Linux laptops for consumers and developers](https://www.zdnet.com/article/best-linux-laptop/ "The best Linux laptops for consumers and developers")

[Want to save your aging computer? Try these 5 Linux distributions](https://www.zdnet.com/article/want-to-save-your-old-computer-try-these-5-linux-distributions/ "Want to save your aging computer? Try these 5 Linux distributions")

[The best distros for beginners](https://www.zdnet.com/article/best-linux-desktops-for-beginners/ "The best distros for beginners")

[How to enable Linux on your Chromebook (and why you should)](https://www.zdnet.com/article/how-to-enable-linux-on-your-chromebook-and-why-you-should/ "How to enable Linux on your Chromebook (and why you should)")

* [The best Linux laptops for consumers and developers](https://www.zdnet.com/article/best-linux-laptop/ "The best Linux laptops for consumers and developers")
* [Want to save your aging computer? Try these 5 Linux distributions](https://www.zdnet.com/article/want-to-save-your-old-computer-try-these-5-linux-distributions/ "Want to save your aging computer? Try these 5 Linux distributions")
* [The best distros for beginners](https://www.zdnet.com/article/best-linux-desktops-for-beginners/ "The best distros for beginners")
* [How to enable Linux on your Chromebook (and why you should)](https://www.zdnet.com/article/how-to-enable-linux-on-your-chromebook-and-why-you-should/ "How to enable Linux on your Chromebook (and why you should)")

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
<li><a href="https://instagram-video-recordings.techidaily.com/updated-in-2024-insta-likes-and-video-powerhouse-get-noticed-and-grow-your-instagram-fast/"><u>[Updated] In 2024, Insta Likes & Video Powerhouse Get Noticed & Grow Your Instagram [Fast!]</u></a></li>
<li><a href="https://screen-recording.techidaily.com/2024-approved-unveiling-best-mac-methods-for-recording-roblox-games/"><u>2024 Approved Unveiling Best Mac Methods for Recording Roblox Games</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/neftiff-movavi/"><u>移動突破: NEF到TIFF的無限制免費轉換器 - 提供由Movavi</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/mpgwmv-movavi/"><u>在網際網路上無需付費轉換MPG到WMV - 利用 Movavi 專業解決方案</u></a></li>
<li><a href="https://location-fake.techidaily.com/a-detailed-vpna-fake-gps-location-free-review-on-oppo-k11x-drfone-by-drfone-virtual-android/"><u>A Detailed VPNa Fake GPS Location Free Review On Oppo K11x | Dr.fone</u></a></li>
<li><a href="https://sound-issues.techidaily.com/beat-the-apple-fixing-distorted-and-silent-sounds-on-iphones/"><u>Beat the Apple: Fixing Distorted and Silent Sounds on iPhones</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/best-free-and-premium-video-combiner-tools-for-windows-10-a-complete-guide/"><u>Best Free & Premium Video Combiner Tools for Windows 10: A Complete Guide</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/como-convertir-archivo-mov-a-formato-de-linea-libre-usando-herramienta-online-sin-coste-movavi-explicado-paso-a-paso/"><u>Cómo Convertir Archivo MOV a Formato De Línea Libre Usando Herramienta Online Sin Coste - MOVavi Explicado Paso a Paso</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/descargar-y-convertir-archivos-tga-a-formato-de-imagen-animada-gif-sin-costo-con-la-herramienta-online-de-conversion-gratuita-de-movavi/"><u>Descargar Y Convertir Archivos TGA a Formato De Imagen Animada GIF Sin Costo Con La Herramienta Online De Conversión Gratuita De Movavi</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/descubre-los-8-reproductores-sin-coste-para-videosdvds-compatibles-con-windows-11-and-macos/"><u>Descubre Los 8 Reproductores Sin Coste Para Vídeos/DVDs Compatibles Con Windows 11 & MacOS</u></a></li>
<li><a href="https://buynow-info.techidaily.com/exercise-and-entertain-with-garmin-vivoactive-2-sync-your-workouts-to-the-beat/"><u>Exercise and Entertain with Garmin Vivoactive 2 - Sync Your Workouts to the Beat</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/facil-comando-de-conversao-para-baixar-audio-em-mp3-do-formato-m4b-guia-detalhado/"><u>Fácil Comando De Conversão Para Baixar Áudio Em MP3 Do Formato M4B - Guia Detalhado</u></a></li>
<li><a href="https://video-content-creator.techidaily.com/new-in-2024-android-video-editors-for-chromebook-top-recommendations/"><u>New In 2024, Android Video Editors for Chromebook Top Recommendations</u></a></li>
<li><a href="https://techno-recovery.techidaily.com/resolving-the-missing-mfc42ddll-file-a-step-by-step-guide/"><u>Resolving the 'Missing mfc42d.dll' File: A Step-by-Step Guide</u></a></li>
<li><a href="https://program-issues.techidaily.com/step-by-step-resolution-eliminating-system-crashes-in-mass-effect-legendary-edition-across-platforms-pcxbox/"><u>Step-by-Step Resolution: Eliminating System Crashes in Mass Effect Legendary Edition Across Platforms (PC/Xbox)</u></a></li>
<li><a href="https://tech-haven.techidaily.com/transform-your-dandd-adventures-with-chatgpt-enhancements/"><u>Transform Your D&D Adventures with ChatGPT Enhancements</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/transformar-archivo-de-audio-en-mpg-sin-coste-convertidor-web-de-movavi/"><u>Transformar Archivo De Audio en MPG Sin Coste - Convertidor Web De Movavi</u></a></li>
<li><a href="https://sound-optimizing.techidaily.com/updated-2024-approved-locating-chuckles-the-guide-to-comedy-audio-tones/"><u>Updated 2024 Approved Locating Chuckles The Guide to Comedy Audio Tones</u></a></li>
<li><a href="https://tech-savvy.techidaily.com/w64-mp3-movavi/"><u>W64 MP3ファイルを無料でオンライン変換: Movaviの簡単ガイド</u></a></li>
</ul></div>

