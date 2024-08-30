---
title: "Step-by-Step Tutorial on Generating Unique AI Graphics: Gifs and Videos via Stable Diffusion"
date: 2024-08-26 19:22:36
updated: 2024-08-29 10:42:56
tags:
  - cutting-edge
categories:
  - tech
thumbnail: https://thmb.techidaily.com/1c0c9da7d1a6e96b7776310e8c7452d6bdf3958002401b8a3af1db05343b435b.jpg
---

## Step-by-Step Tutorial on Generating Unique AI Graphics: Gifs and Videos via Stable Diffusion

### Quick Links

* [Stable Diffusion Can Generate Video?](https://ai-video-apps.techidaily.com/new-vn-video-editor-pro-apk-a-professional-level-video-editing-experience-in-2024/)
* [Animate an Image Using Inpaint](https://data-wizards.techidaily.com/streamlining-file-corruption-fixes-on-macbook/)
* [Generate a Video Using Deforum](https://snapchat-videos.techidaily.com/new-2024-approved-social-network-showdown-2021-the-battle-between-tiktok-and-snapchat/)

### Key Takeaways

 To make an animation using Stable Diffusion web UI, use Inpaint to mask what you want to move and then generate variations, then import them into a GIF or video maker. Alternatively, install the Deforum extension to generate animations from scratch.

 Stable Diffusion is capable of generating more than just still images. With some built-in tools and a special extension, you can get very cool AI video without much effort. Here's how to generate frames for an animated GIF or an actual video file with Stable Diffusion.

##  Stable Diffusion Can Generate Video?

 While [AI-generated film is still a nascent field](https://facebook-clips.techidaily.com/new-how-to-prevent-and-mend-live-stream-glitches-fb/), it is technically possible to craft some simple animations with [Stable Diffusion](https://unlock-android.techidaily.com/7-ways-to-unlock-a-locked-xiaomi-redmi-k70-phone-by-drfone-android/), either as a [GIF](https://driver-download.techidaily.com/1722970449814-get-set-up-fast-linksys-wrt326n-software-pack-full-compatibility-guaranteed/) or an actual video file. There are limitations though.

 Because img2img makes it easy to generate variations of a particular image, Stable Diffusion lends itself well to quickly crafting a bunch of frames for animations, cyclical ones in particular. Think flames licking up from a fire, wheels spinning on a car, or water splashing in a fountain. A practical use could be giving a lifelike ambiance to some RPG artwork:

![A hearth burning in a Dungeons and Dragons-style tavern.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/08/hearth-slow-anim.gif) 

Jordan Gloor / Stable Diffusion / How-To Geek

 You can even make videos based on real images instead of synthetic ones. Here I took a photo of a plant being watered and, with a few clicks, animated the water stream:

![Water being poured into a potted plant.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/08/plant-animation-anim.gif) 

Jordan Gloor / Stable Diffusion / How-To Geek

 If you want to animate an object so that it moves from point A to point B, that's a tall order for Stable Diffusion (at least for now). You'd likely be spending a lot of time tweaking prompts and settings, then poring over a ton of output to find the best frames and placing them in correct order. At that point, you might as well break out Adobe Illustrator and just start animating by hand.

 Despite that, you can make some cool, simple animations with a basic Stable Diffusion setup and another tool of your choice for stitching the frames together in an animation. There's also a project called Deforum that uses Stable Diffusion to create "morphing" animations that look pretty interesting. It'll spit out an [MP4](https://facebook-video-footage.techidaily.com/updated-in-2024-cutting-edge-techniques-for-youtube-video-production-with-sony-vegas/) video, so no external tools are required, and it even lets you add audio. We'll show you the basics of both methods.

 For the purpose of this article, we're going to assume you've already [installed a graphical interface for Stable Diffusion](https://sim-unlock.techidaily.com/in-2024-top-imei-unlokers-for-your-tecno-spark-go-2023-phone-by-drfone-android/), specifically [AUTOMATIC1111's Stable Diffusion web UI](https://github.com/AUTOMATIC1111/stable-diffusion-webui). Compared to the [standard command line install](https://unlock-android.techidaily.com/7-ways-to-unlock-a-locked-xiaomi-redmi-k70-phone-by-drfone-android/), it makes generating images way easier and comes with a ton of handy tools and extras.

##  Animate an Image Using Inpaint

 Using the img2img tool Inpaint, you can highlight the part of an image you want to animate and generate several variations of it. Then you'll drop them into a GIF or video maker and save the frames as an animation.

###  Step 1: Get an Image and Its Prompt

 Start by dropping an image you want to animate into the Inpaint tab of the img2img tool. If you don't have one generated already, take some time [writing a good prompt](https://screen-mirroring-recording.techidaily.com/updated-2024-approved-quick-tips-making-high-quality-recordings-on-iphone/) so you get a good starter photo. You could also import an image you've photographed or drawn yourself.

 If you're importing an image that you didn't generate with Stable Diffusion, you'll still need an appropriate prompt for generating variations, so click "Interrogate CLIP" at the top of the Img2Img page. That will generate a starter prompt based on what Stable Diffusion thinks your image contains. Complete the prompt by adding any other important details.

 For our guide, we've generated a 512x512 image of a robot under a night sky that we want to give a time-lapse sort of animation, with shooting stars and galaxies passing by.

![A robot standing in a field under a starry sky.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/02/robot1.png.png) 

_Stable Diffusion_

 If you want to follow along precisely, you can recreate it with the prompt we used:

a robot stands in a field looking up at the night sky during a meteor shower, shooting stars, galaxies, the cosmos, milky way, ultra realistic, highly detailed, 4k uhd

 And these are the settings we used:

**Checkpoint:** Stable Diffusion 2.0

**Sampling Method:** DPM++ SDE

**Sampling Steps:** 20

**CFG Scale:** 5

**Seed:** 4177542269

###  Step 2: Mask the Parts to Animate With InPaint

 With your image and prompt in place, in the Inpaint tool, use the paintbrush to mask (cover up) every part of the image you want to animate. Leave uncovered anything you want static.

 In our example, we're covering most of the sky. We left a bit of cushion around the robot because in our testing, if we got too close, Stable Diffusion would sometimes add antennae and other appendages to the robot.

![A robot standing in a field under a starry sky.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/02/robot1.png.png) 

_Stable Diffusion_

 You can adjust the Inpaint brush size with a slider by clicking the brush button in the top-right corner of the canvas.

###  Step 3: Generate Your Frames

 Now that you've masked every part of your image you want to see moving, it's time to generate the frames of our animation. But first, you'll want to make sure img2img has the right settings. They can be confusing, so we'll explain what some of them mean and why you may or may not want to tweak them:

* **Mask Mode: Inpaint Masked** \- This makes sure everything covered gets changed and not the other way around. If, for some reason, you want to modify the unmasked part instead, change it to "Inpaint Not Masked."
* **Masked Content: Original** \- This ensures Stable Diffusion will see and take into account the existing image when it's generating variations. Otherwise, it will consider the masked content a blank or randomized canvas.
* **Inpaint Area: Whole Picture** \- This forces Stable Diffusion to generate a whole new image for each frame before integrating it with the original image. Switching to "Only Masked" might speed up generation but may also give you worse results.
* **Sampling Method: DPM++ SDE** \- This is the same sampling method we used for generating our original image, and we're sticking with it to ensure a consistent look. If you don't know what to use, "Euler a" is an all-around good choice.
* **Batch Count: 60** \- This is how many images you want to generate. You may need more or fewer depending on how fast and how long you want your animation sequence to be.
* **CFG Scale: 5** \- The CFG scale, in a sense, determines how much creative liberty Stable Diffusion has. The higher the number, the more strictly Stable Diffusion will try to follow your prompt. Increasing it and getting good results requires having a very good prompt.
* **Denoising Strength: 0.3** \- Possibly the most important setting for this project, the denoising scale determines how much Stable Diffusion will change the original image. You probably want to keep it down around 0.2 or 0.3, since too much frame-to-frame change can ruin animation.
* **Seed: -1** \- This tells Stable Diffusion to start with a random seed. We don't recommend reusing the seed from your original image, since that reduces the amount of variation you'll get (if any at all).

 With all of your settings in place, click "Generate" and sit back while Stable Diffusion draws your animation frames for you. You'll find them in the `/outputs/img2img-images` folder of your Stable Diffusion directory. If you don't like the results, tweak the settings (probably starting with denoising strength and sampling steps) and try again.

###  Step 4: Batch Upscale Your Frames (Optional)

 If you plan to create a high-definition video, remember to upscale all your newly generated frames to the resolution you want. Click "Send to Extras" to get started.

![Click "Send to Extras" so you can upscale your generated images in Stable Diffusion.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/02/robot2.png) 

 Inside Extras, switch to the "Batch Process" tab.

![In the Extras tab, switch to Batch Process and then click "Generate."](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/02/robot4.png) 

 Adjust the "Resize" scale to the number of times you want it resized (setting to 2 will change 512x512 images into 1024x1024 images). Alternatively, switch from "Scale by" to "Scale to" and set a specific resolution. Also set "Upscaler 1" to the upscaler of your choice. We had good enough results with R-ESRGAN 4x+, but feel free to experiment to see which handles your images best.

![Adjust settings for upscaling, then click Generate.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/02/robot5.png) 

 Then hit "Generate" and Stable Diffusion will give you a higher-resolution version of each frame, saved in your `/outputs/extras` folder.

###  Step 5: Animate the Frames in a GIF or Video Maker

 Now that you've got your frames, it's time to stitch them all together and create your final animation. There are many tools you can do this with, including free dedicated websites like [Ezgif](https://ezgif.com/maker) and [flixier](https://flixier.com/tools/gif-maker) that are easy to use and have a lot of fine-tuning controls. However, remember that those websites can see everything you upload, so don't give them anything you aren't comfortable with the world knowing about.

 While those websites are pretty self-explanatory, we'll be demonstrating how you use a free offline photo editing tool, [GIMP](https://www.gimp.org/), to make a GIF. If you want a video file, use [Kdenlive](https://kdenlive.org/en/) or a similar video editor instead---just make sure you tweak the settings so all your frames get imported as clips that are one second or shorter, depending on many frames per second you want.

 To begin, [download GIMP](https://www.gimp.org/downloads/) and install it on your computer if you haven't already. Launch it, then go to File > Open as Layers.

![Click "File" in GIMP and select "Open as Layers."](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/02/robot6.png) 

 Find where the frames you generated are and select all of them at once before clicking "Open." (Hold the Shift key to select multiple files quickly.) GIMP will import all of your images as a separate layer on one canvas. We want this because the way GIMP's GIF generation works is by going through every layer from bottom to top, treating each consecutive layer as the next frame in the animation.

 Now's the fun part. To watch a preview of your GIF, go to Filters > Animation > Playback.

![Click Filters, then under Animation click "Playback" to watch a preview of your GIF.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/02/robot7.png) 

 Press the spacebar to play and pause the GIF. If frames go by too fast or slow, adjust the FPS at the bottom of the playback dialog, and click the refresh button at the top to reload the preview with the new frame rate.

![Click the FPS dropdown box to change the rate of frames-per-second, then the refresh button to regenerate the GIF preview.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/02/robot8.png) 

 Once the animation looks good to you, it's time to generate the GIF file. Close the preview and click File > Export As. When you type in the file save name, add the `.gif` extension to the end so that GIMP knows you want a GIF.

![A robot standing in a field under a starry sky.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/02/robot1.png.png) 

_Stable Diffusion_

 In the GIF export dialog box that appears, make sure the "As Animation" box is checked. Adjust the number of milliseconds between frames too if you want a different frame rate. There are 1000 milliseconds in a second, so 100 will get you right around 10 FPS. Finally, click "Export."

![A robot standing in a field under a starry sky.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/02/robot1.png.png) 

_Stable Diffusion_

 Boom, you've got your complete animated GIF.

![A robot under a night sky.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/08/robot-night-sky-anim.gif) 

Jordan Gloor / Stable Diffusion / How-To Geek

##  Generate a Video Using Deforum

 If you want to want to create more interesting animations with Stable Diffusion, and have it output video files instead of just a bunch of frames for you to work with, use [Deforum](https://deforum.github.io/). It's an image synthesis project with an extension available for Stable Diffusion web UI that lets you direct and generate MP4 video files, even with audio. It's a very powerful and complex tool with a lot of settings to experiment with, including camera pans and zooms, multiple prompts, and video import.

 For our purposes, we'll just introduce you to the basics of generating a fairly simple but interesting animation.

###  Step 1: Install the Deforum Extension

 To get [the Deforum extension](https://github.com/deforum-art/deforum-for-automatic1111-webui), open a command prompt and [change directories](https://extra-information.techidaily.com/quick-and-easy-iphone-burst-techniques/) to your `stable-diffusion-web-ui` folder. Then use this [git clone](https://tech-revival.techidaily.com/guarding-your-chats-how-to-avoid-chatgpt-saving-interactions/) command to install Deforum in your extensions folder use.

git clone https://github.com/deforum-art/deforum-for-automatic1111-webui extensions/deforum

 Launch Stable Diffusion web UI as normal, and open the Deforum tab that's now in your interface.

 The Deforum extension comes ready with defaults in place so you can immediately hit the "Generate" button to create a video of a rabbit morphing into a cat, then a coconut, then a durian. Pretty cool!

###  Step 2: Write Your Prompts

 You might be used to writing individual prompts with Stable Diffusion, but Deforum lets you write multiple prompts that are "scheduled," meaning at whatever point in the animation you choose it will switch to generating frames based on the next prompt in the schedule.

 Click the "Prompts" tab and change the existing prompts to whatever you want, keeping the bracket and tab structure in place. For our example, we'll use this set of prompts:

{ "0": "a robot stands under the night sky during a meteor shower, shooting stars, galaxies, the cosmos, milky way, ultra realistic, highly detailed, 4k uhd", "40": "a space station flies through space during a meteor shower, ultra realistic, highly detailed", "80": "a supernova explodes, vibrant colors, ultra realistic, highly detailed"}

 So what do those numbers mean? By default Deforum generates 120 frames for your animation, and we're dividing that set of frames into three parts. `0` signifies the first frame, so it and all frames after it will be im2img variations of the first prompt. Then at frame 40, Stable Diffusion will start making variations based on our second prompt. At 80, it switches to the third. You can add as many prompt changes as you want and adjust the max frame limit on the Keyframes tab as needed.

###  Step 3: Adjust Deforum Settings

 You've probably already noticed there are a ton of settings involved in Deforum, but we'll walk through a few to get you started. First, in the "Run" tab, you'll find many of your typical Stable Diffusion settings. Rename the batch, enter the seed you want to start with (we're reusing the one for our robot), and change the sampler to the one you want.

![In the "Run" tab change the sampler, seed, and batch name to your preferred settings.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/02/deforum1.png) 

 In the Keyframes tab you can adjust the motion of the "camera" for the animation. It's set by default to zoom at intervals, but we want to add a vertical "pan" movement, so we'll add `0:(-2), 100:(4)`to the "Translation Y" frame. That tells Deforum to treat the first frame as being at pixel -2 on the Y axis, then by frame 100 move to pixel 4\. That will give us a slight pan upward as the animation progresses.

![Enter values in the "Translation Y" field if you want the animation view to change vertically.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/02/deforum3.png) 

 In the Output tab, we'll check the "Make GIF" box which will give us a GIF file in addition to the MPEG video file. This is also where you'd add audio with the "Add Soundtrack" and "Soundtrack Path" settings, if you have some.

![In the Output tab, check the "Make GIF" box if you want a GIF file.](https://static1.howtogeekimages.com/wordpress/wp-content/uploads/2023/02/deforum2.png) 

###  Step 4: Generate Your Video

 Finally, hit that big "Generate" button. Since Deforum is creating and stitching many frames, this will take time, so grab some coffee while you wait. When it's complete, you'll find the MPEG file, the GIF version, plus every individual frame and a readout of the settings you used under the batch name in your `/outputs/img2img-images` directory.

 Here's what our prompt got us:

Your browser does not support the video tag. 

 It's no summer blockbuster, but it's still kind of mesmerizing! Check out [the official Deforum quick start guide](https://docs.google.com/document/d/1RrQv7FntzOuLg4ohjRZPVL7iptIyBhwwbcEYEW2OfcI/edit) to learn about all the other knobs and dials you can adjust.

---

 If you're looking for other cool AI projects, learn how to [generate Minecraft texture packs with Stable Diffusion](https://apple-account.techidaily.com/how-to-remove-the-two-factor-authentication-on-iphone-8-plus-by-drfone-ios/) or [get started with ChatGPT](https://extra-resources.techidaily.com/new-capture-clarity-editing-insights-for-professional-results/), plus [the surprising things you can do with ChatGPT](https://facebook-clips.techidaily.com/updated-achieve-higher-interactions-mastering-the-art-of-square-videos-for-2024/).

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
