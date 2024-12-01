# XIAO ESP32S3 Sense
**Table Of Contents**
* [Top](#xiao-esp32s3-sense "Top")
* [ESP32S3 Sense Information](#esp32s3-sense-information "ESP32S3 Sense Information")
* [Arduino IDE setup](#arduino-ide-setup "Arduino IDE setup")
* [Mods for Blink](#mods-for-blink "Mods for Blink")
* [Mods for CameraWebServer](#mods-for-camerawebserver "Mods for CameraWebServer")

## ESP32S3 Sense Information
[Top](#xiao-esp32s3-sense "Top")<br>
Thanks to **DroneBot** Workshop for their YouTube "XIAO ESP32S3 Sense - Tiny ESP32 Camera" from which I got this information!
- https://www.youtube.com/watch?v=qNzlytUdB_Q

<img src="https://github.com/Mark-MDO47/HalloweenEyes/blob/master/HW/XIAO_ESP32S3_Sense/images/XIAO_ESP32S3_Sense_IO.png" width="600" alt="Pinouts for XIAO ESP32S3 Sense">

<img src="https://github.com/Mark-MDO47/HalloweenEyes/blob/master/HW/XIAO_ESP32S3_Sense/images/XIAO_ESP32S3_Sense_Pinouts.png" width="600" alt="Pinouts for XIAO ESP32S3 Sense">

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
**IMPORTANT** - getting this wrong can destroy the HW module!!!<br>
<img src="https://github.com/Mark-MDO47/HalloweenEyes/blob/master/HW/XIAO_ESP32S3_Sense/images/XIAO_ESP32S3_Sense_ChooseCameraModel.png" width="600" alt="Choose the camera model for XIAO ESP32S3 Sense">
