---
title: Understanding & Activating Smart App Control in Windows 11 - An Essential Tutorial
date: 2024-08-26 16:27:53
updated: 2024-08-29 12:26:10
tags:
  - desktop
categories:
  - tech
thumbnail: https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/06/52679273174_c93a060c3c_o.jpg
---

## Understanding & Activating Smart App Control in Windows 11 - An Essential Tutorial

### Quick Links

* [What Is Smart App Control and How Does It Work?](https://location-social.techidaily.com/how-to-change-location-on-tiktok-to-see-more-content-on-your-vivo-y02t-drfone-by-drfone-virtual-android/)
* [How to Turn On Smart App Control](https://twitter-videos.techidaily.com/new-interlinked-upload-sharing-content-via-twt-plus-tumble-for-2024/)
* [How to Turn Off Smart App Control](https://tech-revival.techidaily.com/enterprise-focused-insights-on-gpt-systems/)

### Key Takeaways

* Smart App Control is a Windows 11 Security feature that stops malicious apps running on your computer.
* Smart App Control can only be enabled on a clean Windows installation.
* While you can force enable Smart App Control on an existing Windows installation using a registry tweak, this can affect its efficacy.

 Smart App Control (SAC) is a Windows Security feature that helps protect you against malicious apps. While it's available on all devices running Windows 11 22H2 or above, you might find you can't turn it on—and for a good reason.

 Let's explore how Smart App Control works, why it's turned off on some systems, and how to enable it.

##  What Is Smart App Control and How Does It Work?

 Smart App Control is a feature within Windows Security that provides protection against untrustworthy apps. When you try to run an app, SAC analyzes its credibility using Microsoft’s Intelligent Security Graph, a cloud-based security service. If the service is unable to make a confident prediction, it then checks the app for a valid signature (which identifies where the file originates from and if it's a trusted source).

 Apps from known publishers or with valid signatures will run as expected. If not, the program is blocked. There’s no manual override option, nor can you add an app to an exemption list.

!['Smart App Control has blocked this app' notification.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/smart-app-control-app-blocking-notification.jpg) 

 Microsoft intends that SAC is only useable on a clean Windows installation. By doing so, Windows can ensure that all the apps installed on your computer are vetted by SAC, thus ensuring the devices' safety. If you received SAC as a part of a Windows 11 update, you'll need to [perform a factory reset](https://facebook-video-footage.techidaily.com/new-blueprints-for-breaking-ground-in-edu-video-production-on-youtube-channels-for-2024/) or [clean install Windows 11](https://instagram-video-files.techidaily.com/new-2024-approved-celebrating-the-premier-25-ones-to-watch-on-insta/) before you can use it (unless you perform a registry tweak, explained below).

 Windows doesn't automatically enable SAC completely. By default, it starts in Evaluation mode. During the evaluation period, Windows monitors your application usage pattern to determine if you are a suitable candidate to have SAC enabled full-time.

![Smart App Control Evaluation mode selected in Windows 11](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/smart-app-control-screen-windows-security-windows-11.jpg) 

 Once the evaluation is complete, if Windows thinks SAC can work without too many interruptions on your system, it's automatically turned on. If not, it's disabled.

##  How to Turn On Smart App Control

 Assuming you meet the conditions explained above, you can skip Evaluation mode and turn on Smart App Control in Windows Security settings.

 First, press Win+i to open the Settings app. Select the "Privacy & Security" tab in the left pane, then click "Windows Security" on the right.

![Windows 11 Privacy & security settings.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/windows-11-settings-app-privay-security-screen.jpg) 

 Click "Open Windows Security" to launch the Windows Security app.

![Windows 11 Settings app showing Open Windows Security option.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/windows-11-settings-app-showing-open-windows-security-option.jpg) 

 In Windows Security, select the "App & Browser Control" tab. Then, beneath "Smart App Control", click "Smart App Control Settings".

![App and Browser Control tab selected in Windows Security.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/windows-security-app-browser-control-tab-selected-1.jpg) 

 Select "On" to enable Smart App Control on your Windows device. Once enabled, SAC starts monitoring and blocks any suspicious app execution on your computer.

![Smart App Control turned on in Windows 11.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/smart-app-control-turned-on-in-windows-11.jpg) 

###  How to Force Enable Smart App Control Using the Registry Editor

 If SAC is turned off on your Windows computer for any reason, you can force enable it using a registry tweak.

 This method bypasses the intended implementation for Smart App Control. We recommend you only enable Smart App Control on a clean installation for a more secure experience. If you do want to proceed, be aware that modifying your Windows Registry involves risk. [Create a restore point](https://instagram-video-files.techidaily.com/updated-in-2024-multiplying-joy-sharing-a-pile-of-photos-and-videos-with-instagram/) before proceeding.

 Press Win+i to open Run. Type "regedit" and click "OK" to open the Registry Editor.

![Inputting regedit within Run.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/win-plus-i-shortcut-to-open-run-box.jpg) 

 In the Registry Editor, navigate to the following location:

Computer > HKEY_LOCAL_MACHINE > SYSTEM > CurrentControlSet > Control > CI > Policy

 In the right pane, locate and double-click the "VerifiedAndReputablePolicyState" value.

![Windows 11 Registry Editor showing the 'VerifiedAndReputablePolicyState' value.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/windows-11-registry-editor-showing-smart-app-control-policy.jpg) 

 In the "Value Data" field, type 1 to enable Smart App Control and click "OK" to save the changes. Alternatively, type 2 to put SAC in Evaluation mode, or 0 to turn it off. You need to relaunch the Windows Security app to apply the changes.

![Changing VerifiedAndReputablePolicyState value in Registry Editor to 1.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/changing-verifiedandreputablepolicystate-value-in-registry-editor-to-1-in-windows-11.jpg) 

##  How to Turn Off Smart App Control

 If you find SAC to be too intrusive, you can turn it off manually in Windows Security settings. Disabling SAC is permanent, and you can’t enable it again without reinstalling Windows or altering the registry (as explained above).

 Open the Start menu, search for "Smart App Control", and select the matching result.

![Smart App Control in Windows 11 search.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/smart-app-control-in-windows-11-search.jpg) 

 Within the Smart App Control window, select "Off."

![Windows Smart App Control settings to enable or disable.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/windows-security-smart-app-control-off-option-showing.jpg) 

 Read the confirmation prompt, then click "Yes, I'm Sure" to disable Smart App Control.

![Smart App Control confirmation screen when turning off.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/smart-app-control-off-confirmation-screen.jpg) 

---

 Smart App Control should work without issue for you. However, if you’re unsure whether to use SAC, leave it in Evaluation mode and let Windows decide what’s best for you. If you find it too intrusive, you can always turn it off in Windows Security settings.

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
