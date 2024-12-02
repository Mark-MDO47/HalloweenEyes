# XIAO ESP32S3 Sense
**Table Of Contents**
* [Top](#xiao-esp32s3-sense "Top")
* [ESP32S3 Sense Information](#esp32s3-sense-information "ESP32S3 Sense Information")
* [Arduino IDE setup](#arduino-ide-setup "Arduino IDE setup")
* [Mods for Blink](#mods-for-blink "Mods for Blink")
* [Mods for CameraWebServer](#mods-for-camerawebserver "Mods for CameraWebServer")
* [Mods for SD_Test](#mods-for-sd_test "Mods for SD_Test")

## ESP32S3 Sense Information
[Top](#xiao-esp32s3-sense "Top")<br>
Images of XIAO ESP32S3 Sense and its pinouts are from https://www.seeedstudio.com/XIAO-ESP32S3-Sense-p-5639.html

<img src="https://github.com/Mark-MDO47/HalloweenEyes/blob/master/HW/XIAO_ESP32S3_Sense/images/XIAO_ESP32S3_Sense_IO.png" width="600" alt="Pinouts for XIAO ESP32S3 Sense">

<img src="https://github.com/Mark-MDO47/HalloweenEyes/blob/master/HW/XIAO_ESP32S3_Sense/images/XIAO_ESP32S3_Sense_Pinouts.png" width="600" alt="Pinouts for XIAO ESP32S3 Sense">

<img src="https://github.com/Mark-MDO47/HalloweenEyes/blob/master/HW/XIAO_ESP32S3_Sense/images/XIAO_ESP32S3_Sense_Pinouts_Back.png" width="600" alt="Pinouts for the back of the XIAO ESP32S3 Sense">

<img src="https://github.com/Mark-MDO47/HalloweenEyes/blob/master/HW/XIAO_ESP32S3_Sense/images/XIAO_ESP32S3_Sense_Pinouts_Camera.png" width="600" alt="Pinouts for the OV2640 camera for the XIAO ESP32S3 Sense">

Following image frm https://wiki.seeedstudio.com/xiao_esp32s3_sense_filesystem/#prepare-the-microsd-card<br>
<img src="https://github.com/Mark-MDO47/HalloweenEyes/blob/master/HW/XIAO_ESP32S3_Sense/images/XIAO_ESP32S3_Sense_SDcard_IO.png" width="600" alt="Pinouts used for SD card slot of the XIAO ESP32S3 Sense">


Thanks to **DroneBot Workshop** for their YouTube "XIAO ESP32S3 Sense - Tiny ESP32 Camera".
- https://www.youtube.com/watch?v=qNzlytUdB_Q

As mentioned in this video, there are a couple of oddities you might see when using this module.

1. You may have trouble loading the module, getting "No serial data received" for example. In this case, use a toothpick or non-conducting probe to hold the "Boot" button down before inserting the USB cable and it may load again.<br>
<img src="https://github.com/Mark-MDO47/HalloweenEyes/blob/master/HW/XIAO_ESP32S3_Sense/images/XIAO_ESP32S3_Sense_NoSerialDataRcvd.png" width="600" alt="XIAO ESP32S3 Sense getting No serial data received">

2. After loading, the module may just not run. In this case, disconnect the USB cable and re-connect and it may start running. Otherwise, try re-loading.

Also thanks to the **techiesms** YouTube "Smallest Camera Module based on ESP32 S3 | XIAO ESP32S3 Sense"
- https://www.youtube.com/watch?v=_wvuOsRgmt4

## Arduino IDE setup
[Top](#xiao-esp32s3-sense "Top")<br>
This shows how to select the XIAO ESP32S3 Sense board in Arduino IDE.<br>
<img src="https://github.com/Mark-MDO47/HalloweenEyes/blob/master/HW/XIAO_ESP32S3_Sense/images/XIAO_ESP32S3_Sense_Board_Arduino.png" width="600" alt="Selecting XIAO ESP32S3 Sense board in Arduino IDE">

Then enable the OPI PSRAM as shown here.<br>
<img src="https://github.com/Mark-MDO47/HalloweenEyes/blob/master/HW/XIAO_ESP32S3_Sense/images/XIAO_ESP32S3_Sense_EnableOpiPsram.png" width="600" alt="Enable XIAO ESP32S3 Sense OPI PSRAM in Arduino IDE">


## Mods for Blink
[Top](#xiao-esp32s3-sense "Top")<br>
Pin 21 is used for the internal LED.<br>
<img src="https://github.com/Mark-MDO47/HalloweenEyes/blob/master/HW/XIAO_ESP32S3_Sense/images/XIAO_ESP32S3_Sense_InternalLED.png" width="400" alt="Editing pin for internal LED for XIAO ESP32S3 Sense">

## Mods for CameraWebServer
[Top](#xiao-esp32s3-sense "Top")<br>
Choose the camera model for XIAO ESP32S3 Sense.<br>
<img src="https://github.com/Mark-MDO47/HalloweenEyes/blob/master/HW/XIAO_ESP32S3_Sense/images/XIAO_ESP32S3_Sense_ChooseCameraModel.png" width="600" alt="Choose the camera model for XIAO ESP32S3 Sense">

## Mods for SD_Test

<img src="https://github.com/Mark-MDO47/HalloweenEyes/blob/master/HW/XIAO_ESP32S3_Sense/images/XIAO_ESP32S3_Sense_mod4TestSD.png" width="600" alt="Specify SD Card pin for XIAO ESP32S3 Sense">
