# Color Analyzer
A **smart color collector** for your future design 💡 

A collector equipped with a **small camera and color-sensing device**. This enables designers to conveniently **capture and record colors or materials** they wish to collect anytime, anywhere, serving as **inspiration for future designs**.


## Visualization
![Color Analyzer 1](https://github.com/liliana0514/Color-Analyzer/blob/main/Color%20Analyzer%201.jpg?raw=true)

## The Sensor Device (Color Analyzer)
![Color Analyzer 2](https://github.com/liliana0514/Color-Analyzer/blob/main/Color%20Analyzer%202.jpg?raw=true)
### Components
- SEEED STUDIO XIAO ESP32S3 SENSE
- OV2640 Camera Module (Texture Imaging Sensor)
- VEML7700 (Lux Sensor)
- Button
- MicroSD Card Module


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

## The Display Device (Wireless Display Screen)
![Color Analyzer 3](https://github.com/liliana0514/Color-Analyzer/blob/main/Color%20Analyzer%203.jpg?raw=true)
### Components
- SEEED STUDIO XIAO ESP32S3 Wi-Fi/B
- LED
- Stepper gauge (Stepper Motor X27)
- ST7789 TFT LCD
- 3-pin Switch

### Communication
1. Power Supply
2. Ground (GND)
3. LEDs / Stepper Gauge / OLED Screen

## Communicated Information
### The Sensor Device
![Communicated Information01](https://github.com/liliana0514/Color-Analyzer/blob/main/Communicated%20Information01.jpg?raw=true)

### The Display Device
![Communicated Information02](https://github.com/liliana0514/Color-Analyzer/blob/main/Communicated%20Information02.jpg?raw=true)

## Information Architecture
![Information Architecture](https://github.com/liliana0514/Color-Analyzer/blob/main/Information%20Architecture.jpg?raw=true)

