# TrackCamera
 ESP32 Camera based on https://github.com/bitluni/ESP32CameraI2S/tree/master/ESP32_I2S_Camera

# Dependencies ETC:
Arduino Settings: 
Board: "ESP32 Wrover Module"
Partition Scheme Default" or "Huge APP (3Mb No OTA)"
Core Debug Level "none"

Install Libraries: 
 https://github.com/RoboticsBrno/ESP32-Arduino-Servo-Library 
 This must be installed to make servos work because this library allows you to select the timer channel to use.. but the 'standard ESP32Servo' does not.

TO Program ESP32Cam board 
   - GPIO 0 must be connected to GND to upload a sketch
   - After connecting GPIO 0 to GND, press the ESP32-CAM on-board RESET button to put your board in flashing mode

