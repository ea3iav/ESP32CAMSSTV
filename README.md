# ESP32CAMSSTV
Simple sstv picture sending for radioamateur.
This project uses an ESP32 microcontroller with an OV2640 camera module to enable image capture, audio output, and LED control. It also includes Push-to-Talk (PTT) functionality.
based on this project 
http://blog.dzl.dk/2022/09/14/stand-alone-sstv-camera/
I added possibility to add two lines of text with you call sign for example. a ptt action when pocture is sent

it will make and send picture when reset is pressed or immediatelly when connected to 5v
You need ESP32 library for arduino and a ESP32-cam board
   +------------------+
        |      ESP32       |
        |                  |
        |   [GPIO 4]  -----> LED Flash
        |  
        |  [GPIO 14]  -----> Speaker (Audio Output)
        |  [GPIO 15]  -----> PTT (Push-to-Talk)
        |                  |
        |  
        |                  |
        +------------------+

        Need to wire it accordingly to your radio input pinout. 
        
🚀 Features
📷 Camera Support: Captures images using the OV2640 camera module.
🔊 Audio Output: Sends audio signals to a speaker via GPIO 14.
💡 LED Control: Controls an LED flash (GPIO 4) and a red status LED (GPIO 33).
🎤 Push-to-Talk (PTT): Enables PTT functionality through GPIO 15.
🔧 Setup & Installation
Flash the ESP32: Load the firmware using Arduino IDE or PlatformIO.
Connect the Components: Ensure all peripherals (camera, speaker, LEDs) are wired correctly.
Power the Board: Use a 5V power source or USB connection.
        
