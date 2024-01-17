# Color Analyzer
A **smart color collector** for your future design 💡 

A collector equipped with a **small camera and color-sensing device**. This enables designers to conveniently **capture and record colors or materials** they wish to collect anytime, anywhere, serving as **inspiration for future designs**.


## Visualization
![Braindump-41](https://github.com/yinyin13/lumiere/assets/148395165/aa7f0345-1a8c-4b89-a30b-348738f54d1c)

## The Sensor Device (Ceiling Light)
### Components
- VEML7700 sensor
- BME280 sensor
- ESP32 microcontroller
- LED * 2

### Communication
1. Connect the components
2. Program the ESP32 to read temperature and lux data from VEML7700 and BME280
3. Program the ESP32 to send data to Display device via Bluetooth

## The Display Device (Remote Control)
### Components
- Stepper gauge
- ESP32 microcontroller
- LED
- Buttons

### Communication
1. Connect the components
2. ESP32 receives data from the Sensor device
3. Program ESP32 to control the stepper gauge to indicate brightness
4. Program ESP32 to send adjustment commands to the Sensor device

## Diagram
![diagram 001](https://github.com/yinyin13/lumiere/assets/148395165/837b9d80-019b-4136-94b9-cce0888619b1)
