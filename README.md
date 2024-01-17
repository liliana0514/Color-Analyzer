# Color Analyzer
A **smart color collector** for your future design 💡 

A collector equipped with a **small camera and color-sensing device**. This enables designers to conveniently **capture and record colors or materials** they wish to collect anytime, anywhere, serving as **inspiration for future designs**.


## Visualization
![Braindump-41]([https://github.com/yinyin13/lumiere/assets/148395165/aa7f0345-1a8c-4b89-a30b-348738f54d1c](https://github.com/liliana0514/Color-Analyzer/blob/main/Color%20Analyzer%201.jpg))

## The Sensor Device (Ceiling Light)
### Components
- ESP32 microcontroller
- TCS34725 RGB(Color Sensor)
- OV7670 Camera Module(Texture Imaging Sensor)
- VEML7700 (light sensor)
- Buttons(switch between different modes)


### Communication
1. Power Supply:
- Connect the VCC of all components (ESP32, TCS34725, OV7670, VEML7700) to a suitable power source.
2. Ground (GND):
- Connect the GND (Ground) of all components (ESP32, TCS34725, OV7670, VEML7700) together. 
3. I2C Communication (ESP32, TCS34725, VEML7700)
- Connect the SDA (data line) and SCL (clock line) pins of the ESP32 to the corresponding pins on the TCS34725 and VEML7700 for I2C communication.
4. Camera Module (OV7670):
- Connect the camera module to the ESP32 using appropriate pins for communication. Consider voltage level compatibility and required resistors for signal conditioning.
5. Buttons:
- Connect the buttons to the ESP32 for user input. Implement debounce circuits if needed to ensure reliable button presses.
6. Mode Switching:
- Use the buttons to toggle between different modes of operation, such as capturing color data, capturing texture images, or adjusting settings.

## The Display Device (Remote Control)
### Components
- ESP32 microcontroller
- LED
- Stepper gauge
- OLED screen  SSD1316



### Communication
1. Power Supply:
- Connect the VCC of all components (ESP32, TCS34725, OV7670, VEML7700) to a suitable power source.


## Diagram
![diagram 001](https://github.com/yinyin13/lumiere/assets/148395165/837b9d80-019b-4136-94b9-cce0888619b1)
