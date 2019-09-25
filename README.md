# TrackCamera
 ESP32 Camera based on https://github.com/bitluni/ESP32CameraI2S/tree/master/ESP32_I2S_Camera
   - Modified to provide three Servo controls, nominally Speed, Up/Down and Left/Right.
   - Using Pins 12, 13, 15

# Dependencies ETC:
## Install Libraries:
 - Include ESP32: (Additional boards Manager URL https://dl.espressif.com/dl/package_esp32_index.json )
 - Add alternate Servo Library : https://github.com/RoboticsBrno/ESP32-Arduino-Servo-Library 
 - This must be installed to make servos work because this library allows you to select the timer channel to use.. but the 'standard ESP32Servo' does not.
 
## Arduino Settings: 
   - Board: "ESP32 Wrover Module"
   - Partition Scheme Default" or "Huge APP (3Mb No OTA)"
   - Core Debug Level "none"

### To Program ESP32Cam board 
   - GPIO 0 must be connected to GND to upload a sketch
   - After connecting GPIO 0 to GND, press the ESP32-CAM on-board RESET button to put your board in flashing mode

