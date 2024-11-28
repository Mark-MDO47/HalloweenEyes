# HalloweenEyes
Eyes in a plastic skull that detect and track people.

**Table Of Contents**
* [Top](#halloweeneyes "Top")
* [The Plan](#the-plan "The Plan")
* [The Hardware](#the-hardware "The Hardware")
* [The AI Software](#the-ai-software "The AI Software")
  * [Ultralytics](#ultralytics "Ultralytics")
  * [Edge Impulse](#edge-impulse "Edge Impulse")
  * [OpenCV](#opencv "OpenCV")
  * [TinyML EDU](#tinyml-edu "TinyML EDU")
* [License](#license "License")

## The Plan
[Top](#halloweeneyes "Top")<br>
John and I will make a plastic skull with one or two eyes that will follow people. If there are multiple people, it will follow one for a while then choose another and follow them for a while.
- Based on https://learn.adafruit.com/hallowing-all-seeing-skull.
- Upgrades to use Artificial Intelligence image processing - face tracking
  - Maybe using Ultralytics and YOLOv8 approach https://www.youtube.com/watch?v=hHyHmOtmEgs&list=PL1FZnkj4ad1PFJTjW4mWpHZhzgJinkNV0&index=46
  - Maybe using TinyML approach https://www.hackster.io/mjrobot/computer-vision-at-the-edge-with-grove-vision-ai-module-v2-0003c7
  - Maybe using OpenCV approach


## The Hardware
[Top](#halloweeneyes "Top")<br>
Still selecting hardware but probably the following:

| Purpose | Choice(s) | Comments |
| --- | --- | --- |
| plastic skull | Life Size Skeleton Skull for Halloween Decor | https://www.amazon.com/gp/product/B0C777NBDJ |
| eyes | Adafruit HalloWing M4 Express | https://www.adafruit.com/product/4300 |
| eye accessories | Clear Acrylic Lens Holder | https://www.adafruit.com/product/4013 |
| eye accessories | Convex Glass Lens with Edge | https://www.adafruit.com/product/3853 |
| AI & vision | maybe Seeed Studio XIAO ESP32S3 Sense<br>includes microphone | https://www.seeedstudio.com/XIAO-ESP32S3-Sense-p-5639.html<br>https://www.youtube.com/watch?v=_wvuOsRgmt4<br>https://github.com/limengdu/SeeedStudio-XIAO-ESP32S3-Sense-camera |
| AI & vision | maybe Seeed Studio Vision AI Module V2 | https://www.digikey.com/en/products/detail/seeed-technology-co-ltd/113991054/16652880<br>currently backorder https://us.seeedstudio.com/Grove-Vision-AI-V2-Kit-p-5852.html?___store=us |
| AI & vision | maybe Sipeed Maixduino AI Development Board<br>K210 RISC-V AI+lOT ESP32 | https://www.dfrobot.com/product-1972.html |
| AI & vision | maybe Aideepen ESP32-CAM W BT Board<br>inexpensive, maybe fast enough | https://www.amazon.com/dp/B0948ZFTQZ |

## The AI Software
[Top](#halloweeneyes "Top")<br>
There are some great resources that allow us to operate at a higher level than I have done before. I **REALLY** like all of these!
- Please take my comments with a grain of salt. They are just my opinions after doing a quick survey. As I get more experience with them I may need to change my thinking on these.

### Ultralytics
[Top](#halloweeneyes "Top")<br>
This seems to be mostly for image processing based on YOLOv5 and YOLOv8 (YOLO in this context means You Only Look Once).
- Seems to allow moving trained models to different formats for implementation on inexpensive hardware.
- They also have a cool Ultralytics AP that allows you to run it on your smart phone (either type).
- Ultralytics is especially interesting to me since I can download the training software and (slowly) train on my own equipment.
  - I am not anxious to (for instance) upload photos or voice captures of my family to the internet.

Here are some entries to the Ultralytics world:
- https://www.ultralytics.com/
- https://github.com/ultralytics
- https://github.com/ultralytics/ultralytics
- https://hub.ultralytics.com/home - free-level account available
- https://www.youtube.com/watch?v=hHyHmOtmEgs&list=PL1FZnkj4ad1PFJTjW4mWpHZhzgJinkNV0&index=46 - this person tracking seems ideally suited for us

### Edge Impulse
[Top](#halloweeneyes "Top")<br>
This has a broad application range - images, speech, keyword detection, motion.
- Very good integration to allow moving trained models to different formats for implementation on inexpensive hardware. There are some known examples such as ESP32-CAM where some pin assignments were changed from an existing officially supported target and made to work, although not officially supported.
- I have not yet found a way to do the training on my own hardware. On the plus side, their Internet-based training facilities are extremely easy to use and seem quite comprehensive.

Here are some entries to the Edge Impulse world:
- https://studio.edgeimpulse.com/studio - free-level account available
- https://edge-impulse.gitbook.io/docs
- https://edge-impulse.gitbook.io/docs/tutorials/end-to-end-tutorials/image-classification
- https://edge-impulse.gitbook.io/docs/edge-ai-hardware/edge-ai-hardware
- https://edge-impulse.gitbook.io/docs/run-inference/arduino-library

### OpenCV
[Top](#halloweeneyes "Top")<br>
CV stands for Computer Vision. Seems to have an emphasis on face recognition.
- They have lots of courses. I signed up for free "OpenCV Bootcamp" and "TensorFlow Keras" courses.

I haven't explored them too much but so far they look very good.
- https://opencv.org/ - free-level account available
- https://opencv.org/university

### TinyML EDU
[Top](#halloweeneyes "Top")<br>
ML stands for Machine Learning. This also looks quite interesting. I have just started exploring. They obviously have courses; also an interesting PDF book "TinyML-Made-Easy.pdf". Lots of activity from them on hackster.io and some cross-pollination with Edge Impulse.
- https://tinyml.seas.harvard.edu/
- https://github.com/tinyMLx
- https://www.hackster.io/mjrobot/tinyml-made-easy-object-detection-with-xiao-esp32s3-sense-6be28d
- https://www.hackster.io/mjrobot/tinyml-made-easy-image-classification-w-xiao-esp32s3-sense-cb42ae

## License
[Top](#halloweeneyes "Top")<br>
I have listed the MIT license which covers any code or comments or materials I create and put here.

Obviously if I use some source that is controlled by a different license, it retains that license.

[Top](#halloweeneyes "Top")<br>
