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
- **Bluetooth Communication Setup**:
  - Configure the ESP32's Bluetooth module as a Bluetooth transmitter.
  - Implement a protocol to send captured images, color data (RGB), and lux readings.
- **Sensor Integration**:
  - Connect sensors (like the TCS34725 and VEML7700) to the ESP32 using I2C or SPI, depending on the sensor’s interface.
- **Data Processing**:
  - Program the ESP32 to process sensor data, resize images, and package this data for Bluetooth transmission.

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

