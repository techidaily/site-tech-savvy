---
title: Efficiently Disconnect Your Bluetooth Devices From PCs Running Windows 11 or 10
date: 2024-08-26 19:28:35
updated: 2024-08-29 11:10:30
tags:
  - desktop
categories:
  - tech
thumbnail: https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/10/52679424740_0fce47316a_o-5.jpg
---

## Efficiently Disconnect Your Bluetooth Devices From PCs Running Windows 11 or 10

### Quick Links

* [Remove Bluetooth Devices Using the Settings App](https://extra-tips.techidaily.com/next-gen-learning-vrs-educational-impact/)
* [Remove Bluetooth Devices with Device Manager](https://facebook-video-share.techidaily.com/updated-navigating-netflix-and-youtubers-how-jake-paul-succeeded/)
* [Remove Bluetooth Devices Using Command Prompt](https://win-able.techidaily.com/solved-mount-and-blade-2-bannerlord-crashes/)

### Key Takeaways

* To remove a Bluetooth device on Windows 11, head into Settings > Bluetooth & Devices > Devices. Next to the device, click the three dots and choose "Remove Device."
* On Windows 10, navigate to Settings > Devices > Bluetooth & Other Devices. Select the device, click "Remove Device," and choose "Yes."
* To delete a Bluetooth device with its drivers, open Device Manager, expand "Bluetooth," right-click the device, select "Uninstall Device," and choose "Uninstall."

 If you don’t wish to keep a paired Bluetooth device, it’s easy to remove it using Settings, Device Manager, and Command Prompt. We’ll show you how to use all these methods on your Windows 11 or Windows 10 PC.

##  Remove Bluetooth Devices Using the Settings App

 A quick way to remove paired Bluetooth devices is by using Windows’ Settings app, though it is a little different in Windows 10 and Windows 11.

 If your device installed certain drivers, Settings won’t remove them. In this case, use the Device Manager method below. If you're unsure what method to use, stick to this one.

###  On Windows 11

 Launch the Settings app by pressing Windows+i. In the left sidebar, select "Bluetooth & Devices." On the right pane, choose "Devices."

![Bluetooth & Devices > Devices highlighted in Windows 11 Settings.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/1-bluetooth-devices-windows-11.jpg) 

 Locate the device you want to remove on the Devices page, then click the three dots next to it and choose "Remove Device."

!['Remove Device' highlighted for a Bluetooth device in Windows 11 Settings.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/2-remove-bluetooth-device-windows-11.jpg) 

 Under your device's name, you'll see a "Removing Device" message. This message will disappear once Windows has deleted the device.

###  On Windows 10

[Open Settings](https://facebook-video-footage.techidaily.com/updated-2024-approved-5-easy-ways-to-multiply-your-youtube-follower-base/) by pressing Windows+i. Select "Devices" in Settings.

!['Devices' highlighted in Windows 10 Settings.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/3-devices-windows-10.jpg) 

 From the left sidebar, choose "Bluetooth & Other Devices."

!['Bluetooth & Other Devices' highlighted in Windows 10 Settings.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/4-bluetooth-devices-windows-10.jpg) 

 On the right pane, find and click the device to remove. Then, choose "Remove Device."

!['Remove Device' highlighted for a Bluetooth device in Windows 10 Settings.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/5-remove-bluetooth-device-windows-10.jpg) 

 In the open prompt, select "Yes."

!['Yes' highlighted in the Bluetooth device removal prompt.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/6-bluetooth-device-removal-prompt-windows-10.jpg) 

##  Remove Bluetooth Devices with Device Manager

 If you can’t remove a device from Settings or you want to remove the device and delete its associated drivers, use this method.

[Open the Device Manager utility](https://desktop-recording.techidaily.com/updated-2024-approved-easily-record-lenovo-laptop-screen-activity/) by right-clicking the Start Menu and selecting "Device Manager."

!['Device Manager' highlighted in Windows' Power User menu.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/7-launch-device-manager.jpg) 

 On the utility window, expand "Bluetooth." Find the device to remove, right-click it, and select "Uninstall Device."

!['Uninstall Device' highlighted for a Bluetooth device in Device Manager.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/8-uninstall-bluetooth-device.jpg) 

 In the open prompt, choose "Uninstall."

!['Uninstall' highlighted in the 'Uninstall Device' window.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/9-confirm-remove-bluetooth-device-1.jpg) 

[Restart your Windows 11](https://screen-video-capture.techidaily.com/updated-in-2024-addressing-mute-problems-in-obs-live-recording/) or [Windows 10](https://article-posts.techidaily.com/comparing-the-creme-de-la-creme-gopro-hero5-black-to-hero4-silver-for-2024/) PC.

##  Remove Bluetooth Devices Using Command Prompt

 If you prefer using command line methods over graphical ones, you can use a command in Command Prompt (or PowerShell) to remove the paired Bluetooth devices from your PC. This method achieves the same result as the graphical methods above.

 To use this method, you’ll first find your device’s instance path. The command that deletes the devices requires this path to identify your device. To find it, open Device Manager by pressing Windows+X and choosing "Device Manager."

 Expand "Bluetooth," right-click the device you want to delete, and select "Properties."

!['Properties' highlighted for a Bluetooth device in Device Manager.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/10-bluetooth-device-properties.jpg) 

 On the Properties window, open the "Details" tab. Click the "Property" drop-down menu and select "Device Instance Path." This is the second option in the menu.

 Right-click the text displayed in the "Value" field and select "Copy."

!['Details,' 'Property,' and 'Copy' highlighted on the 'Properties' window.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/11-copy-bluetooth-device-instance-path.jpg) 

 Close Device Manager. Open the Start Menu, search for "Command Prompt", and select "Run as Administrator."

!['Run as Administrator' highlighted for Command Prompt in the Start Menu.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/12-open-cmd-as-admin.jpg) 

 In the User Account Control (UAC) prompt, select "Yes."

 On the Command Prompt window, type the following command, replacing "DEVICE\_ID" with the value you copied. Enclose the pasted value in double quotes.

 Then, press Enter.

 Make sure to enter the correct device instance path in the command, or you’ll accidentally end up removing a device you didn’t want to delete.

pnputil /remove-device “DEVICE_ID”

![The command to remove a Bluetooth device typed in Command Prompt.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2024/01/13-remove-bluetooth-device-cmd.jpg) 

 Command Prompt will remove the specified Bluetooth device and display a message. If your device isn't removed, ensure the entered device instance path is correct.

---

 With multiple methods at your disposal, removing paired Bluetooth devices, even the stubborn ones, is easy on your Windows PC. You can utilize the method you find convenient to use. And in the future, if you wish to use a device again with your PC, simply pair it how you would any device with your machine.

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
