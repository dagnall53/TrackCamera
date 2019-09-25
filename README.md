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

# Editing the HTML
  - Quick version (from RobotOne)(https://robotzero.one/esp32-cam-custom-html/)
  –&nbsp; <a href="https://gchq.github.io/CyberChef/#recipe=Gzip('Dynamic%20Huffman%20Coding','index.html.gz','',false)To_Hex('0x')Split('0x',',0x')&amp;input=PCFkb2N0eXBlIGh0bWw%2BCjxodG1sPgogICAgPGhlYWQ%2BCiAgICAgICAgPG1ldGEgY2hhcnNldD0idXRmLTgiPgogICAgICAgIDxtZXRhIG5hbWU9InZpZXdwb3J0IiBjb250ZW50PSJ3aWR0aD1kZXZpY2Utd2lkdGgsaW5pdGlhbC1zY2FsZT0xIj4KICAgICAgICA8dGl0bGU%2BUm9ib3QgWmVybyBPbmUgV2FzIEhlcmU8L3RpdGxlPgogICAgPC9oZWFkPgogICAgPGJvZHk%2BCiAgICAgICAgPGRpdiBpZD0ibG9nbyI%2BCiAgICAgICAgICAgIDxsYWJlbCBmb3I9Im5hdi10b2dnbGUtY2IiIGlkPSJuYXYtdG9nZ2xlIj4mIzk3NzY7Jm5ic3A7Jm5ic3A7VG9nZ2xlIHNldHRpbmdzPC9sYWJlbD4KICAgICAgICAgPC9kaXY%2BCiAgICA8L2JvZHk%2BCjwvaHRtbD4" target="_blank" rel="noopener">Click here</a> to open the CyberChef online tool, edit or paste your HTML in the Input field. The code you need to paste into the Arduino IDE will appear in the Output area. Copy all of it <strong>except</strong> the first comma, paste into camera_index.h.
  - I store my  HTML in the GIThub so it can be modifiied etc, then save the compressed data as 'download.dat'. This stores the compressed version with the the preceding ',' which needs to be removed before copying into camera_index.h line 6.
  

