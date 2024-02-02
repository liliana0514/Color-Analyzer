# Color Analyzer
A **smart color collector** for your future design 💡 

A collector equipped with a **small camera and color-sensing device**. This enables designers to conveniently **capture and record colors or materials** they wish to collect anytime, anywhere, serving as **inspiration for future designs**.


## Visualization
![Color Analyzer 1](https://github.com/liliana0514/Color-Analyzer/blob/main/Color%20Analyzer%201.jpg?raw=true)

## The Sensor Device (Color Analyzer)
![The Sensor Device](https://github.com/liliana0514/Color-Analyzer/blob/main/Color%20Analyzer%202.jpg?raw=true)
### Components
- SEEED STUDIO XIAO ESP32S3 SENSE
- OV2640 Camera Module (Texture Imaging Sensor)
- VEML7700 (Lux Sensor)
- Button(6x6mm)
- MicroSD Card Module

### Communication
- **Bluetooth Communication Setup**:
  - Configure the ESP32's Bluetooth module as a Bluetooth transmitter.
  - Implement a protocol to send captured images, color data (RGB), and lux readings.
- **Sensor Integration**:
  - Connect VEML7700 to the ESP32 using I2C or SPI, depending on the sensor’s interface.
- **Data Processing**:
  - Program the ESP32 to process sensor data, resize images, and package this data for Bluetooth transmission.
- **Power Supply**:
  - Connect the VCC of all components to a suitable power source, ensuring compatibility with their voltage requirements.
- **Ground (GND)**:
  - Connect the GND of all components together to ensure a common ground reference.

### **Programming**:
- Program to handle image capture, color detection, lux measurement, and Bluetooth data transmission.

## The Display Device (Wireless Display Screen)
![Color Analyzer 3](https://github.com/liliana0514/Color-Analyzer/blob/main/Color%20Analyzer%203.jpg?raw=true)
### Components
- SEEED STUDIO XIAO ESP32S3 Wi-Fi/B
- LED
- X27 168 Stepper Motor
- ILI9341 2.8" SPI TFT LCD
- 3-pin Switch

### Communication
- **Bluetooth Communication Setup**:
  - Set up the ESP32's Bluetooth module as a receiver.
  - Implement a protocol to receive data (images and lux readings) from the Sensor Device.
- **Display and Actuator Control**:
  - Interface the ESP32 with the ILI9341 2.8" SPI TFT LCD via SPI for image display.
  - Connect and program the stepper motor and LEDs to respond to received data (e.g., lux readings and color data).
- **Power Supply**:
  - Connect the VCC of all components to a suitable power source, ensuring compatibility with their voltage requirements.
- **Ground (GND)**:
  - Connect the GND of all components together to ensure a common ground reference.
 
### General Connectivity:
- **Bluetooth Communication**:
  - Set up ESP32S3 SENSE to transmit image data and lux readings over Bluetooth.
  - Configure ESP32S3 Wi-Fi/B to receive this data and process it accordingly.
- **SPI Connection for ST7789 TFT LCD**:
  - Use SPI pins on ESP32S3 Wi-Fi/B to interface with the LCD.

### Programming:
- Program to receive Bluetooth data, control the stepper motor, update LEDs, and display images and RGB values on the LCD.

### Testing and Validation:
- Test the Bluetooth communication to ensure data is accurately sent and received.
- Validate the functionality of the stepper motor and LEDs based on the received data.
- Check the display quality and responsiveness of the ST7789 TFT LCD.

## Communicated Information
### The Sensor Device
![Communicated Information02](https://github.com/liliana0514/Color-Analyzer/blob/main/Communicated%20Information01_Sensor%20Device.jpg?raw=true)

### The Display Device
![Communicated Information02](https://github.com/liliana0514/Color-Analyzer/blob/main/Communicated%20Information01_Display%20Device.jpg?raw=true)

## Information Architecture
![Information Architecture](https://github.com/liliana0514/Color-Analyzer/blob/main/Information%20Architecture.jpg?raw=true)

